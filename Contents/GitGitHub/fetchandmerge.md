---
layout: default
title: ":octocat: Git、GitHub"
description: ":octocat: Git、GitHub他者の変更点を取り込む"
date: "2021/09/04"
lastmod: "2022/12/15"
---

## 0. はじめに
複数作業で他者の変更点を取り込む方法です。  

<br />

## 1. 空のローカルリポジトリに取り込 む  
まず、Github上にある他者が開発しているプログラムを自分の空のローカルリポジトリに取り込む方法です。  

### 1-1. git cloneを使う  

### 1-2. git pullを使う

### 1-3. git fetchとgit mergeを使う

<br />

## 2. git fetchで他者の変更点をローカルリポジトリに取り込む 
リモートリポジトリの変更点をローカルリポジトリに取り込みます。これを`fetch(フェチ)`と言います。   
`git fetch`を実行してみれば分かりますが取り込んでもmasterブランチやその派生のブランチのプログラムに変化はありません。  
これは、ローカルリポジトリに取り込んでいるのですが、実はもう1つorigin/masterブランチというブランチがリモートリポジトリと  
masterブランチの間にありそこへ変更点を取り込んでいます。  
では、masterブランチなどへ取り込むのはどうするかというとこの次に紹介する`git merge`というものに当たります。  
これは、次に紹介するとしてまずは`git fetch`の使い方について書いていきます。  

### 2-1. origin(リモート名)にあるすべてのブランチの変更点を取り込む  
`git fetch origin`と入力し「Enter」キーを押します。  
```
$ git fetch origin
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 4 (delta 2), reused 4 (delta 2), pack-reused 0
Unpacking objects: 100% (4/4), 952 bytes | 23.00 KiB/s, done.
From github.com:<githubアカウント名>/<リモートリポジトリ名>
 * branch            master     -> FETCH_HEAD
   e675b00..aab3ec8  master     -> origin/master
```

### 2-2. origin(リモート名)の特定のブランチのみの変更点を取り込む  
※masterブランチのみの変更点を取り込む  
```
$ git fetch origin master
```

### 2-3. 現在のブランチ(HEAD)の上流ブランチから変更点を取り込む  
```
$ git fetch
```

### 2-4.すべてのリモートの変更点を取り込む  
１つのリモートリポジトリだけでなくすべてのリモート設定しているリポジトリの変更点を取り込みます。  
```
$ git fetch --all
```

<br />

## 3. git mergeでmasterブランチなどへ取り込む  
`git fetch`でローカリポジトリの`origin/master`ブランチへ取り込まれたものから作業ブランチであるmasterブランチなどへ  
取り込みます。これを`merge(マージ)`と言います。  
これは、ローカルリポジトリで作業しているプログラムソースが実際に改変されます。  
ファイルの追加や削除がリモートリポジトリ側で行われていた場合も変更されます。  

### 3-1. masterブランチが変更されていないものをmerge
masterブランチから派生した作業ブランチをmasterブランチへマージする場合は、masterブランチの変更点をmasterブランチで  
コミットしただけの`Fast-Forward`なマージとなる。  
実際デフォルトでは、マージした履歴は残らず変更前のmasterブランチの先へコミット群が追加された形となる。  
マージ履歴すなわちマージコミットはマージする時にmasterブランチに変更があった場合に行われるがmasterブランチに変更が  
ない場合にもマージコミットを残せるようにすることができる。  
オプションに`--no-ff`を付ければ良い。  

```
$ git merge --no-ff master
```

また、毎回付ける場合には以下コマンドを実行してconfigに追加しておけばマージコミットを残せるようにできる。  
※リポジトリ毎に設定したいなら--globalを`--local`に変更して入力し「Enter」キーを押します。  
```
$ git config --global --add merge.ff false
$ git config --global --add pull.ff only
```

`--global`オプションならユーザーフォルダ直下の.gitconfigに、`--local`ならリポジトリにできる.gitフォルダ内のconfig  
ファイルに以下のように追加される。  

```
[merge]
    ff = false
[pull]
    ff = only
```



***
