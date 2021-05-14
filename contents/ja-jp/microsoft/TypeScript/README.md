
# TypeScript

[![GitHub Actions CI](https://github.com/microsoft/TypeScript/workflows/CI/badge.svg)](https://github.com/microsoft/TypeScript/actions?query=workflow%3ACI)
[![Devops Build Status](https://dev.azure.com/typescript/TypeScript/_apis/build/status/Typescript/node10)](https://dev.azure.com/typescript/TypeScript/_build?definitionId=7)
[![npm version](https://badge.fury.io/js/typescript.svg)](https://www.npmjs.com/package/typescript)
[![Downloads](https://img.shields.io/npm/dm/typescript.svg)](https://www.npmjs.com/package/typescript)

[TypeScript](https://www.typescriptlang.org/)は、アプリケーション規模のJavaScript用の言語です。TypeScriptは、任意のブラウザ、任意のホスト、任意のOSの大規模なJavaScriptアプリケーション用のツールをサポートするオプションの型をJavaScriptに追加します。TypeScriptは、読み取り可能な標準ベースのJavaScriptにコンパイルされます。[playground](https://www.typescriptlang.org/play/)で試したり、[ブログ](https://blogs.msdn.microsoft.com/typescript)や[Twitterアカウント](https://twitter.com/typescript)最新情報を入手してください。

[コミュニティページ](https://www.typescriptlang.org/community/)でTypeScriptのユーザーを見つけてください。

## インストール

最新の安定バージョンの場合：

```bash
npm install -g typescript
```

ナイトリービルドの場合：

```bash
npm install -g typescript@next
```

## コントリビュート

TypeScriptに[コントリビュート](https://github.com/microsoft/TypeScript/blob/master/CONTRIBUTING.md)する方法はたくさんあります。
* [バグを送信](https://github.com/microsoft/TypeScript/issues)し、チェックイン時に修正を確認するのに役立ててください。
* [ソースコードの変更](https://github.com/microsoft/TypeScript/pulls)を確認。
* [StackOverflow](https://stackoverflow.com/questions/tagged/typescript)で他のTypeScriptユーザーや開発者と交流。
* [TypeScriptコミュニティDiscord](https://discord.gg/typescript)で互いに助け合う。
* Twitterの[#typescript](https://twitter.com/search?q=%23TypeScript)ディスカッションに参加。
* [バグ修正にコントリビュート](https://github.com/microsoft/TypeScript/blob/master/CONTRIBUTING.md)。
* アーカイブされた言語仕様([docx](https://github.com/microsoft/TypeScript/blob/master/doc/TypeScript%20Language%20Specification%20-%20ARCHIVED.docx?raw=true)、
[pdf](https://github.com/microsoft/TypeScript/blob/master/doc/TypeScript%20Language%20Specification%20-%20ARCHIVED.pdf?raw=true)、[md](https://github.com/microsoft/TypeScript/blob/master/doc/spec-ARCHIVED.md))を読む。

このプロジェクトは、[Microsoftオープンソースの行動規範](https://opensource.microsoft.com/codeofconduct/)を採用しています。詳細については、
[行動規範に関するFAQ](https://opensource.microsoft.com/codeofconduct/faq/)を参照するか、[opencode@microsoft.com](mailto:opencode@microsoft.com)
に質問やコメントをお問い合わせください。

## ドキュメント

*  [5分でTypeScript](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
*  [プログラミングハンドブック](https://www.typescriptlang.org/docs/handbook/intro.html)
*  [ホームページ](https://www.typescriptlang.org/)

## ビルド

TypeScriptコンパイラをビルドするには、[Git](https://git-scm.com/downloads)と[Node.js](https://nodejs.org/)がインストールされていることを確認してください。

リポジトリのコピーをクローンします：

```bash
git clone https://github.com/microsoft/TypeScript.git
```

TypeScriptディレクトリに移動します：

```bash
cd TypeScript
```

[Gulp](https://gulpjs.com/)ツールと、開発の依存関係をインストールします：

```bash
npm install -g gulp
npm ci
```

次のいずれかを使用して、ビルドとテストを行います:

```
gulp local             # コンパイラをbuilt/localにビルドする。
gulp clean             # ビルドされたコンパイラを削除します。
gulp LKG               # 最後の既知の商品をビルド済みのものと交換します。
                       # ビルドされたコンパイラが安定状態に達したときに実行されるブートストラップステップ。
gulp tests             # ビルドされたコンパイラを使用してテストインフラストラクチャをビルドします。
gulp runtests          # ビルドされたコンパイラとテストインフラストラクチャを使用してテストを実行します。
                       # 使用する特定のスイートランナーをオーバーライドしたり、このコマンドのテストを指定することができます。
                       # 特定のテストには --tests=<testPath> を使用し、特定のスイートには --runner=<runnerName> を使用します。
                       # 有効なランナーには、適合性、コンパイラー、フォースラッシュ、プロジェクト、ユーザー、およびdockerが含まれます。
                       # userおよびdockerランナーは、拡張テストスイートランナーです。ユーザーランナーは、tests/cases/user ディレクトリの
                       # ディスク上で動作し、dockerランナーはコンテナー内で動作します。
                       # dockerランナーを機能させるには、システムパスにdocker実行可能ファイルを含める必要があります。
gulp runtests-parallel # runtestと同様ですが、複数のスレッドに分割されます。デフォルトでは、システムコア数と同じ数のスレッドを使用します。
                       # これを調整するには、 --workers=<number> を使用します。
gulp baseline-accept   # ベースラインテストの結果がgulp runtestsから取得された結果に置き換えられます。
gulp lint              # TypeScriptソースでeslintを実行します。
gulp help              # 上記のコマンドのリストを表示します。
```


## 使用法

```bash
node built/local/tsc.js hello.ts
```


## ロードマップ

計画されている機能と今後の方向性の詳細については、[ロードマップ](https://github.com/microsoft/TypeScript/wiki/Roadmap)を参照してください。

---
[オリジナル](https://github.com/microsoft/TypeScript/blob/master/README.md)
