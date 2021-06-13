# iota.go

公式Goライブラリ。

このライブラリを使用すると、次のことができます：

- インデックス作成とトランザクションペイロードを使用してメッセージを作成する
- メッセージと出力を取得する
- トランザクションに署名する
- アドレスを生成する
- IOTAノードと対話する
- Goベースのノードソフトウェアの基盤として機能する

より高度なアカウント管理が必要な場合は、
PythonとJavaScriptでバインディングも提供している[wallet.rs](https://github.com/iotaledger/wallet.rs)をご覧ください。

## 要件

> このライブラリは主にGoバージョン1.16.xでテストされました

ライブラリを使用するには、Goを[最新の安定バージョンに](https://golang.org/)更新することをお勧めします。

## ライブラリの使用

ライブラリの使用は簡単です。他の依存関係と同じように`go get`するだけです：

```bash
go get github.com/iotaledger/iota.go/v2
```

## APIリファレンス

[ここ](https://pkg.go.dev/github.com/iotaledger/iota.go/v2)でAPIリファレンスを読むことができます。

## ディスカッションに参加する

コミュニティに参加したい場合、セットアップのサポートが必要な場合、問題がある場合、またはIOTAについて他の人と話し合いたい場合は、
[Discord](https://discord.iota.org/)の`#clients-dev`または`#clients-discussion`チャンネルに参加してください。

## ライセンス

MITライセンスは[ここ](LICENSE)にあります。

---
[オリジナル](https://github.com/iotaledger/iota.go/blob/main/README.md)
