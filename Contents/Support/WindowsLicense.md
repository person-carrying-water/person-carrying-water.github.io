---
layout: default
title: ":newspaper: Microsoft Windows"
description: ":paperclip: Microsoft Windowsライセンス"
date: "2023/02/23"
lastmod: "2023/02/24"
---

## 1. WindowsクライアントOS向けライセンス  
Windows10やWindows11などのクライアントOSは、サーバー用途としての提供はライセンス的にNGとなる。  
例えば、SQL ServerやOracleなどのデータベースアプリをインストールしてクライアントからのデータベースアクセスはできない。  
これは、無料のExpress Editonであっても同様である。  
では、ファイル共有などもNGかというとそうではない。  
それがNGならファイル共有の機能は無いと思いますし、個人で使用している大多数の人もライセンス違反となってしまいます。  
Microsoftによると、ファイル共有、プリンタの共有、IIS(Webサーバー)などの用途で最大２０デバイスまでならサーバーのような提供・アクセスの仕方も可能のようです。  

※IISではなくApache Http ServerやTomcatなどではライセンス的にどうかは問い合わせる必要があるのでしょう。  
WebサーバーのMicrosoft製品に限定しているのがIISだけなのでこのように書かれているかもしれませんので。  

<br />

## 2. WindowsサーバーOS向けライセンス  
### 2-1. Windows Serverライセンス  
サーバー用ライセンスは、CPUのハード的な物理的個数と内部コア数に応じてライセンスが必要。  
また、クライアントからのアクセスは別途クライアントアクセスライセンス(CAL)を購入・取得しアクセスする必要がある。  
ユーザ数に応じてのユーザーライセンスとデバイス数に応じてのデバイスライセンスがあり用途に応じたライセンスを選ぶことができる。  

また、Windows Serverと同一ネットワークにあってもそのクライアントからのアクセスを制限してWindows Serverにアクセスできないのであれば、
CALを購入する必要はない。しかし、外部ネットワークであってもWindows Serverへアクセスできる状態であるならCALの購入が必要。  

### 2-2. Windows Server IoT 20xx for Storageライセンス  
NASなどのバンドルOEMとして配布されているOSで、基本ファイルサーバーとしての用途に限定されている。  
アプリケーションのインストールも基本的にはできない。  
SQL Server Express Editionなどの非エンタープライズデータベースであるなら、インストールしてデータベースサーバーとして使える。  
クライアント・アクセス・ライセンス(CAL)は必要は無い。  
Workgroup Editonでのアクセスは、50ユーザーに限定されている。  

※SQL Server以外の非エンタープライズ製品であるOracle Database Express Editonや無料のPostgresSQLはインストール可能かは問い合わせる必要が
あるのでしょう。Express Editionという所でOKを出しているのか無料・無償という所でOKを出しているのかMicrosoftの非エンタープライズに限定している
のかは分かりません。  

* * *
