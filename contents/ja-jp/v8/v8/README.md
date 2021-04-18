V8 JavaScript エンジン
=============

V8はGoogleのオープンソースJavaScriptエンジンです。

V8は、ECMA-262で指定されているようにECMAScriptを実装します。

V8はC++で記述されており、GoogleのオープンソースブラウザであるGoogle Chromeで使用されています。

V8はスタンドアロンで実行することも、任意のC++アプリケーションに組み込むこともできます。

V8ロジェクトページ：https://v8.dev/docs


コードの取得
=============

[デポツール](http://www.chromium.org/developers/how-tos/install-depot-tools)をチェックアウトし、下記を実行します

        fetch v8

これにより、V8がディレクトリ `v8`にチェックアウトされ、そのすべての依存関係がフェッチされます。
最新の状態に保つには、下記を実行します

        git pull origin
        gclient sync

すべてのブランチをフェッチするには`.git/config`のリモート構成に以下を追加します：

        fetch = +refs/branch-heads/*:refs/remotes/branch-heads/*
        fetch = +refs/tags/*:refs/tags/*


コントリビュート
=============

[v8.dev/docs/contribute](https://v8.dev/docs/contribute)に記載されている手順に従ってください 。

---
[オリジナル](https://github.com/v8/v8/blob/master/README.md)
