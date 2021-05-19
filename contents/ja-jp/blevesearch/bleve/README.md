# ![bleve](docs/bleve.png) bleve

[![Tests](https://github.com/blevesearch/bleve/workflows/Tests/badge.svg?branch=master&event=push)](https://github.com/blevesearch/bleve/actions?query=workflow%3ATests+event%3Apush+branch%3Amaster)
[![Coverage Status](https://coveralls.io/repos/github/blevesearch/bleve/badge.svg?branch=master)](https://coveralls.io/github/blevesearch/bleve?branch=master)
[![GoDoc](https://godoc.org/github.com/blevesearch/bleve?status.svg)](https://godoc.org/github.com/blevesearch/bleve)
[![Join the chat at https://gitter.im/blevesearch/bleve](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/blevesearch/bleve?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![codebeat](https://codebeat.co/badges/38a7cbc9-9cf5-41c0-a315-0746178230f4)](https://codebeat.co/projects/github-com-blevesearch-bleve)
[![Go Report Card](https://goreportcard.com/badge/blevesearch/bleve)](https://goreportcard.com/report/blevesearch/bleve)
[![Sourcegraph](https://sourcegraph.com/github.com/blevesearch/bleve/-/badge.svg)](https://sourcegraph.com/github.com/blevesearch/bleve?badge)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

goのモダンテキストインデックス - [blevesearch.com](http://www.blevesearch.com/)

## 特徴

* goデータ構造（JSONを含む）にインデックスを付ける
* 強力な構成によってバックアップされたインテリジェントなデフォルト
* サポートされているフィールドタイプ：
    * テキスト、数値、日付
* サポートされているクエリタイプ：
    * 用語、フレーズ、一致、一致フレーズ、接頭辞
    * 接続詞、論理和、ブール値
    * 数値範囲、日付範囲
    * 人間による入力のための単純なクエリ[構文](http://www.blevesearch.com/docs/Query-String-Query/)
* tf-idfスコアリング
* 検索結果の一致の強調表示
* ファセットの集約をサポート：
    * 用語ファセット
    * 数値範囲ファセット
    * 日付範囲ファセット

## ディスカッション

[Googleグループ](https://groups.google.com/forum/#!forum/bleve)でbleveの使用法と開発について話し合う。

## インデックス作成

```go
message := struct{
	Id   string
	From string
	Body string
}{
	Id:   "example",
	From: "marty.schoch@gmail.com",
	Body: "bleve indexing is easy",
}

mapping := bleve.NewIndexMapping()
index, err := bleve.New("example.bleve", mapping)
if err != nil {
	panic(err)
}
index.Index(message.Id, message)
```

## クエリ

```go
index, _ := bleve.Open("example.bleve")
query := bleve.NewQueryStringQuery("bleve")
searchRequest := bleve.NewSearchRequest(query)
searchResult, _ := index.Search(searchRequest)
```

## ライセンス

Apache License Version 2.0

---
[オリジナル](https://github.com/blevesearch/bleve/blob/master/README.md)
