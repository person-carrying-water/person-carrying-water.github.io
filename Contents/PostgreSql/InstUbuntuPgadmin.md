---
layout: default
title: ":package: PostgreSQL、pgAdmin"
description: ":inbox_tray: pgAdminインストール(Ubuntu)"
date: "2026/01/22"
lastmod: "2026/01/22"
---

## 0. はじめに  
pgAdminの最新版のインストール手順です。  

<br />

## 1. 最新版のpgAdminインストールのための事前準備  
リポジトリの公開鍵をインストールします。  
```
$ scurl -fsS https://www.pgadmin.org/static/packages_pgadmin_org.pub | sudo gpg --dearmor -o /usr/share/keyrings/packages-pgadmin-org.gpg
```

リポジトリ構成ファイルを作成します。  

```
$ sudo sh -c 'echo "deb [signed-by=/usr/share/keyrings/packages-pgadmin-org.gpg] https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/$(lsb_release -cs) pgadmin4 main" > /etc/apt/sources.list.d/pgadmin4.list && apt update'
```

<br />

## 2. pgAdminをインストールする  
以下でPpgAdmin4をインストールします。  
```
$ sudo apt install pgadmin4
```

以下で、インストールされているか確認  
```
$ apt list pgadmin4
pgadmin4/pgadmin4,now 9.11 all [installed]
N: There are 8 additional versions. Please use the '-a' switch to see them.
```
または、  
```
$ apt show pgadmin4
package: pgadmin4
Version: 9.11
Priority: optional
Section: database
Maintainer: pgAdmin Development Team <pgadmin-hackers@postgresql.org>
Installed-Size: unknown
Depends: pgadmin4-server (= 9.11), pgadmin4-desktop (= 9.11), pgadmin4-web (= 9.11)
Download-Size: 668 B
APT-Manual-Installed: yes
APT-Sources: https://ftp.postgresql.org/pub/pgadmin/pgadmin4/apt/noble pgadmin4/main all Packages
Description: Installs all required components to run pgAdmin in desktop and web modes. pgAdmin is the most popular and feature rich Open Source administration and development platform for PostgreSQL, the most advanced Open Source database in the world.

N: There are 8 additional records. Please use the '-a' switch to see them.
```

**pgAdmin4を起動して使えるようにする。**  
`pgAdminを起動してサーバーの登録をする`
Serversを右クリックして登録→サーバーをクリック  
接続タブのホスト名にlocalhost、パスワードにpostgresのパスワードを入力し保存する。postgresユーザーでログインできる。

___
