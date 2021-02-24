<p align="center">
  <a href="https://yarnpkg.com/">
    <img alt="Yarn" src="https://github.com/yarnpkg/assets/blob/master/yarn-kitten-full.png?raw=true" width="546">
  </a>
</p>

<p align="center">
  高速で信頼性が高く、安全な依存関係管理。
</p>

<p align="center">
  <a href="https://circleci.com/gh/yarnpkg/yarn"><img alt="Circle Status" src="https://circleci.com/gh/yarnpkg/yarn.svg?style=shield&circle-token=5f0a78473b0f440afb218bf2b82323cc6b3cb43f"></a>
  <a href="https://ci.appveyor.com/project/kittens/yarn/branch/master"><img alt="Appveyor Status" src="https://ci.appveyor.com/api/projects/status/0xdv8chwe2kmk463?svg=true"></a>
  <a href="https://dev.azure.com/yarnpkg/yarn/_build"><img alt="Azure Pipelines status" src="https://dev.azure.com/yarnpkg/yarn/_apis/build/status/Yarn%20Acceptance%20Tests"></a>
  <a href="https://discord.gg/yarnpkg"><img alt="Discord Chat" src="https://img.shields.io/discord/226791405589233664.svg"></a>
  <a href="http://commitizen.github.io/cz-cli/"><img alt="Commitizen friendly" src="https://img.shields.io/badge/commitizen-friendly-brightgreen.svg"></a>
</p>

---

**高速：** Yarnはダウンロードしたすべてのパッケージをキャッシュするため、同じパッケージを再度ダウンロードする必要はありません。また、リソース使用率を最大化するために、ほぼすべてを同時に実行します。これは、インストールがさらに高速になることを意味します。

**頼もしい：** Yarnは、インストール操作に詳細で簡潔なロックファイル形式と決定論的アルゴリズムを使用して、あるシステムで機能するインストールが別のシステムでもまったく同じように機能することを保証できます。

**セキュア：** Yarnはチェックサムを使用して、コードが実行される前に、インストールされているすべてのパッケージの整合性を検証します。

## 特徴

* **オフラインモード。** 以前にパッケージをインストールしたことがある場合は、インターネット接続せずに再インストールできます。
* **決定論的。** インストールの順序に関係なく、同じ依存関係がどのマシンにもまったく同じ方法でインストールされます。
* **ネットワークパフォーマンス。** Yarnは、ネットワークの使用率を最大化するために、リクエストを効率的にキューに入れ、リクエストウォーターフォールを回避します。
* **ネットワークの回復力。** 単一の要求が失敗しても、インストール全体が失敗することはありません。リクエストは失敗すると自動的に再試行されます。
* **フラットモード。** Yarnは、依存関係の不一致バージョンを単一バージョンに解決して、重複の作成を回避します。
* **より多くの絵文字。** 🐈

## Yarnのインストール

Yarnのインストール方法の詳細については、私達のWebサイトの [インストールガイド](https://yarnpkg.com/en/docs/install) をお読み下さい。

## Yarnの使用

Yarnの使用方法の詳細についでは、私達のWebサイトの [使用ガイド](https://yarnpkg.com/en/docs/usage) をお読み下さい。

## Yarnへのコントリビュート

どんなに大きくても小さくても、コントリビュートはいつでも歓迎します。実質的な機能リクエストは、 [RFC](https://github.com/yarnpkg/rfcs) として提案する必要があります。コントリビュートする前に [行動規範](CODE_OF_CONDUCT.md) をお読み下さい。

[Contributing](https://yarnpkg.com/org/contributing/) を参照して下さい。

## 先行技術

優れた先行技術がなければ、Yarnは存在しなかったでしょう。Yarnは次のプロジェクトに触発されました：

 - [Bundler](https://github.com/bundler/bundler)
 - [Cargo](https://github.com/rust-lang/cargo)
 - [npm](https://github.com/npm/cli)

## クレジット

npmパッケージ名を寄付してくれた [Sam Holmes](https://github.com/samholmes) に感謝いたします！

---
[オリジナル](https://github.com/yarnpkg/yarn/blob/master/README.md)
