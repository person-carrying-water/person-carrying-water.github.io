---
layout: default
title: ":newspaper: オープンソースソフトウェアライセンス(OSS)"
description: ":page_with_curl: オープンソースソフトウェアライセンス(OSS)全般"
date: "2022/01/04"
lastmod: "2023/02/26"
---

## はじめに  


<br />

## ライセンス文の形式  
ライセンス全文の中には、著作権表示とライセンス本文と免責事項が含まれている。  
例えば、以下の三条項BSDライセンスで見てみます。  
その前に、オープンライセンスが適用されるのは`英語の原文`のみであり日本語訳ではライセンス効果が基本的には無い。  
ただし、日本語訳ライセンスを別途付与することは禁じられていません。  

```
Copyright (c) <YEAR>, <OWNER>
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:
* Redistributions of source code must retain the above copyright notice, 
  this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright notice, 
  this list of conditions and the following disclaimer in the documentation 
  and/or other materials provided with the distribution.
* Neither the name of the <organization> nor the names of its contributors 
  may be used to endorse or promote products derived from this software 
  without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

#### 1. 著作権表示  
まず以下の部分が`著作権表示`にあたる部分です。  
YEARには、**著作権が発生した年**、OWNERには**著作権保持者**を入れます。  

```
Copyright (c) <YEAR>, <OWNER>
All rights reserved.
```

#### 2. ライセンス本文  
次に以下の部分が`ライセンス本文`にあたる部分です。  

```
Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:
* Redistributions of source code must retain the above copyright notice, 
  this list of conditions and the following disclaimer.
* Redistributions in binary form must reproduce the above copyright notice, 
  this list of conditions and the following disclaimer in the documentation 
  and/or other materials provided with the distribution.
* Neither the name of the <organization> nor the names of its contributors 
  may be used to endorse or promote products derived from this software 
  without specific prior written permission.
```

#### 3. 免責事項(Disclaimer)
最後に以下の部分が`免責事項(Disclaimer)`にあたる部分です。  
責任に関する事が書いてある部分になります。
すべて大文字で書いてある場合が多いのが特徴です。  

<br />

## 2. ライセンスの種類  
### 2-1. コピーレフト型、非コピーレフト型  
まず、大きく分けてライセンスの種類はコピーレフト型と非コピーレフト型に分かれます。  
コピーレフト型のライセンスを施したものを使う時は、それを提供するときも同じライセンスに従って同じライセンスとして提供しなければなりません。  
例えば、GPLライセンスのものをそのまま提供する場合やそれを含めたもので提供する場合はGPLライセンスとして提供しなければなりません。
逆に、非コピーレフト型のライセンスは、同じライセンスとして提供する必要はありません。  
ただし、著作権表示などを載せる必要がある場合があります。  

よく、GPLライセンスなどはソースコードの開示が必要と言われていますがソースコードを開示していれば良いわけではなくGPLライセンスとして提供しなければなりません。  
ソースコードの開示をしていればそれだけで済むという話ではなくコピーレフトとして同じライセンス形態で提供して派生させていく必要があるということです。  
技術的なものを自分・自社で閉じ込めて置きたいのであれば採用されませんが、技術をオープン・アウトプットして互いに高め合うこと・自分の技術が間違っているかを知るという
ためにも繋がりますのでデメリットばかりでは無いのかもしれません。 

コピーレフト型を少し緩めた準コピーレフト型に位置するものも存在します。  
例えば、GPLを緩めたLGPLライセンス、Java言語向けにクラスパス例外を設けているライセンス形態もあります。  

### 2-2. 動的リンク、静的リンク  
よく、ライセンスで動的リンク、静的リンクとして使う場合という言葉が出てきますが動的リンクは実行時に呼び出してライブラリを使う方法で
静的リンクはコンパイル時に一緒にコンパイルしてしまうものを指すようです。  

プログラムソースの先頭でimportして使うのはどちらになるかはプログラム言語の種類やコンパイルなのかインタプリタなのかにもよるようです。  

ちなみにJavaは、jarファイルをクラスパスに追加しプログラムの先頭でimport文を追加して使うのは静的リンクとして使っていることになるようです。  
[LGPLとJava](https://www.gnu.org/licenses/lgpl-java.ja.html)  

### 2-3. GPLの疑問  
クラスパス例外もない純粋なGPLライセンスは、動的リンク、静的リンクに関わらずオリジナルのソースコードを含むすべての開示が必要ですが
インターネットで利用する人すべてに公開しなければならないとか誤解のあるのも現状のようです。  
また、社内システムで使う場合はどうなの？という疑問もあります。  

まず、社内システムを自社内のエンジニアが開発することにおいて、その上でGPLライセンスのものを扱う時はGPLライセンスに従いますがプログラムソースを
開示する相手はいませんので事実上技術の流出はありません。  
もちろん、LGPLライセンスやクラスパス例外GPLもソースの開示は当然ありません。  

次に、インターネットの不特定多数の人間が扱うシステムの場合、これは利用する不特定多数に開示することは対象外になるようです。  
ただし、AGPLライセンスの場合は免除されず開示する必要があるようですが詳しくは分かりません。  

よって、社内で使うシステム、不特定多数が扱うWebシステムに関わらず、システムを委託した顧客とシステム開発に関わる人・企業との間でプログラムソース
の開示が必要ということのようです。  


<br />

## Githubの明示的にライセンスが付いていないソースコードについて  
Githubに明示的にライセンスされていないリポジトリはどのようになっているのか見ていきます。  
[GitHub Terms of Service(GitHubの利用規約)](https://docs.github.com/en/github/site-policy/github-terms-of-service)のD. User-Generated Content(ユーザー作成コンテンツ)の第5項には以下のように書かれておりGithubを使用するユーザーは以下に同意しています。  

```
5. License Grant to Other Users

