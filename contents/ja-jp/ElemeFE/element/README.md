<p align="center">
  <img src="https://cdn.rawgit.com/ElemeFE/element/dev/element_logo.svg">
</p>

<p align="center">
  <a href="https://travis-ci.org/ElemeFE/element">
    <img src="https://travis-ci.org/ElemeFE/element.svg?branch=master">
  </a>
  <a href="https://coveralls.io/github/ElemeFE/element?branch=master">
    <img src="https://coveralls.io/repos/github/ElemeFE/element/badge.svg?branch=master">
  </a>
  <a href="https://cdnjs.com/libraries/element-ui">
    <img src="https://img.shields.io/cdnjs/v/element-ui.svg">
  </a>
  <a href="https://www.npmjs.org/package/element-ui">
    <img src="https://img.shields.io/npm/v/element-ui.svg">
  </a>
  <a href="https://npmcharts.com/compare/element-ui?minimal=true">
    <img src="http://img.shields.io/npm/dm/element-ui.svg">
  </a>
  <br>
  <a href="http://img.badgesize.io/https://unpkg.com/element-ui/lib/index.js?compression=gzip&label=gzip%20size:%20JS">
    <img src="http://img.badgesize.io/https://unpkg.com/element-ui/lib/index.js?compression=gzip&label=gzip%20size:%20JS">
  </a>
  <a href="http://img.badgesize.io/https://unpkg.com/element-ui/lib/theme-chalk/index.css?compression=gzip&label=gzip%20size:%20CSS">
    <img src="http://img.badgesize.io/https://unpkg.com/element-ui/lib/theme-chalk/index.css?compression=gzip&label=gzip%20size:%20CSS">
  </a>
  <a href="#backers">
    <img src="https://opencollective.com/element/backers/badge.svg">
  </a>
  <a href="#sponsors">
    <img src="https://opencollective.com/element/sponsors/badge.svg">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg">
  </a>
</p>

> Web用のVue.js2.0UIツールキット。

ElementはVue2.xのままになります

Vue 3.0の場合、同じチームの[Element Plus](https://github.com/element-plus/element-plus)を使用することをお勧めします

## リンク
- ホームページとドキュメント
  - [海外のユーザー](http://element.eleme.io/#/en-US)
  - [中国のユーザー](http://element-cn.eleme.io/#/zh-CN)
  - [スペインのユーザー](http://element.eleme.io/#/es)
  - [フランスのユーザー](http://element.eleme.io/#/fr-FR)
- [awesome-element](https://github.com/ElementUI/awesome-element)
- [FAQ](./FAQ.md)
- [Vue.js 3.0移行](https://github.com/element-plus/element-plus)
- [テーマのカスタマイズ](http://element.eleme.io/#/en-US/component/custom-theme)
- [オンラインでテーマをプレビューして生成](https://elementui.github.io/theme-chalk-preview)
- [React用のElement](https://github.com/elemefe/element-react)
- [Angular用のElement](https://github.com/ElemeFE/element-angular)
- [Atomヘルパー](https://github.com/ElemeFE/element-helper)
- [Visual Studio Codeヘルパー](https://github.com/ElemeFE/vscode-element-helper)
- スターターキット
  - [element-starter](https://github.com/ElementUI/element-starter)
  - [element-in-laravel-starter](https://github.com/ElementUI/element-in-laravel-starter)
- [Design resources](https://github.com/ElementUI/Resources)
- Gitter
  - [海外のユーザー](https://gitter.im/element-en/Lobby)
  - [中国のユーザー](https://gitter.im/ElemeFE/element)

## インストール
```shell
npm install element-ui -S
```

## クイックスタート
``` javascript
import Vue from 'vue'
import Element from 'element-ui'

Vue.use(Element)

// または
import {
  Select,
  Button
  // ...
} from 'element-ui'

Vue.component(Select.name, Select)
Vue.component(Button.name, Button)
```
詳細については、ドキュメントの[クイックスタート](http://element.eleme.io/#/en-US/component/quickstart)を参照してください。

## ブラウザサポート
最新のブラウザとInternetExplorer10以降。

## 開発
Elementを使用するだけの場合は、この部分をスキップしてください。

Elementへの貢献に関心のある方は、このプロジェクトの実行方法について、コントリビューションガイド([中文](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.zh-CN.md) | [英語](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.en-US.md) | [スペイン語](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.es.md) | [フランス語](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.fr-FR.md))を参照してください。

## 変更ログ
各リリースの詳細な変更は、[リリースノート](https://github.com/ElemeFE/element/releases)に記載されています。

## FAQ
[よくある質問](https://github.com/ElemeFE/element/blob/master/FAQ.md)をいくつか集めました。問題を報告する前に、FAQに問題に対する回答があるかどうかを検索してください。

## コントリビュート
プルリクエストを行う前に、必ずコントリビューションガイド([中文](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.zh-CN.md) | [英語](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.en-US.md) | [スペイン語](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.es.md) | [フランス語](https://github.com/ElemeFE/element/blob/master/.github/CONTRIBUTING.fr-FR.md))をお読みください。

## スペシャルサンクス
英語のドキュメントはSwiftGG翻訳チームによって提供されました：
- [raychenfj](https://github.com/raychenfj)
- [kevin](http://thekevin.cn/)
- [曾小涛](https://github.com/zengxiaotao)
- [湾仔王二](https://github.com/wanzaiwanger)
- [BlooDLine](http://www.ibloodline.com/)
- [陈铭嘉](https://chenmingjia.github.io/)
- [千叶知风](http://mpc6.com/)
- [梁杰](http://numbbbbb.com)
- [Changing](https://github.com/sunzhuo11)
- [mmoaay](https://github.com/mmoaay)

スペイン語のドキュメントは、これらのコミュニティ開発者によって利用可能になりました：
- [adavie1](https://github.com/adavie1)
- [carmencitaqiu](https://github.com/carmencitaqiu)
- [coderdiaz](https://github.com/coderdiaz)
- [fedegar33](https://github.com/fedegar33)
- [Gonzalo2310](https://github.com/Gonzalo2310)
- [lesterbx](https://github.com/lesterbx)
- [ProgramerGuy](https://github.com/ProgramerGuy)
- [SantiagoGdaR](https://github.com/SantiagoGdaR)
- [sigfriedCub1990](https://github.com/sigfriedCub1990)
- [thechosenjuan](https://github.com/thechosenjuan)

フランス語のドキュメントは、これらのコミュニティ開発者によって利用可能になりました：
- [smalesys](https://github.com/smalesys)
- [blombard](https://github.com/blombard)

## ディスカッショングループに参加する

[Dingtalk App](https://www.dingtalk.com/)を使用してQRコードをスキャンし、ディスカッショングループに参加します：

<img alt="Join Discusion Group" src="https://user-images.githubusercontent.com/17680888/93177882-0ae92d80-f766-11ea-870d-3fa2d7f06454.png" width="300">


## ライセンス
[MIT](LICENSE)

---
[オリジナル](https://github.com/ElemeFE/element/blob/dev/README.md)
