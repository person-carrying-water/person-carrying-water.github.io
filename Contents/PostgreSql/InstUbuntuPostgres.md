---
layout: default
title: ":package: PostgreSQL、pgAdmin"
description: ":inbox_tray: PostgreSQLインストール(Ubuntu)"
date: "2026/01/22"
lastmod: "2026/01/22"
---

## 0. はじめに  
ubuntu24.04のリポジトリでは、postgresql16になっており最新の18ではないのでリポジトリを追加し最新版をインストールすることにします。  

<br />

## 1. 最新版のPostgreSQLリポジトリを追加する  
最新版をリポジトリに追加するため以下を入力します。  
```
$ sudo apt install -y postgresql-common
```

```
$ sudo /usr/share/postgresql-common/pgdg/apt.postgresql.org.sh
```

リポジトリ追加されたので`apt list postgresql-18`や`apt show postgresql`で確認。  

<br />

## 2. PostgreSQLをインストールする  
以下でPostgreSQLをインストール。  
```
$ sudo apt install postgresql-18
```

以下で、インストールされているかバージョン確認  
```
$ psql --version
```

以下で、PostgreSQLが起動しているか確認  
```
$ systemctl status postgresql
```

`Active: active(exited)`になっていれば起動中で`q`でsystemctlを終了できます。  

<br />

## 3. postgresのパスワード設定  
以下で、**postgres**ユーザーのパスワードを変更できます。  
```
$ sudo -U postgres psql
postgres=# ALTER ROLE postgres WITH PASSWORD '(設定するパスワード)';
ALTER ROLE
postgres=# exit;
```

___
