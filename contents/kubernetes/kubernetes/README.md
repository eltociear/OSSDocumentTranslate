# Kubernetes (K8s)

[![GoPkg Widget]][GoPkg] [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/569/badge)](https://bestpractices.coreinfrastructure.org/projects/569)

<img src="https://github.com/kubernetes/kubernetes/raw/master/logo/logo.png" width="100">

----

KubernetesはK8sと呼ばれ、複数のホスト間で [コンテナ化されたアプリケーション] を管理するためのオープンソースシステムです。
これはアプリケーションの展開、保守、及びスケーリングの為の基本的なメカニズムを提供します。

Kubernetesは [Borg] と呼ばれるシステムを使用して、本番ワークロードを大規模に実行するGoogleでの10年半の経験と
コミュニティからの最高のアイディアと実践を組み合わせに基づいてビルドされています。

Kubernetesは Cloud Native Computing Foundation ([CNCF]) によってホスティングされています。
コンテナパッケージ化、動的スケジューリング、マイクロサービス指向の技術は
CNCFへの参加を検討して下さい。
誰が関与し、Kubernetesがどのような役割を果たすかについての詳細は、 [announcement] をお読み下さい。

----

## K8sの使用を開始するには

[kubernetes.io] のドキュメントを御覧ください。

[interactive tutorial] をお試し下さい。

[Scalable Microservices with Kubernetes] の無料コースを受講して下さい。

その他のアプリケーションでのライブラリとしてKubernetesコードを使用するには、 [list of published components](https://git.k8s.io/kubernetes/staging/README.md) を参照して下さい。
ライブラリとしての `k8s.io/kubernetes` モジュールまたは、 `k8s.io/kubernetes/...` パッケージの使用はサポートされていません。

## K8sの開発を開始するには

[community repository] は、ソースからKubernetesをビルドする方法、
コードとドキュメントにコントリビュートする方法、
誰に何を連絡するかなどに関する全ての情報をホストします。

Kubernetesをすぐにビルドする場合は、次の2つのオプションがあります：

##### [Go environment] での実行

```
mkdir -p $GOPATH/src/k8s.io
cd $GOPATH/src/k8s.io
git clone https://github.com/kubernetes/kubernetes
cd kubernetes
make
```

##### [Docker environment] での実行

```
git clone https://github.com/kubernetes/kubernetes
cd kubernetes
make quick-release
```

詳細については、 [developer's documentation] を御覧ください。

## サポート

サポートが必要な場合は、 [troubleshooting guide] から始めて、概説したプロセスを進めて下さい。

質問がある場合、 [one way or another][communication] からお問い合わせ下さい。

[announcement]: https://cncf.io/news/announcement/2015/07/new-cloud-native-computing-foundation-drive-alignment-among-container
[Borg]: https://research.google.com/pubs/pub43438.html
[CNCF]: https://www.cncf.io/about
[communication]: https://git.k8s.io/community/communication
[community repository]: https://git.k8s.io/community
[containerized applications]: https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/
[developer's documentation]: https://git.k8s.io/community/contributors/devel#readme
[Docker environment]: https://docs.docker.com/engine
[Go environment]: https://golang.org/doc/install
[GoPkg]: https://pkg.go.dev/k8s.io/kubernetes
[GoPkg Widget]: https://pkg.go.dev/badge/k8s.io/kubernetes.svg
[interactive tutorial]: https://kubernetes.io/docs/tutorials/kubernetes-basics
[kubernetes.io]: https://kubernetes.io
[Scalable Microservices with Kubernetes]: https://www.udacity.com/course/scalable-microservices-with-kubernetes--ud615
[troubleshooting guide]: https://kubernetes.io/docs/tasks/debug-application-cluster/troubleshooting/

---
[オリジナル](https://github.com/kubernetes/kubernetes/blob/master/README.md)
