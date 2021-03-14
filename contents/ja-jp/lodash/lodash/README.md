# lodash

[Site](https://lodash.com/) |
[Docs](https://lodash.com/docs) |
[FP Guide](https://github.com/lodash/lodash/wiki/FP-Guide) |
[Contributing](https://github.com/lodash/lodash/blob/master/.github/CONTRIBUTING.md) |
[Wiki](https://github.com/lodash/lodash/wiki "Changelog, Roadmap, etc.") |
[Code of Conduct](https://code-of-conduct.openjsf.org) |
[Twitter](https://twitter.com/bestiejs) |
[Chat](https://gitter.im/lodash/lodash)

[Lodash](https://lodash.com/)ライブラリは[UMD](https://github.com/umdjs/umd)モジュールとしてエクスポートされます。

[lodash-cli](https://www.npmjs.com/package/lodash-cli)を使用して生成：
```shell
$ npm run build
$ lodash -o ./dist/lodash.js
$ lodash core -o ./dist/lodash.core.js
```

## ダウンロード

 * [Core build](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/core.js) ([~4 kB gzip圧縮](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/core.min.js))
 * [Full build](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/lodash.js) ([~24 kB gzip圧縮](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/lodash.min.js))
 * [CDN copies](https://www.jsdelivr.com/projects/lodash) [![jsDelivr Hits](https://data.jsdelivr.com/v1/package/npm/lodash/badge)](https://www.jsdelivr.com/package/npm/lodash)

Lodashは、[MIT license](https://raw.githubusercontent.com/lodash/lodash/4.17.10-npm/LICENSE)でリリースされ、最新の環境をサポートしています。<br>
[ビルドの違い](https://github.com/lodash/lodash/wiki/build-differences)を確認して、自分に合ったものを選択してください。

## インストール

ブラウザの場合：
```html
<script src="lodash.js"></script>
```

npmの場合：
```shell
$ npm i -g npm
$ npm i lodash
```
注： 5.0.0より前のnpmを使用している場合は、`--save`を追加して下さい

Node.jsの場合：
```js
// 完全なビルドをロードします。
var _ = require('lodash');
// コアビルドをロードします。
var _ = require('lodash/core');
// 不変の自動カリー化、イテレティファースト、データラストメソッドのFPビルドをロードします。
var fp = require('lodash/fp');

// 関数カテゴリをロードします。
var array = require('lodash/array');
var object = require('lodash/fp/object');

// より小さなbrowserify/rollup/webpackバンドルのための関数をチェリーピックします。
var at = require('lodash/at');
var curryN = require('lodash/fp/curryN');
```

ES6以下のバンドルサイズで書かれたLodashモジュールをお探しですか？[lodash-es](https://www.npmjs.com/package/lodash-es)をチェックしてください。

## なぜLodash？

Lodashは、配列の数値、オブジェクト、文字列などを操作する手間を省くことでJavaScriptを簡単にします。<br>
Lodashのモジュラーメソッドは次の場合に最適です：

 * 配列、オブジェクト、文字列の反復
 * 値の操作とテスト
 * 合成関数の作成

## モジュールフォーマット

Lodashは、[さまざまなビルド](https://lodash.com/custom-builds)およびモジュール形式で利用できます。

 * [lodash](https://www.npmjs.com/package/lodash) & [per method packages](https://www.npmjs.com/search?q=keywords:lodash-modularized)
 * [lodash-es](https://www.npmjs.com/package/lodash-es)、[babel-plugin-lodash](https://www.npmjs.com/package/babel-plugin-lodash)、および[lodash-webpack-plugin](https://www.npmjs.com/package/lodash-webpack-plugin)
 * [lodash/fp](https://github.com/lodash/lodash/tree/npm/fp)
 * [lodash-amd](https://www.npmjs.com/package/lodash-amd)

---
[オリジナル](https://github.com/lodash/lodash/blob/master/README.md)
