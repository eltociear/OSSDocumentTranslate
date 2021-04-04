three.js
========

[![NPM Package][npm]][npm-url]
[![Build Size][build-size]][build-size-url]
[![NPM Downloads][npm-downloads]][npmtrends-url]
[![Language Grade][lgtm]][lgtm-url]

#### JavaScript 3D ライブラリ ####

使いやすく、軽量で、クロスブラウザの汎用3Dライブラリを作成することが目的です。現在のビルドにはWebGLレンダラーのみが含まれていますが、WebGPU（実験的）、SVG、CSS3Dレンダラーもサンプルで利用できます。

[例](https://threejs.org/examples/) &mdash;
[ドキュメント](https://threejs.org/docs/) &mdash;
[Wiki](https://github.com/mrdoob/three.js/wiki) &mdash;
[移行](https://github.com/mrdoob/three.js/wiki/Migration-Guide) &mdash;
[質問](http://stackoverflow.com/questions/tagged/three.js) &mdash;
[フォーラム](https://discourse.threejs.org/) &mdash;
[Slack](https://join.slack.com/t/threejs/shared_invite/enQtMzYxMzczODM2OTgxLTQ1YmY4YTQxOTFjNDAzYmQ4NjU2YzRhNzliY2RiNDEyYjU2MjhhODgyYWQ5Y2MyZTU3MWNkOGVmOGRhOTQzYTk) &mdash;
[Discord](https://discordapp.com/invite/HF4UdyF)

### 使用法 ###

このコードは、シーン、カメラ、およびジオメトリックキューブを作成し、キューブをシーンに追加します。次に、シーンとカメラの`WebGL`レンダラーを作成し、そのビューポートを`document.body`要素に追加します。最後に、カメラのシーン内の立方体をアニメーション化します。

```javascript
import * as THREE from './js/three.module.js';

let camera, scene, renderer;
let geometry, material, mesh;

init();

function init() {

	camera = new THREE.PerspectiveCamera( 70, window.innerWidth / window.innerHeight, 0.01, 10 );
	camera.position.z = 1;

	scene = new THREE.Scene();

	geometry = new THREE.BoxGeometry( 0.2, 0.2, 0.2 );
	material = new THREE.MeshNormalMaterial();

	mesh = new THREE.Mesh( geometry, material );
	scene.add( mesh );

	renderer = new THREE.WebGLRenderer( { antialias: true } );
	renderer.setSize( window.innerWidth, window.innerHeight );
	renderer.setAnimationLoop( animation );
	document.body.appendChild( renderer.domElement );

}

function animation( time ) {

	mesh.rotation.x = time / 2000;
	mesh.rotation.y = time / 1000;

	renderer.render( scene, camera );

}
```

すべてがうまくいった場合は、[こちら](https://jsfiddle.net/zdjankqw/)が表示されるはずです。

### このリポジトリをクローンする ###

リポジトリをすべての履歴で複製すると、最大2GBのダウンロードになります。履歴全体が必要ない場合は、`depth`パラメーターを使用してダウンロードサイズを大幅に減らすことができます。

```sh
git clone --depth=1 https://github.com/mrdoob/three.js.git
```

### 変更ログ ###

[リリース](https://github.com/mrdoob/three.js/releases)


[npm]: https://img.shields.io/npm/v/three
[npm-url]: https://www.npmjs.com/package/three
[build-size]: https://badgen.net/bundlephobia/minzip/three
[build-size-url]: https://bundlephobia.com/result?p=three
[npm-downloads]: https://img.shields.io/npm/dw/three
[npmtrends-url]: https://www.npmtrends.com/three
[lgtm]: https://img.shields.io/lgtm/alerts/github/mrdoob/three.js
[lgtm-url]: https://lgtm.com/projects/g/mrdoob/three.js/

---
[オリジナル](https://github.com/mrdoob/three.js/blob/dev/README.md)
