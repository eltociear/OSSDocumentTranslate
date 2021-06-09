# Smarty 3テンプレートエンジン
[smarty.net](https://www.smarty.net/)

[![Build Status](https://travis-ci.org/smarty-php/smarty.svg?branch=master)](https://travis-ci.org/smarty-php/smarty)

## ドキュメント

ドキュメントについては、
[www.smarty.net/docs/en/](https://www.smarty.net/docs/en/)を参照してください

## 要件

SmartyはPHP 5.2からPHP 7.4で実行できます。

## 配布リポジトリ

> Smarty 3.1.28は、ランタイムテンプレートの継承を導入します

> Smarty 3.1の機能に対する最近の拡張については、NEW_FEATURESおよびINHERITANCE_RELEASE_NOTESファイルをお読みください

Smartyバージョン 3.1.11以降がgithubにあり、Composerでインストールできます。


"smarty/smarty"パッケージはlibs/....  サブフォルダーから開始されます。

Smarty 3.1の最新の安定版を入手するには、次を使用します：

```json
"require": {
    "smarty/smarty": "~3.1"
}
```

composer.jsonファイル内。

trunkバージョンを取得するには、次を使用します：

```json
"require": {
    "smarty/smarty": "~3.1@dev"
}
```

特定のバージョンの場合は、次のようなものを使用します：

```json
"require": {
    "smarty/smarty": "3.1.19"
}
```

PHPUnitテストは、次のような対応するcomposerエントリによってインストールできます：

```json
"require": {
    "smarty/smarty-phpunit": "3.1.19"
}
```

lexer/parserジェネレーターにも同様のことが当てはまります。

```json
"require": {
    "smarty/smarty-lexer": "3.1.19"
}
```

または、次を使用できます：

```json
"require": {
    "smarty/smarty-dev": "3.1.19"
}
```

3つのパッケージすべてをインストールするためのラッパーです。

Composerは、Smarty2バージョン 2.6.24から2.6.30でも使用できます。

---
[オリジナル](https://github.com/smarty-php/smarty/blob/master/README.md)