Any User-Generated Content you post publicly, including issues, comments, and contributions to other Users' repositories, may 
be viewed by others. By setting your repositories to be viewed publicly, you agree to allow others to view and "fork" your 
repositories (this means that others may make their own copies of Content from your repositories in repositories they control).

If you set your pages and repositories to be viewed publicly, you grant each User of GitHub a nonexclusive, worldwide license 
to use, display, and perform Your Content through the GitHub Service and to reproduce Your Content solely on GitHub as permitted 
through GitHub's functionality (for example, through forking). You may grant further rights if you [adopt a license](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-license-to-a-repository#including-an-open-source-license-in-your-repository). 
If you are uploading Content you did not create or own, you are responsible for ensuring that the Content you upload is licensed 
under terms that grant these permissions to other GitHub Users.
```

**日本語訳**  


```
5.他のユーザーへのライセンス付与

問題、コメント、他のユーザーのリポジトリへの投稿など、あなたが公に投稿したユーザー生成コンテンツは、他のユーザーによって表示される可能性があります。
リポジトリを公開するように設定することにより、他の人があなたのリポジトリを表示および「フォーク」できるようにすることに同意したことになります
（これは、他の人が自分が管理するリポジトリ内の自分のリポジトリからコンテンツの独自のコピーを作成できることを意味します）。

ページとリポジトリを公開するように設定した場合、GitHubの各ユーザーに、GitHubサービスを通じてコンテンツを使用、表示、実行し、GitHubの機能で許可されて
いるようにGitHubでのみコンテンツを複製する非独占的な世界規模のライセンスを付与します（たとえば、フォークを介して）。ライセンスを採用すると、さらに権
利を付与できます。作成または所有していないコンテンツをアップロードする場合は、アップロードするコンテンツが他のGitHubユーザーにこれらのアクセス許可を
付与する条件に基づいてライセンスされていることを確認する責任があります。
```

これにより、リポジトGithubで閲覧とフォークなどGithub内でのみの活用は許可されていますが、コードをローカルにダウンロードしたりGitでgit Clone、git pull、git mergeでローカルに反映したりすることつまり、Github以外での活用が許可されていません。


***
