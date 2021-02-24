# <a href='https://www.meteor.com'><img src='https://user-images.githubusercontent.com/841294/26841702-0902bbee-4af3-11e7-9805-0618da66a246.png' height='60' alt='Meteor'></a>

[![TravisCI Status](https://travis-ci.org/meteor/meteor.svg?branch=devel)](https://travis-ci.org/meteor/meteor)
[![CircleCI Status](https://circleci.com/gh/meteor/meteor/tree/devel.svg?style=shield&circle-token=c2d3c041506bd493ef3795ffa4448684cfce97b8)](https://circleci.com/gh/meteor/meteor/tree/devel)

Meteorは、最新のWebアプリケーションを構築するための非常にシンプルな環境です。

Meteorを使用すると、アプリを作成できます：

* 人気のあるオープンソースライブラリを選択し
* HTMLではなくネットワーク経由でデータを送信する
* モダンなJavaScript

入門チュートリアルをお試しください：
 * [React](https://react-tutorial.meteor.com) - 新
 * [Blaze](https://www.meteor.com/tutorials/blaze/creating-an-app)
 * [Angular](https://www.meteor.com/tutorials/angular/creating-an-app)
 * [Vue](https://www.meteor.com/tutorials/vue/creating-an-app)
 * [Svelte](https://www.meteor.com/tutorials/svelte/creating-an-app)

次に、 [ガイド](https://guide.meteor.com) と [ドキュメント](https://docs.meteor.com/) をお読み下さい。

## クイックスタート

Windowsの場合、インストーラーはhttps://www.meteor.com/installにあります。

Linux/macOSの場合では、次の行を使用します：

```bash
curl https://install.meteor.com/ | sh
```

プロジェクトの作成：

```bash
meteor create try-meteor
```

実行：

```bash
cd try-meteor
meteor
```

## 開発者向けリソース

Meteorを使ってアプリケーションをビルドしますか？

* Galaxyホスティングにデプロイ： https://www.meteor.com/hosting
* アナウンスリスト： https://www.meteor.com/でサインアップ
* ディスカッションフォーラム： https://forums.meteor.com/
* この [招待リンク](https://join.slack.com/t/meteor-community/shared_invite/enQtODA0NTU2Nzk5MTA3LWY5NGMxMWRjZDgzYWMyMTEyYTQ3MTcwZmU2YjM5MTY3MjJkZjQ0NWRjOGZlYmIxZjFlYTA5Mjg4OTk3ODRiOTc) をクリックし、MeteorコミュニティSlackに参加して下さい。


Meteorの支援やコントリビュートに興味がありますか？これらのリソースが役立ちます：

* [Core development guide](DEVELOPMENT.md)
* [Contribution guidelines](CONTRIBUTING.md)
* [Feature requests](https://github.com/meteor/meteor-feature-requests/)
* [Issue tracker](https://github.com/meteor/meteor/issues)

## Meteorのアンインストール

短いランチャーシェルスクリプトとは別に、Meteorは自分自身をホームディレクトリ内にインストールします。
Meteorをアンインストールするには、次のコマンドを実行します：

```bash
rm -rf ~/.meteor/
sudo rm /usr/local/bin/meteor
```

Windowsでは、コントロールパネルからアンインストーラーを実行するだけです。

---
[オリジナル](https://github.com/meteor/meteor/blob/devel/README.md)
