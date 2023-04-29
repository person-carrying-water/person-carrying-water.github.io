---
layout: default
title: ":cloud: クラウド、Heroku"
description: ":cloud: Herokuコマンド"
date: "2019/02/20"
lastmod: "2022/01/20"
---

## 1. ログイン、ログアウト

### 1-1. ログイン

    $ heroku login --interactive
    heroku: Enter your login credentials
    Email: <herokuに登録したメールアドレスを入力>
    Password: <herokuに登録したパスワードを入力>
    Logged in as <メールアドレス>

\--interactiveを入れないと既定のブラウザが開きログイン画面が出る。  
heroku cli はデフォルトでブラウザが開くように設定してあるようだ。  

### 1-2. ログアウト

    $ heroku logout
    Logging out... done

<br />

## 2. Heroku CLIのバージョンを確認する

    $ heroku version
    heroku/7.59.2 win32-x64 node-v12.21.0

<br />

## 3. Heroku CLIのバージョンをアップする

Herokuのコマンドを発行していると以下の様な警告が表示される。  

```\#heroku
 »   Warning: heroku update available from 7.53.0 to 7.59.2.
```

Heroku CLIの最新版が出ていますが古いバージョンをお使いですという事でしょう。  

バージョンアップするには以下の様に実行します。  

    $ heroku update
    heroku: Updating CLI from 7.53.0 to 7.59.2... done
    heroku: Updating CLI... done

バージョンアップされましたのでバージョンを確認してみましょう。  

<br />

## 4. Herokuのスタックをアップグレードする  
アプリをデプロイした時など、スタックのバージョンが古いものを使っている場合に以下のようなメッセージが出ます。  

    This app is using the Heroku-18 stack, which is supported until April 30th, 2023.
    A newer stack is available: Heroku-20. To upgrade, see:
    https://devcenter.heroku.com/articles/upgrading-to-the-latest-stack

**日本語訳**  

> このアプリは、2023年4月30日までサポートされているHeroku-18スタックを使用しています。  
> 新しいスタックが利用可能です：Heroku-20。アップグレードするには、以下を参照してください。  
> https://devcenter.heroku.com/articles/upgrading-to-the-latest-stack  

[スタックのアップグレードについて](https://devcenter.heroku.com/ja/articles/upgrading-to-the-latest-stack)  
このページを参考に`heroku stack:set heroku-20 -a <アプリ名>`と入力しアップグレードします。  
※ただし、すでにアプリが稼働している場合は再デプロイするまで有効になりません。  

    $ heroku stack:set heroku-20 -a <アプリ名>
    Setting stack to heroku-20... done
    You will need to redeploy ⬢ <アプリ名> for the change to take effect.
    Run git push heroku main to trigger a new build on ⬢ <アプリ名>.

**日本語訳**  

> スタックをheroku-20に設定しています...完了  
> 変更を有効にするには、⬢<アプリ名>を再デプロイする必要があります。  
>  git push heroku mainを実行して、⬢アプリ名で新しいビルドをトリガーします。  

**デプロイ**  

    $ git push heroku master
    Enumerating objects: 21, done.
    Counting objects: 100% (21/21), done.
    Delta compression using up to 8 threads
    Compressing objects: 100% (7/7), done.
    Writing objects: 100% (11/11), 838 bytes | 838.00 KiB/s, done.
    Total 11 (delta 4), reused 0 (delta 0), pack-reused 0
    remote: Compressing source files... done.
    remote: Building source:
    remote:
    remote: -----> Building on the Heroku-20 stack
    remote: -----> Using buildpack: heroku/java
    remote: -----> Java app detected
    remote: -----> Installing JDK 17.0.1... done
    remote: -----> Installing Maven 3.6.2... done
    remote: -----> Executing Maven
    remote:        $ mvn -DskipTests clean dependency:list install
    remote:        [INFO] Scanning for projects...
    以下省略


* * *
