# Cargo

Cargoは、Rustプロジェクトの依存関係をダウンロードし、プロジェクトをコンパイルします。

詳細については https://doc.rust-lang.org/cargo/ をご覧下さい。

## コードステータス

[![Build Status](https://dev.azure.com/rust-lang/cargo/_apis/build/status/rust-lang.cargo?branchName=auto-cargo)](https://dev.azure.com/rust-lang/cargo/_build?definitionId=18)

コードドキュメント： https://docs.rs/cargo/

## Cargoのインストール

CargoはデフォルトでRustとともに配布されるため、 `rustc` がローカルにインストールされている場合は、おそらく `cargo` もローカルにインストールされています。

## ソースからのコンパイル

Cargoをビルドするには、次のツールとパッケージが必要です：

* `git`
* `curl` (Unixの場合)
* `pkg-config` (Unixでは、 `libssl` ヘッダー/ライブラリーを見つけるために使用されます)
* OpenSSL headers (Unixの場合のみ、これはubuntuの `libssl-dev` パッケージです)
* `cargo` 及び、 `rustc`

まず、このリポジトリをチェックアウトしてください

```
git clone https://github.com/rust-lang/cargo
cd cargo
```

`cargo` がすでにインストールされているので、簡単に実行できます：

```
cargo build --release
```

## Cargoへの新しいサブコマンドの追加

Cargoは、Cargo自体を変更することなく、新しいサブコマンドで拡張できるように設計されています。
詳細およびコミュニティで開発された既知のサブコマンドのリストについては、 [the Wiki page][third-party-subcommands] を参照してください。

[third-party-subcommands]: https://github.com/rust-lang/cargo/wiki/Third-party-cargo-subcommands


## リリース

CargoのリリースはRustのリリースと一致します。
高レベルのリリースノートは、 [Rust's release notes][rel] の一部として入手できます。
詳細なリリースノートは、このリポジトリの [CHANGELOG.md] にあります。

[rel]: https://github.com/rust-lang/rust/blob/master/RELEASES.md
[CHANGELOG.md]: CHANGELOG.md

## 問題の報告

バグを見つけましたか？私たちはそれについて知りたいです！

GitHub [issue tracker][issues] で全ての問題を報告して下さい。

[issues]: https://github.com/rust-lang/cargo/issues

## コントリビュート

Cargoへのコントリビュートの完全な紹介については、 **[Cargo Contributor Guide]** を参照して下さい。

[Cargo Contributor Guide]: https://rust-lang.github.io/cargo/contrib/

## ライセンス

Cargoは主にMITライセンスとApacheライセンス（バージョン2.0）の両方の条件で配布されます。

詳細については [LICENSE-APACHE](LICENSE-APACHE) 及び、 [LICENSE-MIT](LICENSE-MIT) を参照して下さい。

### サードパーティソフトウェア

このプロダクトには、OpenSSL Toolkit (https://www.openssl.org/) で使用するために
OpenSSL Projectによって開発されたソフトウェアが含まれています。

バイナリ形式では、このプロダクトには、 [upstream repository][1] から取得できるリンク例外を除いて
GNU General Public Licenseバージョン2の条件の下でライセンスされているソフトウェアが含まれています。

詳細については [LICENSE-THIRD-PARTY](LICENSE-THIRD-PARTY) を参照して下さい。

[1]: https://github.com/libgit2/libgit2

---
[オリジナル](https://github.com/rust-lang/cargo/blob/master/README.md)
