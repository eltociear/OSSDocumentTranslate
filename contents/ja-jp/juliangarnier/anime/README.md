<h1 align="center">
  <a href="https://animejs.com"><img src="./documentation/assets/img/animejs-v3-header-animation.gif" width="250"/></a>
  <br>
  anime.js
</h1>

<h4 align="center">JavaScriptアニメーションエンジン | <a href="https://animejs.com" target="_blank">animejs.com</a></h4>

<p align="center">
  <a href="https://www.npmjs.com/package/animejs" rel="nofollow"><img src="https://camo.githubusercontent.com/011820ee25bf1d3ddaf635d869903b98eccaeae7/68747470733a2f2f696d672e736869656c64732e696f2f6e706d2f762f616e696d656a732e7376673f7374796c653d666c61742d737175617265" alt="npm version" data-canonical-src="https://img.shields.io/npm/v/animejs.svg?style=flat-square" style="max-width:100%;"></a>
  <a href="https://www.npmjs.com/package/animejs" rel="nofollow"><img src="https://camo.githubusercontent.com/3e9b69d51aee25fad784a3097676696096621d47/68747470733a2f2f696d672e736869656c64732e696f2f6e706d2f646d2f616e696d656a732e7376673f7374796c653d666c61742d737175617265" alt="npm downloads" data-canonical-src="https://img.shields.io/npm/dm/animejs.svg?style=flat-square" style="max-width:100%;"></a>
</p>

<blockquote align="center">
  <em>Anime.js</em> (<code>/ˈæn.ə.meɪ/</code>) は、シンプルでありながら強力なAPIを備えた軽量のJavaScriptアニメーションライブラリです。<br>
  これは、CSSプロパティ、SVG、DOM属性、およびJavaScriptオブジェクトで機能します。
</blockquote>

<p align="center">
  <a href="#getting-started">はじめに</a>&nbsp;|&nbsp;<a href="#documentation">ドキュメント</a>&nbsp;|&nbsp;<a href="#demos-and-examples">デモと例</a>&nbsp;|&nbsp;<a href="#browser-support">ブラウザのサポート</a>
</p>

## 入門

### ダウンロード

npm経由

```bash
$ npm install animejs --save
```

または手動[ダウンロード](https://github.com/juliangarnier/anime/archive/master.zip)。

### 使用法

#### ES6モジュール

```javascript
import anime from 'animejs/lib/anime.es.js';
```

#### CommonJS

```javascript
const anime = require('animejs');
```

#### ファイルインクルード

HTMLで`anime.min.js`をリンクします：

```html
<script src="anime.min.js"></script>
```

### Hello world

```javascript
anime({
  targets: 'div',
  translateX: 250,
  rotate: '1turn',
  backgroundColor: '#FFF',
  duration: 800
});
```

## [ドキュメント](https://animejs.com/documentation/)

* [ターゲット](https://animejs.com/documentation/#cssSelector)
* [プロパティ](https://animejs.com/documentation/#cssProperties)
* [プロパティパラメータ](https://animejs.com/documentation/#duration)
* [アニメーションパラメータ](https://animejs.com/documentation/#direction)
* [値](https://animejs.com/documentation/#unitlessValue)
* [キーフレーム](https://animejs.com/documentation/#animationKeyframes)
* [スタガリング](https://animejs.com/documentation/#staggeringBasics)
* [タイムライン](https://animejs.com/documentation/#timelineBasics)
* [コントロール](https://animejs.com/documentation/#playPause)
* [コールバックと約束](https://animejs.com/documentation/#update)
* [SVGアニメーション](https://animejs.com/documentation/#motionPath)
* [イージング機能](https://animejs.com/documentation/#linearEasing)
* [ヘルパー](https://animejs.com/documentation/#remove)

## [デモと例](http://codepen.io/collection/b392d3a52d6abf5b8d9fda4e4cab61ab/)

* [CodePenのデモと例](http://codepen.io/collection/b392d3a52d6abf5b8d9fda4e4cab61ab/)
* [juliangarnier.com](http://juliangarnier.com)
* [animejs.com](https://animejs.com)
* [@tobiasahlin](https://twitter.com/tobiasahlin)による[文字の移動](http://tobiasahlin.com/moving-letters/)
* [@crnacura](https://twitter.com/crnacura)による[勾配地形アニメーション](https://tympanus.net/Development/GradientTopographyAnimation/)
* [@crnacura](https://twitter.com/crnacura)による[有機的な形状のアニメーション](https://tympanus.net/Development/OrganicShapeAnimations/)
* [@lmgonzalves](https://twitter.com/lmgonzalves)による[ピーススライダー](https://tympanus.net/Tutorials/PiecesSlider/)
* [スタガリングアニメーション](https://codepen.io/juliangarnier/pen/4fe31bbe8579a256e828cd4d48c86182?editors=0100)
* [イージングアニメーション](https://codepen.io/juliangarnier/pen/444ed909fd5de38e3a77cc6e95fc1884)
* [球体アニメーション](https://codepen.io/juliangarnier/pen/b3bb8ca599ad0f9d00dd044e56cbdea5?editors=0010)
* [レイヤードアニメーション](https://codepen.io/juliangarnier/pen/6ca836535cbea42157d1b8d56d00be84?editors=0010)
* [anime.jsロゴアニメーション](https://codepen.io/juliangarnier/pen/d43e8ec355c30871cbe775193255d6f6?editors=0010)


## ブラウザのサポート

| Chrome | Safari | IE / Edge | Firefox | Opera |
| --- | --- | --- | --- | --- |
| 24+ | 8+ | 11+ | 32+ | 15+ |

## <a href="https://animejs.com"><img src="./documentation/assets/img/animejs-v3-logo-animation.gif" width="150" alt="anime-js-v3-logo"/></a>

[ウェブサイト](https://animejs.com/) | [ドキュメント](https://animejs.com/documentation/) | [デモと例](http://codepen.io/collection/b392d3a52d6abf5b8d9fda4e4cab61ab/) | [MITライセンス](LICENSE.md) | © 2019 [Julian Garnier](http://juliangarnier.com).

---
[オリジナル](https://github.com/juliangarnier/anime/blob/master/README.md)
