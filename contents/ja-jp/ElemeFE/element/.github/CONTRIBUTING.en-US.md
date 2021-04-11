# Element UIコントリビュートガイド

こんにちは！ElementUIをお選びいただきありがとうございます。

Element UIは、開発者、デザイナー、製品マネージャー向けのVue2.0ベースのコンポーネントライブラリです。

Elementへの貢献に関心をお寄せいただきありがとうございます。ただし、投稿を送信する前に、少し時間を取って、次のガイドラインをよく読んでください。

## Issueガイドライン

- Issueは、バグレポート、機能のリクエスト、および設計関連のトピック専用です。その他の質問は直接締め切られる場合があります。Elementの使用中に質問が発生した場合は、[Gitter](https://gitter.im/element-en/Lobby)でヘルプを求めてください。

- Issueを提出する前に、同様のIssueがすでに発行されているかどうかを確認してください。

- 使用している`Element`と`Vue`のバージョンを指定し、OSとブラウザの情報を提供してください。[JSFiddle](https://jsfiddle.net/)は、Issueを明確に再現できるように、ライブデモを作成することをお勧めします。

## プルリクエストガイドライン

- このリポジトリを自分のアカウントにフォークします。ここでブランチを作成しないでください。

- コミット情報は`[Component Name]: Info about commit.`のようにフォーマットする必要があります　(例 `Button: Fix xxx bug`)

- `lib`ディレクトリ内にファイルを含め **ない** でください。

- `npm run dist`を実行すると正しいファイルが出力されることを確認してください。

- 互換性とファイルサイズのために、私たちのbabel構成は`preset-2015`のみをインポートしたため、`ES2015`の`Array.prototype.find`や`Object.assign`のようなAPIは推奨されません。必要に応じて、サードパーティのポリフィルをインポートできます。

- PRを作成する前にリベースして、コミット履歴を明確に保ちます。

- PRが`dev`ブランチではなく`master`ブランチに作成されていることを確認してください。

- PRでバグが修正された場合は、関連するバグについて説明してください。

- PRのマージには、2人のメンテナが必要です。1人はレビュー後に変更を承認し、もう1人はレビューしてマージします。

## 前提条件
`Node.js 4以降`、`yarn`及び`npm 3+`が必要です。注：依存関係のバージョンをロックするためにyarnを使用するため、`npm install`の代わりに`yarn`を使用して依存関係をインストールする必要があります。
```shell
git clone git@github.com:ElemeFE/element.git
npm run dev

# http://localhost:8085 を開く
```

> **注意** ：`examples/play/index.vue`ファイルを変更し、提供したコンポーネントを使用してから、`npm run dev:play`を実行し、[http://localhost:8085](http://localhost:8085)を実行して取得します。その結果、より早く分かりやすくなります。

ビルドするには：

```shell
npm run dist
```

## コンポーネント開発ガイドライン
- `make new <component-name>`を実行して、新しいコンポーネントのプロジェクトディレクトリを作成します。テストコード、エントリーファイル、ドキュメントが含まれています。
- ネストされたコンポーネントについては、`Button`を参照してください。
- 他のコンポーネントに依存するコンポーネントについては、`Select`を参照してください。

## コードスタイル
[ElemeFE](https://github.com/elemefe)の[ESLint](https://github.com/ElemeFE/eslint-config-elemefe)設定に従うだけです。

---
[オリジナル](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.en-US.md)
