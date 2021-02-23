[![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/npm/cli/Node%20CI/latest)](https://github.com/npm/cli/actions?query=workflow%3A%22Node+CI%22+branch%3Alatest) [![Coveralls github branch](https://img.shields.io/coveralls/github/npm/cli/latest)](https://coveralls.io/github/npm/cli?branch=latest)

# npm - JavaScriptパッケージマネージャー

### 要件

* このプログラムの実行には、 [**Node.js** `v10`](https://nodejs.org/en/download/) 以降がインストールされている必要があります

### インストール

**`npm`** は、デフォルトで [**`node`**](https://nodejs.org/) 及びほとんどのサードパーティーディストリビューションにバンドルされています。公式にサポートされているダウンロード／ディストリビューションは、以下にあります： [nodejs.org/en/download](https://nodejs.org/en/download)

#### 直接ダウンロード

カスタムの `install.sh` スクリプトを使用して、 [**npmjs**.com](https://npmjs.com/) から直接 **`npm`** をダウンロードしてインストールできます：

```bash
curl -qL https://www.npmjs.com/install.sh | sh
```

#### Nodeバージョン管理

**`node`** 及び／または **`npm`** の複数バージョンを管理する場合は、次のような"Nodeバージョン管理"の使用を検討して下さい：

* [**`nvm`**](https://github.com/nvm-sh/nvm)
* [**`nvs`**](https://github.com/jasongin/nvs)
* [**`nave`**](https://github.com/isaacs/nave)
* [**`n`**](https://github.com/tj/n)
* [**`volta`**](https://github.com/volta-cli/volta)
* [**`nodenv`**](https://github.com/nodenv/nodenv)

### 使用法

```bash
npm <command>
```

### リンク＆リソース

* [**Documentation**](https://docs.npmjs.com/) - **npm** の全ての公式ドキュメントとハウツー
    * 注： `npm help-search <query>` を使用してローカルでドキュメントを検索することもできます
* [**Bug Tracker**](https://github.com/npm/cli/issues) - CLIに対してバグ検索、または送信を行う
* [**Roadmap**](https://github.com/npm/roadmap) - 公開ロードマップに従って追跡及びフォロー
* [**Feedback**](https://github.com/npm/feedback) - npmレジストリ、Webサイト、CLIに関するアイディアとディスカッションにコントリビュート
* [**RFCs**](https://github.com/npm/rfcs) - npm CLIのAPI／デザインに関するアイディアと仕様にコントリビュート
* [**Service Status**](https://status.npmjs.org/) - 現在のステータスを監視し、Webサイトとレジストリのインシデントレポートを確認
* [**Project Status**](https://npm.github.io/statusboard/) - メンテナンスされている全てのOSSプロジェクトの状態を1つのビューで確認
* [**Events Calendar**](https://calendar.google.com/calendar/u/0/embed?src=npmjs.com_oonluqt8oftrt0vmgrfbg6q6go@group.calendar.google.com) - RFC呼び出し、リリース、ミートアップ、会議を追跡
* [**Support**](https://www.npmjs.com/support) - **npm** [website](https://npmjs.com) もしくは [registry](https://registry.npmjs.org) で問題が発生しましたか？チケットを [こちら](https://www.npmjs.com/support) に提出

### 謝辞

* `npm` は、デフォルトで [https://registry.npmjs.org](https://registry.npmjs.org) の **npm Public Registry** を使用するように設定されています；このレジストリの使用には、 [https://npmjs.com/policies/terms](https://npmjs.com/policies/terms) で入手できる **利用規約** が適用されます
* 他の互換性あるレジストリを使用するように `npm` を設定できます。サードパーティーのレジストリの設定について詳しくは [こちら](https://docs.npmjs.com/cli/v7/using-npm/registry) をご覧下さい。

### ブランディングに関するFAQ

#### "npm"？"NPM"または"Npm"？

**`npm`** は、通常全ての大文字表記のファイルを除いて大文字にしないで下さい (例 `man` ページのタイトル) 。

#### "npm"は"Node Package Manager"の頭字語ですか？

一般に信じられている事とは正反対に **`npm`** は、"Node Package Manager"の頭字語 **ではありません** ； これは **"npm is not an acronym"（訳：npmは頭字語ではありません）** の再帰的な略語です ("ninaa"の場合は、頭字語になります) 。 **`npm`** の全身は **"pm"** という名前のbashユーティリティで、これは **"pkgmakeinst"** の短縮名でした - これは様々なプラットフォームに様々なものをインストールするbash関数です。 **`npm`** が頭字語と見なされているとすれば、それは"node pm"、または"new pm"となる可能性があります。

---
[オリジナル](https://github.com/npm/cli/blob/latest/README.md)
