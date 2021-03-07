<p align="center">
  <a href="https://babeljs.io/">
    <img alt="babel" src="https://raw.githubusercontent.com/babel/logo/master/babel.png" width="546">
  </a>
</p>

<p align="center">
  次世代JavaScriptを作成するためのコンパイラ。
</p>

<p align="center">
  <a href="https://gitpod.io/#https://github.com/babel/babel"><img alt="Gitpod ready-to-code" src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod"></a>
</p>
<p align="center">
    <a href="https://www.npmjs.com/package/@babel/core"><img alt="v7 npm Downloads" src="https://img.shields.io/npm/dm/@babel/core.svg?maxAge=43200&label=v7%20downloads"></a>
  <a href="https://www.npmjs.com/package/babel-core"><img alt="v6 npm Downloads" src="https://img.shields.io/npm/dm/babel-core.svg?maxAge=43200&label=v6%20downloads"></a>
</p>
<p align="center">
  <a href="https://circleci.com/gh/babel/babel"><img alt="CircleCI Status" src="https://img.shields.io/circleci/project/github/babel/babel/main.svg?label=circle&maxAge=43200"></a>
  <a href="https://codecov.io/github/babel/babel"><img alt="Coverage Status" src="https://img.shields.io/codecov/c/github/babel/babel/main.svg?maxAge=43200"></a>
  <a href="https://slack.babeljs.io/"><img alt="Slack Status" src="https://slack.babeljs.io/badge.svg"></a>
  <a href="https://twitter.com/intent/follow?screen_name=babeljs"><img alt="Follow on Twitter" src="https://img.shields.io/twitter/follow/babeljs.svg?style=social&label=Follow"></a>
</p>

<h2 align="center">Babelのサポーター</h2>

<p align="center">
  <a href="#backers"><img alt="Backers on Open Collective" src="https://opencollective.com/babel/backers/badge.svg" /></a>
  <a href="#sponsors"><img alt="Sponsors on Open Collective" src="https://opencollective.com/babel/sponsors/badge.svg" /></a>
  <a href="https://medium.com/friendship-dot-js/i-peeked-into-my-node-modules-directory-and-you-wont-believe-what-happened-next-b89f63d21558"><img alt="Business Strategy Status" src="https://img.shields.io/badge/business%20model-flavortown-green.svg"></a>
</p>

