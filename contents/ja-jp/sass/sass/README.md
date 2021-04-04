<h1><img width="200px" alt="Sass" src="https://rawgit.com/sass/sass-site/master/source/assets/img/logos/logo.svg" /></h1>

[![@SassCSS on Twitter](https://img.shields.io/twitter/follow/SassCSS?label=%40SassCSS&style=social)](https://twitter.com/SassCSS)
&nbsp;&nbsp;
[![stackoverflow](https://img.shields.io/stackexchange/stackoverflow/t/sass?label=Sass%20questions&logo=stackoverflow&style=social)](https://stackoverflow.com/questions/tagged/sass)
&nbsp;&nbsp;
[![Gitter](https://img.shields.io/gitter/room/sass/sass?label=chat&logo=gitter&style=social)](https://gitter.im/sass/sass?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

**SassはCSSを再び楽しくします**。SassはCSSの拡張であり、ネストされたルール、変数、ミックスイン、セレクターの継承などを追加します。
コマンドラインツールまたはビルドシステムのプラグインを使用して、適切にフォーマットされた標準のCSSに変換されます。

```scss
$font-stack: Helvetica, sans-serif;
$primary-color: #333;

body {
  font: 100% $font-stack;
  color: $primary-color;
}

@mixin border-radius($radius) {
  -webkit-border-radius: $radius;
     -moz-border-radius: $radius;
      -ms-border-radius: $radius;
          border-radius: $radius;
}

nav {
  ul {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  li { @include border-radius(10px); }

  a {
    display: block;
    padding: 6px 12px;
    text-decoration: none;
  }
}
```

## Sassのインストール

Sassは、オペレーティングシステムのパッケージを[GitHubから][]ダウンロードし、[`PATH`に追加][PATH]することで、
Windows、Mac、またはLinuxにインストールできます。それだけです。
外部の依存関係はなく、インストールする必要のあるものは他にありません。

[GitHubから]: https://github.com/sass/dart-sass/releases
[PATH]: https://katiek2.github.io/path-doc/

Node.jsを使用している場合は、[npm][]を使用してSassをインストールすることもできます。

[npm]: https://www.npmjs.com/

```
npm install -g sass
```

**しかし、注意してください。** これによりSassの純粋なJavaScript実装がインストールされ、
ここにリストされている他のオプションよりも実行速度が多少遅くなります。
ただし、インターフェイスは同じであるため、もう少し速度が必要な場合は、後で別の実装に簡単に交換できます！

Sassをインストールするその他の方法については、[SassのWebサイト](https://sass-lang.com/install)を参照してください。

Sassをインストールしたら、`sass`実行可能ファイルを実行してコンパイルし
`.sass`や `.scss`ファイルを`.css`ファイルに変換できます。例えば：

```
sass source/stylesheets/index.scss build/stylesheets/index.css
```

## Sassを学ぶ

Sassを学ぶ方法のガイドについては、[SassのWebサイト](https://sass-lang.com/guide)をチェックしてください！

## このリポジトリ

このリポジトリはSassの実装ではありません。それらは
[`sass/dart-sass`][]と[`sass/libsass`][]にあり、ここには代わりに、次のものが含まれます：

[`sass/dart-sass`]: https://github.com/sass/dart-sass
[`sass/libsass`]: https://github.com/sass/libsass

* [`spec/`][]、言語機能の仕様が含まれています。
* [`proposal/`][]、言語の変更に関する進行中の提案が含まれています。
* [`accepted/`][]、受け入れられ、実装されているか、実装中の提案が含まれています。

[`spec/`]: https://github.com/sass/sass/tree/master/spec
[`proposal/`]: https://github.com/sass/sass/tree/master/proposal
[`accepted/`]: https://github.com/sass/sass/tree/master/accepted

これにはSassの完全な仕様が含まれていないことに注意してください。代わりに、機能仕様は、新しい機能が設計されているとき、
または実装者が何かがどのように機能するかについてさらに明確にする必要があるときに、必要に応じて作成されます。
これは、`spec/`のspecの多くが問題の機能のごく一部しかカバーしていないことを意味します。

### バージョン管理ポリシー

このリポジトリの提案はバージョン管理されており、時間の経過に伴う変更の追跡と古いバージョンの参照が容易になります。
すべてのバージョンには、`proposal.<name>.draft-<version>`の形式のGitタグがあります。
変更のバッチごとに新しいバージョンを作成する必要があります。

すべてのバージョンにはメジャーバージョンがあり、マイナーバージョンもある場合があります (`<major>.<minor>`で表示)。
マイナーバージョンは、提案の意図されたセマンティクスに影響を与えない変更のためにインクリメントする必要があります。
それ以外の場合は、メジャーバージョンをインクリメントする必要があります。

---
[オリジナル](https://github.com/sass/sass/blob/master/README.md)
