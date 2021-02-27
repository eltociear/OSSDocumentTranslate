# Intro.js v3

[![Build Status](https://travis-ci.org/usablica/intro.js.svg?branch=master)](https://travis-ci.org/usablica/intro.js)
[![](https://data.jsdelivr.com/v1/package/npm/intro.js/badge)](https://www.jsdelivr.com/package/npm/intro.js)
[![npm](https://img.shields.io/npm/dm/intro.js)](https://www.jsdelivr.com/package/npm/intro.js)

> 軽量でユーザーフレンドリーなオンボーディングツアーライブラリ

## 入手先
Intro.jsのローカルコピーは次の場所から入手できます：

**1)** このGitHubリポジトリからは、 ```git clone https://github.com/usablica/intro.js.git``` を使用

**2)** boweでは ```bower install intro.js --save``` を使用

**3)** npmでは ```npm install intro.js --save``` を使用

**4)** CDNからのダウンロードは ([1](http://www.jsdelivr.com/projects/intro.js) と [2](https://cdnjs.com/libraries/intro.js))

## 使用法
Intro.jsは、次の3つの簡単な手順でサイトに追加できます：

**1)** ページに `intro.js` と `introjs.css` (または本番用に縮小されたバージョン) を含めます。 右横書き言語サポートには `introjs-rtl.min.css` を使用してください。

> CDNでホストされるファイルは、 [jsDelivr](http://www.jsdelivr.com/projects/intro.js) (Show Moreをクリック) と [cdnjs](https://cdnjs.com/libraries/intro.js) で入手できます。

**2)** HTML要素に `data-intro` と `data-step` を追加します。ヒントを追加するには、 `data-hint` 属性を使用する必要があります。

例えば：

```html
<a href='http://google.com/' data-intro='Hello step one!'></a>
````

[ここ](https://introjs.com/docs/intro/attributes/)で全ての属性を参照してください。

**3)** このJavaScript関数を呼び出し：
```javascript
introJs().start();
````

必要に応じて、1つのパラメータを `introJs` 関数に渡して、プレゼンテーションセクションを制限します。

**例えば** `introJs(".introduction-farm").start();` は `class='introduction-farm'` を持つ要素に対してのみ導入を実行します。

<p align="center"><img src="https://raw.githubusercontent.com/usablica/intro.js/gh-pages/img/introjs-demo.png"></p>

## ドキュメント

[ドキュメント](http://introjs.com/docs)にアクセスして下さい。

## 使用：

Intro.jsには、さまざまな目的のための多くのラッパーがあります。詳細については、[ドキュメント](http://introjs.com/docs)にアクセスして下さい。

## ビルド

先ず `nodejs` と `npm` をインストールし、最初に次のコマンドを実行する必要があります： `npm install` ですべての依存関係をインストールします。

これで、次のコマンドを実行して、すべての静的リソースを縮小できます。

    npm run build

## コントリビューター ✨

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tr>
    <td align="center"><a href="http://afshinm.name"><img src="https://avatars3.githubusercontent.com/u/314326?v=4" width="100px;" alt=""/><br /><sub><b>Afshin Mehrabani</b></sub></a><br /><a href="https://github.com/usablica/intro.js/commits?author=afshinm" title="Code">💻</a> <a href="https://github.com/usablica/intro.js/commits?author=afshinm" title="Documentation">📖</a></td>
    <td align="center"><a href="https://bozdoz.com"><img src="https://avatars0.githubusercontent.com/u/1410985?v=4" width="100px;" alt=""/><br /><sub><b>bozdoz</b></sub></a><br /><a href="https://github.com/usablica/intro.js/commits?author=bozdoz" title="Code">💻</a> <a href="https://github.com/usablica/intro.js/commits?author=bozdoz" title="Documentation">📖</a></td>
  </tr>
</table>

<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

## サポート／議論
- [Stackoverflow](http://stackoverflow.com/questions/tagged/intro.js)

## ライセンス

### 商用ライセンス

Intro.jsを商用アプリケーション、テーマ、またはプラグインに使用する場合は、商用ライセンスが適切なライセンスです。このオプションを使用すると、ソースコードは独占的に保持されます。[introjs.com](http://introjs.com/#commercial)で商用ライセンスを購入します

### オープンソースライセンス

GNU AGPLv3

---
[オリジナル](https://github.com/usablica/intro.js/blob/master/README.md)
