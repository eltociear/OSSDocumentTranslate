# Deno

[![Build Status - Cirrus][]][Build status] [![Twitter handle][]][Twitter badge]

<img align="right" src=docs/images/deno3.png height="150px">

DenoはV8を使用し、Rustでビルドされた _シンプル_ で _モダン_ かつ _セキュア_ な **JavaScript** と **TypeScript** ランタイムです。

### 特徴

- デフォルトで保護。明示的に有効にしない限り、ファイルやネットワーク、または環境へのアクセスはなし。
- TypeScriptを追加設定なしにサポート。
- 単一の実行可能ファイルを生成。
- 依存関係インスペクター (deno info) やコードフォーマッターの様な組み込みユーティリティ。
- [Deno](https://deno.land/std/) での動作が保証されているレビュー済の標準モジュールのセット。

### インストール

Shell (Mac, Linux)：

```sh
curl -fsSL https://deno.land/x/install/install.sh | sh
```

PowerShell (Windows)：

```powershell
iwr https://deno.land/x/install/install.ps1 -useb | iex
```

[Homebrew](https://formulae.brew.sh/formula/deno) (Mac)：

```sh
brew install deno
```

[Chocolatey](https://chocolatey.org/packages/deno) (Windows)：

```powershell
choco install deno
```

[Cargo](https://crates.io/crates/deno) を使用したソースからのビルド及びインストール：

```sh
cargo install deno
```

その他のオプションについては [deno_install](https://github.com/denoland/deno_install/blob/master/README.md) と [releases](https://github.com/denoland/deno/releases) を御覧下さい。

### はじめに

簡単なプログラムを実行してみて下さい：

```sh
deno run https://deno.land/std/examples/welcome.ts
```

又は、より複雑なもの：

```ts
import { serve } from "https://deno.land/std/http/server.ts";
const s = serve({ port: 8000 });
console.log("http://localhost:8000/");
for await (const req of s) {
  req.respond({ body: "Hello World\n" });
}
```

[manual](https://deno.land/manual) にて、より詳細な紹介や例、または環境設定を見つけることができます。

それより更に詳細な情報はランタイム [documentation](https://doc.deno.land) にあります。

### コントリビュート

あなたの助けに感謝します！

コントリビュートするには私達の [guidelines](https://github.com/denoland/deno/blob/master/docs/contributing/style_guide.md) を御覧下さい。

[Build Status - Cirrus]: https://github.com/denoland/deno/workflows/ci/badge.svg?branch=master&event=push
[Build status]: https://github.com/denoland/deno/actions
[Twitter badge]: https://twitter.com/intent/follow?screen_name=deno_land
[Twitter handle]: https://img.shields.io/twitter/follow/deno_land.svg?style=social&label=Follow

---
[オリジナル](https://github.com/denoland/deno/blob/master/README.md)
