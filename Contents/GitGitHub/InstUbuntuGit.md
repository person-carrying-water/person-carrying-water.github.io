---
layout: default
title: ":octopus: Git、GitHub"
description: ":cat: gitインストール(Ubuntu)"
date: "2026/01/15"
lastmod: "2026/01/15"
---

## 0. はじめに
LinuxのOSのUbuntuにgitをインストールする手順です。

<br />

## 1. 最新版のgitをリポジトリに登録する  
`apt list git`や`apt show git`などでバージョンを確認するとバージョンの低いものがリポジトリに登録されている。
### 1-1. 最新版のgitをリポジトリに登録する  
最新版のgitをリポジトリに追加するには**Personal Package Archive(PPA)を使用します。  

```
$ sudo apt-add-repository ppa:git-core/ppa
```

### 1-2. パッケージ情報を更新する  
```
$ sudo apt update
```

<br />

## 2. gitをインストールする 
### 2-1. gitをインストールする  

```
$ sudo apt install git
```

***

