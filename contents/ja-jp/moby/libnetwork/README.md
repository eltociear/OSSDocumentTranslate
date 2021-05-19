# libnetwork - コンテナのネットワーキング

[![Circle CI](https://circleci.com/gh/docker/libnetwork/tree/master.svg?style=svg)](https://circleci.com/gh/docker/libnetwork/tree/master) [![Coverage Status](https://coveralls.io/repos/docker/libnetwork/badge.svg)](https://coveralls.io/r/docker/libnetwork) [![GoDoc](https://godoc.org/github.com/docker/libnetwork?status.svg)](https://godoc.org/github.com/docker/libnetwork) [![Go Report Card](https://goreportcard.com/badge/github.com/docker/libnetwork)](https://goreportcard.com/report/github.com/docker/libnetwork)

Libnetworkは、コンテナーを接続するためのネイティブGo実装を提供します

libnetworkの目標は、一貫性のあるプログラミングインターフェイスとアプリケーションに必要なネットワーク抽象化を提供する堅牢なコンテナネットワークモデルを提供することです。

#### デザイン
詳細については、[デザイン](docs/design.md)を参照してください。

#### libnetworkの使用

幅広いユースケースに適合するために利用できる多くのネットワーキングソリューションがあります。libnetworkは、ドライバー/プラグインモデルを使用して、これらすべてのソリューションをサポートすると同時に、シンプルで一貫性のあるネットワークモデルをユーザーに公開することで、ドライバー実装の複雑さを抽象化します。


```go
import (
	"fmt"
	"log"

	"github.com/docker/docker/pkg/reexec"
	"github.com/docker/libnetwork"
	"github.com/docker/libnetwork/config"
	"github.com/docker/libnetwork/netlabel"
	"github.com/docker/libnetwork/options"
)

func main() {
	if reexec.Init() {
		return
	}

	// ネットワークドライバーを選択して構成します
	networkType := "bridge"

	// 新しいコントローラインスタンスを作成
	driverOptions := options.Generic{}
	genericOption := make(map[string]interface{})
	genericOption[netlabel.GenericData] = driverOptions
	controller, err := libnetwork.New(config.OptionDriverConfig(networkType, genericOption))
	if err != nil {
		log.Fatalf("libnetwork.New: %s", err)
	}

	// コンテナが参加するためのネットワークを作成します。
	// NewNetworkは、libnetworkとDriversが使用できる可変個引数のオプションの引数を受け入れます。
	network, err := controller.NewNetwork(networkType, "network1", "")
	if err != nil {
		log.Fatalf("controller.NewNetwork: %s", err)
	}

	// 新しいコンテナごと：IPとインターフェースを割り当てます。返されたネットワーク設定は、
	// コンテナ情報（検査など）、およびポート公開のiptablesルールに使用されます。
	// この情報は含まれているか、返されたエンドポイントからアクセスできます。
	ep, err := network.CreateEndpoint("Endpoint1")
	if err != nil {
		log.Fatalf("network.CreateEndpoint: %s", err)
	}

	// コンテナのサンドボックスを作成します。
	// NewSandboxは、libnetworkが使用できる可変個引数のオプションの引数を受け入れます。
	sbx, err := controller.NewSandbox("container1",
		libnetwork.OptionHostname("test"),
		libnetwork.OptionDomainname("docker.io"))
	if err != nil {
		log.Fatalf("controller.NewSandbox: %s", err)
	}

	// サンドボックスは、join apiを介してエンドポイントに参加できます。
	err = ep.Join(sbx)
	if err != nil {
		log.Fatalf("ep.Join: %s", err)
	}

	// libnetworkクライアントは、Info() APIを介してエンドポイントの運用データを確認できます
	epInfo, err := ep.DriverInfo()
	if err != nil {
		log.Fatalf("ep.DriverInfo: %s", err)
	}

	macAddress, ok := epInfo[netlabel.MacAddress]
	if !ok {
		log.Fatalf("failed to get mac address from endpoint info")
	}

	fmt.Printf("Joined endpoint %s (%s) to sandbox %s (%s)\n", ep.Name(), macAddress, sbx.ContainerID(), sbx.Key())
}
```

## コントリビュート

libnetworkをハックしたいですか？[Dockerのコントリビューションガイド](https://github.com/docker/docker/blob/master/CONTRIBUTING.md)が適用されます。

## 著作権とライセンス
コードとドキュメントの著作権 2015 Docker, inc。Apache 2.0 licenseの下でリリースされたコード。クリエイティブ・コモンズの下でリリースされたドキュメント。

---
[オリジナル](https://github.com/moby/libnetwork/blob/master/README.md)
