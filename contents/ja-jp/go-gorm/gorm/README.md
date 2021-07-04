# GORM

Go言語用の素晴らしいORMライブラリは、開発者に優しいことを目指しています。

[![go report card](https://goreportcard.com/badge/github.com/go-gorm/gorm "go report card")](https://goreportcard.com/report/github.com/go-gorm/gorm)
[![test status](https://github.com/go-gorm/gorm/workflows/tests/badge.svg?branch=master "test status")](https://github.com/go-gorm/gorm/actions)
[![Join the chat at https://gitter.im/jinzhu/gorm](https://img.shields.io/gitter/room/jinzhu/gorm.svg)](https://gitter.im/jinzhu/gorm?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Open Collective Backer](https://opencollective.com/gorm/tiers/backer/badge.svg?label=backer&color=brightgreen "Open Collective Backer")](https://opencollective.com/gorm)
[![Open Collective Sponsor](https://opencollective.com/gorm/tiers/sponsor/badge.svg?label=sponsor&color=brightgreen "Open Collective Sponsor")](https://opencollective.com/gorm)
[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT)
[![Go.Dev reference](https://img.shields.io/badge/go.dev-reference-blue?logo=go&logoColor=white)](https://pkg.go.dev/gorm.io/gorm?tab=doc)

## 概要

* フル機能のORM
* アソシエーション（Has One, Has Many, Belongs To, Many To Many, Polymorphism, Single-table inheritance）
* フック（前/後/保存/更新/削除/検索）
* `Preload`、`Joins`を使用した積極的な読み込み
* トランザクション、ネストされたトランザクション、保存ポイント、保存されたポイントへのロールバック
* コンテキスト、プリペアドステートメントモード、ドライランモード
* バッチ挿入、FindInBatches、マップへの検索
* SQL Builder、Upsert、Locking、Optimizer / Index / Comment Hints、NamedArg、Search / Update / Create with SQL Expr
* 複合プライマリキー
* 自動マイグレーション
* ロガー
* 拡張可能で柔軟なプラグインAPI：データベースリゾルバー（複数のデータベース、読み取り/書き込み分割）/プロメテウス…
* すべての機能にはテストが付属しています
* 開発者に優しい

## 入門

* GORMガイド [https://gorm.io](https://gorm.io)

## コントリビュート

[より良いGORMになるための手伝いをすることができます、できることをチェックしてください](https://gorm.io/contribute.html)

## ライセンス

© Jinzhu, 2013~time.Now

[MITライセンス](https://github.com/go-gorm/gorm/blob/master/License)の下でリリース

---
[オリジナル](https://github.com/go-gorm/gorm/blob/master/README.md)
