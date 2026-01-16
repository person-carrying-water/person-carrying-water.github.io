---
layout: default
title: ":package: Microsoft Visual Studio Code"
description: ":inbox_tray: Microsoft Visual Studio Codeインストール(Ubuntu)"
date: "2026/01/15"
lastmod: "2026/01/16"
---

## 0. はじめに  
Ubuntuはインストール方法がいくつかあるがsnapを使ったインストールでは日本語入力ができずやむを得ず公式サイトから.debファイルをダウンロードして行う方法で行います。   
Ubuntu24.04とVS Code1.108.1の動作環境で日本語入力不可でした。  

ちなみに、snapでのインストールは以下のコマンドでインストールできます。至って簡単。  
```
$ sudo snap install code --classic
[sudo] password for <ユーザー名>: パスワード入力(表示されないが構わず入力しEnter)
code 585eba7c from Visual Studio Code (vscode✓) installed
```

アンインストールは、以下のコマンドで削除できます。  
すでに、snap版をインストールしている場合など。  
```
$ sudo snap remove code
[sudo] password for <ユーザー名>: パスワード入力(表示されないが構わず入力しEnter)
code removed (snap data snapshot saved)
```

`snap list`や`snap list code`などで一覧から削除されているか確認。  

<br />

## 1. Microsoft Visual Studio Codeをダウンロードする  
公式サイトから.debパッケージを~Downloadsフォルダにダウンロードする。  
wgetやcurlを使ってインストールすることもできるがURLが都度変わる可能性もあるので割愛する。  

<br />

## 2. Microsoft Visual Studio Codeをインストールする  
### 2-1. ダウンロードフォルダに移動する  
ターミナルを開きます。  
ダウンロードフォルダに移動するためcdコマンドを入力します。  

```
~$ cd Downloads
~Downloads$
```

### 2-2. ダウンロードされたファイルでインストールする  
`sudo apt install ./<インストールファイル名>.deb`コマンドでインストールします。

```
~/Downloads$ sudo apt install ./code_1.108.1-1768404234_amd64.deb
[sudo] password for <ユーザー名>: パスワード入力(表示されないが構わず入力しEnter)
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
Note, selecting 'code' instead of './code_1.108.1-1768404234_amd64.deb'
The following NEW packages will be installed:
  code
0 upgraded, 1 newly installed, 0 to remove and 0 not upgraded.
Need to get 0 B/114 MB of archives.
After this operation, 469 MB of additional disk space will be used.
Get:1 /home/<ユーザー名>/Downloads/code_1.108.1-1768404234_amd64.deb code amd64 1.108.1-1768404234 [114 MB]
Preconfiguring packages ...
Selecting previously unselected package code.
(Reading database ... 243148 files and directories currently installed.)
Preparing to unpack .../code_1.108.1-1768404234_amd64.deb ...
Unpacking code (1.108.1-1768404234) ...
Setting up code (1.108.1-1768404234) ...
Processing triggers for gnome-menus (3.36.0-1.1ubuntu3) ...
Processing triggers for shared-mime-info (2.4-4) ...
Processing triggers for desktop-file-utils (0.27-2build1) ...
N: Download is performed unsandboxed as root as file '/home/<ユーザー名>/Downloads/code_1.108.1-1768404234_amd64.deb' couldn't be accessed by user '_apt'. - pkgAcquire::Run (13: Permission denied)
```

### 2-3. インストールされているか確認する  
apt list codeやapt show codeなどでインストールされているか確認できる。
```
~/Downloads$ apt list code
Listing... Done
code/now 1.108.1-1768404234 amd64 [installed,local]
```

**将来的にアンインストールしたい場合**  
Visual Studio Codeをアンインストールしたい場合は以下のコマンドで削除できる。　　
```
$ apt remove code
```

___
