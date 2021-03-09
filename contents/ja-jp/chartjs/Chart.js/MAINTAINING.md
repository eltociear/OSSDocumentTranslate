# メンテナンス

## リリースプロセス

Chart.jsは、[Travis CI](https://travis-ci.org/)によってライブラリ[リリース](https://github.com/chartjs/Chart.js/releases)を自動化します。

### 新バージョンのリリース

1. `release-drafter`ツールによってドラフトされたリリースのリリースバージョンを[GitHub](https://github.com/chartjs/Chart.js/releases/new)で更新
2. リリースを公開
3. [GitHub Actions](https://github.com/chartjs/Chart.js/actions?query=workflow%3A%22Node.js+Package%22)のビルドプロセスに従う

このタグを作成すると、新しいビルドがトリガーされます：

* `Chart.js.zip`パッケージが生成され、distファイルと例が含まれます
* `dist/*.js`と`Chart.js.zip`はGitHubリリースに添付されています(ダウンロード)
* 新しいnpmパッケージが[npmjs](https://www.npmjs.com/package/chart.js)で公開されています

最後に、[cdnjs](https://cdnjs.com/libraries/Chart.js)はnpmリリースから自動的に更新されます。

### 参考文献

* [GitHub Actionリリース](https://github.com/chartjs/Chart.js/pull/7891)
* [dist/* ファイル](https://github.com/chartjs/Chart.js/issues/3033)
* [cdnjs npm自動アップデート](https://github.com/cdnjs/cdnjs/pull/8401)

---
[オリジナル](https://github.com/chartjs/Chart.js/blob/master/MAINTAINING.md)