Babel (["バベル"](https://soundcloud.com/sebmck/how-to-pronounce-babel)と発音)は、多くの企業やプロジェクトで使用されているコミュニティ主導のプロジェクトであり、[ボランティア](https://babeljs.io/team)のグループによって維持されています。プロジェクトの将来をサポートしたい場合は、以下を検討してください：

- プロジェクトに開発期間を与える。 ([Twitter](https://twitter.com/babeljs)または、[Slack](https://slack.babeljs.io/)でガイダンスを入手してください！)
- [Open Collective](https://opencollective.com/babel)または、[Patreon](https://www.patreon.com/henryzhu)のスポンサーになることで資金を提供する！

## スポンサー

トップスポンサーは以下の通りです！ [[スポンサーになる](https://opencollective.com/babel#sponsor)]

<a href="https://opencollective.com/babel/sponsor/0/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/0/avatar.svg"></a>
<a href="https://opencollective.com/babel/sponsor/1/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/1/avatar.svg"></a>
<a href="https://opencollective.com/babel/sponsor/2/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/2/avatar.svg"></a>
<a href="https://opencollective.com/babel/sponsor/3/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/3/avatar.svg"></a>
<a href="https://opencollective.com/babel/sponsor/4/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/4/avatar.svg"></a>
 <a href="https://opencollective.com/babel/sponsor/5/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/5/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/6/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/6/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/7/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/7/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/8/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/8/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/9/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/9/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/10/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/10/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/11/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/11/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/12/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/12/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/13/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/13/avatar.svg"></a>
  <a href="https://opencollective.com/babel/sponsor/14/website" target="_blank"><img src="https://opencollective.com/babel/sponsor/14/avatar.svg"></a>

## 概論

Babelは、最新バージョンのJavaScriptでコードを作成するのに役立つツールです。サポートされている環境が特定の機能をネイティブにサポートしていない場合、Babelはそれらの機能をサポートされているバージョンにコンパイルするのに役立ちます。

**入力**

```js
// ES2020 Null 合体演算子
function greet(input) {
  return input ?? "Hello world";
}
```

**出力**

```js
function greet(input) {
  return input != null ? input : "Hello world";
}
```

私たちの[REPL](https://babel.dev/repl#?browsers=defaults%2C%20not%20ie%2011&loose=true&code_lz=GYVwdgxgLglg9mABAcwE4FN1QBQzABxCgEpEBvAKEUQyhFST0KkQH5XEAiACXQBs-cRAHc4qPgBNOAbgoBfIA&shippedProposals=true&sourceType=script&lineWrap=true&presets=env%2Cenv&prettier=true)で試してみてください。

## FAQ

### Babelをメンテナンスしているのは誰ですか？

ほとんどの場合、あなたが資金を提供している一握りのボランティアです！[team page](https://babeljs.io/team)をご覧下さい。

### Babelの歌はありますか？

私はあなたが尋ねてくれてとてもうれしいです： [@angus-c](https://github.com/angus-c)による[Hallelujah —— Babelを讃えて](SONG.md)、[@swyx](https://twitter.com/@swyx)による[audio version](https://youtu.be/40abpedBKK8)。あなたの録音をツイートしてください！

### サポートを探していますか？

質問やサポートについては、[Slack Community](https://slack.babeljs.io/)に参加する([ここでsign up](https://slack.babeljs.io/)して招待状を受け取る)か、[Stack Overflow](https://stackoverflow.com/questions/tagged/babeljs)で質問するか、[Twitter](https://twitter.com/babeljs)でpingを送信してください。

### ドキュメントはどこですか？

私たちのWebサイトをチェックしてください： [babeljs.io](https://babeljs.io/)または、[babel/website](https://github.com/babel/website/issues)で問題/機能を報告します。

### バグを報告したり、機能をリクエストしたりしたいですか？

[CONTRIBUTING.md](CONTRIBUTING.md)を読み、[babel/issues](https://github.com/babel/babel/issues)で問題テンプレートに記入してください！

### Babelにコントリビュートしてみませんか？

確認：

- 私達の[#development](https://babeljs.slack.com/messages/development) Slack channelで挨拶する！([sign-up](https://slack.babeljs.io))
- [good first issue](https://github.com/babel/babel/labels/good%20first%20issue)と、[help wanted](https://github.com/babel/babel/labels/help%20wanted)ラベル。取り組むことができる問題の種類を理解するために[closedのissue](https://github.com/babel/babel/issues?utf8=%E2%9C%93&q=is%3Aclosed+label%3A%22good+first+issue%22)も確認することをお勧めします。

リソース：

- [CONTRIBUTING.md](CONTRIBUTING.md)を使用して、リポジトリの設定を開始します。
- 議論/ノート/ロードマップ： [babel/notes](https://github.com/babel/notes)
- TC39提案の進捗状況： [babel/proposals](https://github.com/babel/proposals)
- リリース投稿と説明を含むブログ： [/blog](https://babeljs.io/blog)
- オープンソースとBabelについての話のビデオページ： [/videos](https://babeljs.io/videos)
- [podcast](https://podcast.babeljs.io)

### リポジトリはどのように構成されていますか？

Babelリポジトリは、多くの[npmパッケージ](packages/README.md)で構成される[monorepo](doc/design/monorepo.md)として管理されます。

## ライセンス

[MIT](LICENSE)

---
[オリジナル](https://github.com/babel/babel/blob/main/README.md)
