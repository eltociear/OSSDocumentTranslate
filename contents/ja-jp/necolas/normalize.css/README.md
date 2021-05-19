# normalize.css

<a href="https://github.com/necolas/normalize.css"><img
  src="https://necolas.github.io/normalize.css/logo.svg" alt="Normalize Logo"
  width="80" height="80" align="right"></a>

> CSSリセットのモダンな代替手段

[![npm][npm-image]][npm-url] [![license][license-image]][license-url]
[![changelog][changelog-image]][changelog-url]
[![gitter][gitter-image]][gitter-url]


**NPM**

```sh
npm install --save normalize.css
```

**CDN**

https://yarnpkg.com/en/package/normalize.css を参照してください

**ダウンロード**

https://necolas.github.io/normalize.css/latest/normalize.css を参照してください


## 何をするためのもの？

* 多くのCSSリセットとは異なり、便利なデフォルトを保持します。
* さまざまな要素のスタイルを正規化します。
* バグと一般的なブラウザの不整合を修正します。
* 微妙な変更で使いやすさが向上します。
* 詳細なコメントを使用して、コードの機能を説明します。


## ブラウザのサポート

* Chrome
* Edge
* Firefox ESR以降
* Internet Explorer 10以降
* Safari 8+
* Opera


## 拡張された詳細と既知の問題

normalize.cssの難解な部分の追加の詳細と説明。

#### `pre, code, kbd, samp`

`font-family: monospace, monospace`ハックは、フォーマット済みテキストのフォントサイズの継承とスケーリングを修正します。
`monospace`の複製は意図的なものです。[ソース](https://en.wikipedia.org/wiki/User:Davidgothberg/Test59)。

#### `sub, sup`

通常、 `sub`または`sup`を使用すると、すべてのブラウザのテキストの行ボックスの高さに影響します。[ソース](https://gist.github.com/413930)。

#### `select`

デフォルトでは、OSX上のChromeとOSX上のSafariでは、borderプロパティが設定されていない限り、`select`のスタイルが非常に制限されています。
`optgroup`要素のデフォルトのフォントの太さは、OSXのChromeおよびOSXのSafariでは安全に変更できません。

#### `[type="checkbox"]`

Firefoxの実装はボックスのサイズ、パディング、または幅を尊重しないため、チェックボックスとラジオ入力のスタイルを設定しないことをお勧めします。

#### `[type="number"]`

数値入力に適用される特定のフォントサイズ値により、デクリメントボタンのカーソルスタイルが`default`から`text`に変更されます。

#### `[type="search"]`

デフォルトでは、検索入力は完全にスタイル設定できません。 OSX/iOSのChromeとSafariでは、`font`、`padding`、`border`、
または`background`を制御することはできません。Windows上のChromeとSafariでは、`border`を適切に制御できません。`border-width`が適用されますが、
その境界線の外側の1pxの境界線の色（制御できません）のみが表示されます。`-webkit-appearance：textfield`を適用すると、
検索入力の利点を失うことなくこれらの問題に対処できます（過去の検索を表示するなど）。

## コントリビュート

関係者全員が寄付プロセスを簡単かつ効果的に行うために、[コントリビューションガイド](CONTRIBUTING.md)をお読みください。


[changelog-image]: https://img.shields.io/badge/changelog-md-blue.svg?style=flat-square
[changelog-url]: CHANGELOG.md
[license-image]: https://img.shields.io/npm/l/normalize.css.svg?style=flat-square
[license-url]: LICENSE.md
[npm-image]: https://img.shields.io/npm/v/normalize.css.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/normalize.css
[gitter-image]: https://img.shields.io/badge/chat-gitter-blue.svg?style=flat-square
[gitter-url]: https://gitter.im/necolas/normalize.css

---
[オリジナル](https://github.com/necolas/normalize.css/blob/master/README.md)
