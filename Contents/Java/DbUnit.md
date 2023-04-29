---
layout: default
title: ":page_with_curl: Oracle Java"
description: ":heavy_check_mark: データベーステストツール(DbUnit)"
date: "2023/04/15"
lastmod: "2023/04/15"
---

## 0. はじめに  
JUnitなどの単体テストツールがあれば、データベースへアクセスするテストを行うことができますがDBUnitを使うと  
比較的簡単にできるようなので使い方を書いていきます。  
また、テストデータをXMLファイルやエクセルファイル、CSVファイル形式で用意できるので都合のよいものを選べます。

<br />

## 1. 事前準備  
MavenまたはGradleを使いダウンロードするか、以下をMavenRepositoryで個別にダウンロードしてクラスパスへ追加してください。  
**dbunit-x.x.x.jar**  
**checker-qual-x.x.x.jar**  
**slf4j-api-x.x.x.jar**  

#### Oracleデータベースを使用する場合の追加  
**ojdbc8-x.x.x.x.jar**  
**ons-x.x.x.x.jar**  
**oraclepki-x.x.x.x.jar**  
**osdt-cert-x.x.x.x.jar**  
**simplefan-x.x.x.x.jar**  

#### PostgreSQLデータベースを使用する場合の追加  
**postgresql-x.x.x.jar**  

#### slf4jによる追加ライブラリ  
`slf4j-api-x.x.x.jar`は、追加で以下のいずれかが必要です。  
このライブラリが無いとエラーが表示されます。  
[Slf4J-apiを使用する](Slf4jApi)  

**slf4j-simple-x.x.x.jar**
**slf4j-nop-x.x.x.jar**  
**slf4j-reload4j.jar**  
**slf4j-jdk14.jarまたはlogback-classic.jar**  

※x.x.xまたはx.xはVersion番号が入り適応なものを入手してください。  

<br />

## 2. データベース接続  

準備中  

___
