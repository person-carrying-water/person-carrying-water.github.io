---
layout: default
title: ":newspaper: オープンソースソフトウェアライセンス(OSS)"
description: ":page_with_curl: MITライセンス"
date: "2022/01/04"
lastmod: "2022/01/04"
---

## 0. はじめに
MITライセンスは、BSDライセンスタイプの非コピーレフト型の非常に緩いライセンスです。  

ライセンスタイプ：**BSDライセンス**  
伝番タイプ：**非伝番タイプ(非コピーレフト)**  

<br />

## 1. ライセンス条件  
### 必要な条件  
ライセンスを守るために必要な作業です。  

1. 利用する著者の著作権表示を記載あるいは記載したファイルを付属する  
2. ライセンス本文(リンク可)を記載あるいは記載したファイルを付属する  
3. 免責事項(リンク可)を記載あるいは記載したファイルを付属する  
4. NOTICLEファイルがあればそれも付属する  

### 許可されている事  
1. 商用利用  
2. 複製、改変  
3. 頒布(はんぷ)、再頒布  
4. 再許諾(サブライセンス)  

### 禁止されている事
1. ライセンサーや作者へ責任を追及する事  
2. ライセンサーや作者が責任を負うようにライセンスする事  
3. ライセンス本文および免責事項を改変する事(そのままのライセンス文を使用する事)  

### 免除されている事  
1. 無償(無料)  
2. ソースコードの開示(公開)  

<br />

## 2. 記載、付属方法  
### ライセンスファイルで行う方法  
LICENSEファイルなどにライセンス全文を記載する。  

### バイナリ形式のみで行う方法  
デスクトップアプリなどのバイナリのみで行う場合は、Aboutや設定などに記載する。  

### URLリンクを掲載する方法  
ライセンス全文でなくても、オープンソース・イニシアティブのウェブサイトのURLをリンクを記載する事も可能なようです。  
プログラムソースの中に埋め込む方法に適しています。  

```
Copyright (c) <year> <copyright holders>
Released under the MIT license
https://opensource.org/licenses/mit-license.php
```

### 関数やクラス単位で掲載する方法  
ソースコード単位ではなく、関数やクラスなど一部のみ活用する場合`「The 関数名 function is: ライセンス表示」`とする事も可能なようです。  
```
The inherits function is:
ISC license | https://github.com/isaacs/inherits/blob/master/LICENSE
```

<br />

## 3. ライセンス全文  
### 原文  
MITライセンスで提供されているライブラリ、ソースコード名称<利用するソフトウェア名>をどこかに記入する場合もある。  

```
MIT License

Copyright (c) <year> <copyright holders>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

### 日本語訳  
```
MIT License

Copyright (c) <著作権発生年> <著作権保持者名>

以下に定める条件に従い、本ソフトウェアおよび関連文書のファイル（以下「ソフトウェア」）の
複製を取得するすべての人に対し、ソフトウェアを無制限に扱うことを無償で許可します。
これには、ソフトウェアの複製を使用、複写、変更、結合、掲載、頒布、サブライセンス、および
/または販売する権利、およびソフトウェアを提供する相手に同じことを許可する権利も無制限に
含まれます。

上記の著作権表示および本許諾表示を、ソフトウェアのすべての複製または重要な部分に記載する
ものとします。

ソフトウェアは「現状のまま」で、明示であるか暗黙であるかを問わず、何らの保証もなく提供されます。
ここでいう保証とは、商品性、特定の目的への適合性、および権利非侵害についての保証も含みますが、
それに限定されるものではありません。 作者または著作権者は、契約行為、不法行為、またはそれ以外で
あろうと、ソフトウェアに起因または関連し、あるいはソフトウェアの使用またはその他の扱いによって
生じる一切の請求、損害、その他の義務について何らの責任も負わないものとします。
```

***
