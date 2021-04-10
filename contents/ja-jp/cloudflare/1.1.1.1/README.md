# 1.1.1.1 Site

### _Cloudflare DNS リゾルバーとWarpのウェブサイト_

## コントリビュート

1.1.1.1ドキュメントサイトは、TypeScript、Pugテンプレート、およびStylusスタイルシートを使用して構築されています。Webpackは、これらのアセットをCloudflareでホストされているビルドにコンパイルするために使用されます。ローカルコピーは、最初にYarn（またはNPM）を使用してプロジェクトの依存関係をインストールすることで実行できます。

### 要件

- *nixまたはMacOSオペレーティングシステム
- Node 9.x以降

```bash
yarn install
```

上記コマンドが完了したら、開発サーバーを起動します。

```bash
yarn start
```

コンソールには、プロジェクトに対応するIPアドレスが表示されます。

---
[オリジナル](https://github.com/cloudflare/1.1.1.1/blob/master/README.md)
