# D3: データドリブンドキュメント

<a href="https://d3js.org"><img src="https://d3js.org/logo.svg" align="left" hspace="10" vspace="6"></a>

**D3** (または **D3.js**) web標準を使用してデータを視覚化するためのJavaScriptライブラリです。D3は、SVGやCanvas、HTMLを使用してデータに命を吹き込むのに役立ちます。D3は、強力な視覚化と対話の手法をDOM操作へのデータドリブンアプローチと組み合わせ、最新のブラウザの全機能と、データに適したビジュアルインターフェイスを自由に設計できるようにします。

## リソース

* [Introduction](https://observablehq.com/@d3/learn-d3)
* [API Reference](https://github.com/d3/d3/blob/master/API.md)
* [Releases](https://github.com/d3/d3/releases)
* [Examples](https://observablehq.com/@d3/gallery)
* [Wiki](https://github.com/d3/d3/wiki)

## インストール

npmを使用する場合は、 `npm install d3` です。それ以外の場合は、 [latest release](https://github.com/d3/d3/releases/latest) をダウンロードして下さい。リリースされたバンドルは匿名AMD、CommonJS、そして普通な環境をサポートします。 [d3js.org](https://d3js.org)、 [CDNJS](https://cdnjs.com/libraries/d3)、 または [unpkg](https://unpkg.com/d3/) から直接ロードすることができます。例えば：

```html
<script src="https://d3js.org/d3.v6.js"></script>
```

圧縮版の場合：

```html
<script src="https://d3js.org/d3.v6.min.js"></script>
```

スタンドアロンのD3マイクロライブラリを使用することもできます。例えば、 [d3-selection](https://github.com/d3/d3-selection) ：

```html
<script src="https://d3js.org/d3-selection.v2.js"></script>
```

D3は [ES2015 modules](http://www.2ality.com/2014/09/es6-modules-final.html) を使用して記述されています。 [custom bundle using Rollup](https://bl.ocks.org/mbostock/bb09af4c39c79cffcde4) 、Webpackもしくはお好みのバンドラーを作成します。D3をES2015アプリケーションにインポートするには、特定のD3モジュールから特定のシンボルをインポートします：

```js
import {scaleLinear} from "d3-scale";
```

または、全てを名前空間 (ここでは `d3`) にインポートします：

```js
import * as d3 from "d3";
```

Nodeでは：

```js
const d3 = require("d3");
```

[Object.assign](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign) を使用して、個々のモジュールを要求し、それらを `d3` オブジェクトに結合することもできます：

```js
const d3 = Object.assign({}, require("d3-format"), require("d3-geo"), require("d3-geo-projection"));
```

---
[オリジナル](https://github.com/d3/d3/blob/master/README.md)
