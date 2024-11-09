---
layout: default
title: ":newspaper: Oracle Java"
description: ":paperclip: Oracle Java Development Kit リリース、サポート表"
date: "2019/03/30"
lastmod: "2024/11/09"
---

## 0. はじめに

Oracle JDK(本家)を商用目的で利用するには有料でOracle社と契約する必要があるJDK11～16があります。非商用(個人向け)または開発目的向けに限り  
無料で使うOTNライセンスの元で使うJDKもあります。  
※OracleサイトからOracle JDKアップデート(本家用)をダウンロードできるが非商用(個人向け)または開発目的向けでこれが提供される  
のは`2020年12月31日`までとなります。  

Oracle JDK17からは、再び商用利用でも無料で使う事ができるようになった。  
ただし、ソースの改変をしたもので商用利用を無料で使う事はできない。  
Oracleの長期リリース(LTS)を現在3年から2年周期へと変更するとしている。  

JDK10以前でも無料使用サポートでしたが、最終のJDK8の商用向け無償サポートは2019年01月31日で終了し2019年04月16日以降  
Oracle社のJavaのライセンスが変わりそれ以降のバージョンでの商用利用は有償となりました(非商用や開発は無料)。  
J2SE1.3は、2006年の1.3.1 Update 20を最後に、J2SE1.4は、2008年の1.4.2 Update 19を最後に無料サポートを終了しています。  
J2SE5.0は、2009年10月リリースのUpdate22を最後のUpdateとし2009年10月31日で無料サポートを終了しました。  
Java6は2013年2月の6u37リリースで無料サポートを終了しJava7は2015年04月30日で無償サポートを終了しています。  

また、商用利用も無料で使うには純正Oracle製ではなくAdopt製のOpenJDKやOracle製でもOpenJDK(サポート短い)など互換を使用する手もある。  
半年毎に新しいメジャーバージョンが出る。新しい長期サポート(LTS)版は６バージョン後(３年後)に出る。  
**Adopt Open JDKは、Eclipse Foundationと合同でADOPTIUMというJDKに置き換わって今後はリリースされます。**

<br />

## 1. Oracle JDKリリース、サポート表

[リリースノート](https://www.oracle.com/technetwork/java/javase/jdk-relnotes-index-2162236.html)  
[Oracle Java SE サポート・ロードマップ](https://www.oracle.com/technetwork/jp/java/eol-135779-ja.html)  
[Javaリリース](https://www.java.com/ja/download/faq/release_dates.xml)  
[ADOPTIUM(AdoptOpenJDK + Eclipse Foundation)](https://adoptium.net/)  
[Adopt OpenJDK サポート](https://adoptopenjdk.net/support.html)  
[RedHat OpenJDK サポート](https://access.redhat.com/ja/articles/1457743)  

### Oracle Java SE 23  
**リリースタイプ：non-LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 23         | 2024/09/17 | 2024/10/15 | 2025/03/31               | 利用不可                   | 無期限                     | 現在 |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 23のリリースノート](https://www.oracle.com/java/technologies/javase/23u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 23.0.2 | 2025/01/21 | 次期 |
| 23.0.1 + 11 | 2024/10/15 | 現在 |

<br />

### Oracle Java SE 22  
**リリースタイプ：non-LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 22         | 2024/03/19 | 2024/07/16 | 2024/09/30               | 利用不可                   | 無期限                     | **終了** |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 22のリリースノート](https://www.oracle.com/java/technologies/javase/22u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 22.0.2 + 9 | 2024/07/16 | **終了** |
| 22.0.1 + 8 | 2024/04/16 | **終了** |

<br />

### Oracle Java SE 21  
**リリースタイプ：LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | 無償<br />サポート期限 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | --------------------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 21         | 2023/09/19 | 2024/10/15 | 2026/09/30            | 2028/09/30               | 2031/09/30                 | 無期限                     | 現在  |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 21のリリースノート](https://www.oracle.com/java/technologies/javase/21u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 21.0.6     | 2025/01/21 | 次期 |
| 21.0.5 + 9  | 2024/10/15 | 現在 |
| 21.0.4 + 8  | 2024/07/16 | 有効 |
| 21.0.3 + 7  | 2024/04/16 | 有効 |
| 21.0.2 + 13 | 2024/01/16 | 有効 |
| 21.0.1 + 12 | 2023/10/17 | 有効 |

<br />

### Oracle Java SE 20  
**リリースタイプ：non-LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 20         | 2023/03/21 | 2023/07/18 | 2023/09/30               | 利用不可                   | 無期限                     | **終了** |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 20のリリースノート](https://www.oracle.com/java/technologies/javase/20u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 20.0.2 + 9 | 2023/07/18 | **終了** |
| 20.0.1 + 9 | 2023/04/18 | **終了** |

<br />

### Oracle Java SE 19  
**リリースタイプ：non-LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 19         | 2022/09/20 | 2023/01/17 | 2023/03/31               | 利用不可                   | 無期限                     | **終了** |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 19のリリースノート](https://www.oracle.com/java/technologies/javase/19u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 19.0.2 + 7  | 2023/01/17 | **終了**  |
| 19.0.1 + 10 | 2022/10/18 | **終了**  |

<br />

### Oracle Java SE 18  
**リリースタイプ：non-LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 18         | 2022/03/22 | 2022/08/18 | 2022/09/30               | 利用不可                   | 無期限                     | **終了** |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 18のリリースノート](https://www.oracle.com/java/technologies/javase/18u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 18.0.2.1 + 1 | 2022/08/18 | **終了** |
| 18.0.2 + 9  | 2022/07/19 | **終了** |
| 18.0.1.1 + 10 | 2022/05/02 | **終了** |
| 18.0.1 + 10 | 2022/04/19 | **終了** |

<br />

### Oracle Java SE 17  
**リリースタイプ：LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | 無償<br />サポート期限 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | --------------------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 17         | 2021/09/14 | 2024/10/15 | 2024/09/30            | 2026/09/30               | 2029/09/30                 | 無期限                     | 有効 |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 17のリリースノート](https://www.oracle.com/java/technologies/javase/17u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 17.0.14    | 2025/01/21 | 次期  |
| 17.0.13 + 10 | 2024/10/15 | 現在  |
| 17.0.12 + 8  | 2024/07/16 | 有効  |
| 17.0.11 + 7  | 2024/04/16 | 有効  |
| 17.0.10 + 11 | 2024/01/16 | 有効  |
| 17.0.9 + 11 | 2023/10/17 | 有効  |
| 17.0.8 + 9 | 2023/07/18 | 有効  |
| 17.0.7 + 8 | 2023/04/18 | 有効  |
| 17.0.6 + 9 | 2023/01/17 | 有効  |
| 17.0.5 + 9 | 2022/10/18 | 有効  |
| 17.0.4.1 + 1 | 2022/08/18 | 有効  |
| 17.0.4 + 11 | 2022/07/19 | 有効  |
| 17.0.3.1 + 8 | 2022/05/02 | 有効 |
| 17.0.3 + 8  | 2022/04/19 | 有効 |
| 17.0.2 + 8  | 2022/01/18 |  有効 |
| 17.0.1 + 12 | 2021/10/19 |  有効  |

<br />

### Oracle Java SE 16  
**リリースタイプ：non-LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 16         | 2021/03/16 | 2021/07/20 | 2021/09/30               | 利用不可                   | 無期限                     | **End** |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 16のリリースノート](https://www.oracle.com/java/technologies/javase/16u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 16.0.2 + 7 | 2021/07/20 | **End** |
| 16.0.1 + 9 | 2021/04/20 | **End** |

<br />

### Oracle Java SE 11  
**リリースタイプ：LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 11         | 2018/09/25 | 2024/10/15 | 2023/09/30               | 2032/01/31                 | 無期限                     | 有効 |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 11のリリースノート](https://www.oracle.com/java/technologies/javase/11u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 11.0.26    | 2025/01/21 | 次期  |
| 11.0.25 + 9 | 2024/10/15 | 現在  |
| 11.0.24 + 7 | 2024/07/16 | 有効  |
| 11.0.23 + 7 | 2024/04/16 | 有効 |
| 11.0.22 + 9 | 2024/01/16 | 有効  |
| 11.0.21 + 9 | 2023/10/17 | 有効  |
| 11.0.20 + 9 | 2023/07/18 | 有効  |
| 11.0.19 + 9 | 2023/04/18 | 有効  |
| 11.0.18 + 9 | 2023/01/17 | 有効  |
| 11.0.17 + 10 | 2022/10/18 | 有効 |
| 11.0.16.1 + 1 | 2022/08/18 | 有効 |
| 11.0.16 + 11 | 2022/07/19 | 有効 |
| 11.0.15.1 + 8 | 2022/05/02 | 有効 |
| 11.0.15 + 8 | 2022/04/19 | 有効 |
| 11.0.14 + 8 | 2022/01/18 |  有効  |
| 11.0.13 + 10| 2021/10/19 |  有効  |
| 11.0.12 + 8| 2021/07/20 | 有効  |

<br />

### Oracle Java SE 8  
**リリースタイプ：LTS**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | 無償<br />サポート期限 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | --------------------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 8          | 2014/03/18 | 2024/10/15 | 2019/01/31            | 2022/03/31               | 2030/12/31                 | 無期限                     | 有効 |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 8のリリースノート](https://www.oracle.com/java/technologies/javase/8u-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 8u441      | 2025/01/21 | 次期  |
| 8u431-b10  | 2024/10/15 | 現在  |
| 8u421-b09  | 2024/07/16 | 有効  |
| 8u411-b09  | 2024/04/16 | 有効  |
| 8u401-b10  | 2024/01/16 | 有効  |
| 8u391-b13  | 2023/10/17 | 有効  |
| 8u381-b09  | 2023/07/18 | 有効  |
| 8u371-b11  | 2023/04/18 | 有効  |
| 8u361-b09  | 2023/01/17 | 有効  |
| 8u351-b10  | 2022/10/18 | 有効  |
| 8u345-b31  | 2022/08/18 | 有効 |
| 8u341-b10  | 2022/07/19 | 有効 |
| 8u333-b09  | 2022/05/02 | 有効 |
| 8u331-b09  | 2022/04/19 | 有効 |
| 8u321-b07  | 2022/01/18 |  有効  |
| 8u311-b11  | 2021/10/19 |  有効  |
| 8u301-b09  | 2021/07/20 |  有効  |

<br />

### Oracle Java SE 7  
**リリースタイプ：---**  

#### リリース、サポート期限  
[Oracle Java SE Supportロードマップ](https://www.oracle.com/jp/java/technologies/java-se-support-roadmap.html)  
[Oracle Java SE Supportロードマップ(us)](https://www.oracle.com/java/technologies/java-se-support-roadmap.html)  

| バージョン | リリース日 | 最新更新日 | 無償<br />サポート期限 | Premier<br />サポート期限 | Extended<br />サポート期限 | Sustaining<br />サポート期限|  状態   |
| :--------- | ---------: | ---------: | --------------------: | -----------------------: | -------------------------: | -------------------------: | :-----: |
| 7          | 2011/07/28 | 2023/07/18 | 2015/04/30            | 2019/07/31               | 2022/07/31                 | 無期限                     | **終了** |

#### 更新版(Critical Patch Updates)  
[Oracle Java SE 7のリリースノート](https://www.oracle.com/java/technologies/javase/7u-relnotes.html)  
[Oracle Java SE 7のサポート・リリースノート](https://www.oracle.com/java/technologies/javase/7-support-relnotes.html)  

| ベースライン | 更新発表日 |   状態   |
| :--------- | ---------: | :-----: |
| 7u441-b08(Restricted)  | 2024/10/15 | **終了** |
| 7u431-b04(Restricted)  | 2024/07/16 | **終了** |
| 7u421-b06(Restricted)  | 2024/04/16 | **終了** |
| 7u411-b09(Restricted)  | 2024/01/16 | **終了** |
| 7u401-b07(Restricted)  | 2023/10/17 | **終了** |
| 7u391-b05(Restricted)  | 2023/07/18 | **終了** |
| 7u381-b08(Restricted)  | 2023/04/18 | **終了** |
| 7u371-b07(Restricted)  | 2023/01/17 | **終了** |
| 7u361-b08(Restricted) | 2022/10/18 | **終了** |
| 7u351-b07  | 2022/07/19 | **終了** |
| 7u343-b08  | 2022/05/02 | **終了** |
| 7u341-b08  | 2022/04/19 | **終了** |
| 7u331-b06  | 2022/01/18 | **終了** |
| 7u85-b15   | 2015/07/14 | **終了** |
| 7u80-b15   | 2015/04/14 | **終了** |
| 7u79-b15   | 2015/04/14 | **終了** |
| 7u1-b08    | 2011/10/18 | **終了** |

<br />

## 2. 過去のリリース・サポート表  

| バージョン         | 提供         |      リリース日 | Oracle 無償<br />サポート期限 | Oracle Premier<br />サポート期限 | Oracle Extended<br />サポート期限 |    状態    | LTS |
| :------------ | :--------- | ---------: | --------------------: | -------------------------: | --------------------------: | :------: | :-: |
| 1.0.0         | Oracle JDK | 1996/01/23 |                    ?? |                       none |                        none |  **End** |  -- |
| 1.1.0         | Oracle JDK | 1997/02/19 |                    ?? |                       none |                        none |  **End** |  -- |
| 1.2.0         | Oracle JDK | 1998/12/08 |                    ?? |                       none |                        none |  **End** |  -- |
| 1.3.0         | Oracle JDK | 2000/05/08 |            2006/12/31 |                       none |                        none |  **End** |  -- |
| 1.4.0         | Oracle JDK | 2002/02/06 |            2008/10/31 |                       none |                        none |  **End** |  -- |
| 1.5.0         | Oracle JDK | 2004/09/30 |            2009/10/31 |                       none |                        none |  **End** |  -- |
| 1.5.0         | Oracle JDK | 2004/09/30 |            2009/10/31 |                       none |                        none |  **End** |  -- |
| 1.6.0         | Oracle JDK | 2006/12/11 |            2013/02/19 |                 2015/12/31 |                  2018/12/31 |  **End** |  -- |
| 1.6.0_37-b06  | Oracle JDK | 2013/02/19 |            2013/02/19 |                 2015/12/31 |                  2018/12/31 |  **End** |  -- |
| 1.6.0_211-b11 | Oracle JDK | 2018/10/16 |            2013/02/19 |                 2015/12/31 |                  2018/12/31 |  **End** |  -- |
| 1.8.0         | Oracle JDK | 2014/03/18 |            2019/01/31 |                 2022/03/31 |                  2030/12/31 |   valid  |  -- |
| 9 + 181       | Oracle JDK | 2017/09/21 |            2018/03/20 |                 2018/03/20 |                        none |  **End** | non |
| 9.0.1 + 11    | Oracle JDK | 2017/10/17 |            2018/03/20 |                 2018/03/20 |                        none |  **End** | non |
| 9.0.4 + 11    | Oracle JDK | 2018/01/16 |            2018/03/20 |                 2018/03/20 |                        none |  **End** | non |
| 10            | Oracle JDK | 2018/03/20 |            2018/09/25 |                 2018/09/25 |                        none |  **End** | non |
| 10.0.1 + 10   | Oracle JDK | 2018/04/17 |            2018/09/25 |                 2018/09/25 |                        none |  **End** | non |
| 10.0.2 + 13   | Oracle JDK | 2018/07/17 |            2018/09/25 |                 2018/09/25 |                        none |  **End** | non |
| 12 + 33       | Oracle JDK | 2019/03/19 |                    -- |                 2019/09/17 |                        none |  **End** | non |
| 12.0.1 + 12   | Oracle JDK | 2019/04/16 |                    -- |                 2019/09/17 |                        none |  **End** | non |
| 12.0.2 + 10   | Oracle JDK | 2019/07/16 |                    -- |                 2019/09/17 |                        none |  **End** | non |
| 13 + 13       | Oracle JDK | 2019/09/17 |                    -- |                 2020/03/31 |                        none |  **End** | non |
| 13.0.1 + 9    | Oracle JDK | 2019/10/15 |                    -- |                 2020/03/31 |                        none |  **End** | non |
| 13.0.2 + 8    | Oracle JDK | 2020/01/14 |                    -- |                 2020/03/31 |                        none |  **End** | non |
| 14 + 36       | Oracle JDK | 2020/03/17 |                    -- |                 2020/09/30 |                        none |  **End** | non |
| 14.0.2 + 12   | Oracle JDK | 2020/07/14 |                    -- |                 2020/09/30 |                        none |  **End** | non |
| 15 + 36       | Oracle JDK | 2020/09/15 |                    -- |                 2021/03/31 |                        none |  **End** | non |
| 15.0.2 + 7    | Oracle JDK | 2021/01/19 |                    -- |                 2021/03/31 |                        none |  **End** | non |

<br />

## 4. Amazon Corretoリリース、サポート表

[amazon correto(github)](https://github.com/corretto)  
[よくある質問](https://aws.amazon.com/jp/corretto/faqs/)  

> #### Amazon抜粋
>
> #### 全般
>
> Q:長期サポート (LTS) は Corretto にとって何を意味しますか?  
> A: Amazon Corretto は、マルチプラットフォームで本番環境に対応した、長期サポート (LTS) を含む無料の Open Java Development Kit  
> (OpenJDK) ディストリビューションです。LTS には、最短でも関連するリリースバージョンの指定日 (例: Corretto 8 の場合は2026年5月)  
> までは、パフォーマンスの向上とセキュリティの更新を無償で提供するという Amazon のコミットメントが含まれています。アップデートは  
> 四半期ごとにリリースされる予定です。Amazon では、通常の四半期サイクルの範囲外で、利用可能になった際に緊急で対応できる修正 (セキ  
> ュリティを含む) を適用することも計画しています。  

> Q: Corretto の長期サポートには何が含まれますか?  
> A: Corretto の長期サポート (LTS) には、無償のパフォーマンス強化およびセキュリティアップデートが含まれます。このサポートは最短で  
> も Corretto 8 は 2026 年 5 月まで、Corretto 11 は 2027 年 9 月までご利用いただけます。アップデートは四半期ごとにリリースされる  
> 予定です。  

> Corretto の LTS は、AWS に関するお客様の目的を達成するために専門家の指導とサポートを提供する AWS サポートのプランとは無関係です。  
> すでに AWS サポートのプランに契約済みの場合、Corretto はほかのすべてのサポートされている AWS サービスおよびソフトウェアと同じ基準  
> でカバーされます。プランを契約していないお客様で、Correto のサポートのみが目的である場合、プランの契約は意味を持たないかもしれませ  
> ん。プランが最適であるかどうか判断するには、ウェ> ブサイトにアクセスしてください。現在のところ、Corretto 固有のサポートプランを開  
> 始する予定はありません。当社のロードマップはすべてお客様からのフィードバックを反映したものです。機能に関するご要望はCorretto GitHub  
> レポジトリからお寄せください。  

| バージョン  | 提供OS            |  リリース日 | サポート期限 | 状態   |
| :---------- | :---------------- | ---------: | ---------: | :-----: |
| 8.302.08.1  | すべて            | 2021/07/21 | 2026/05/31 | current |
| 11.0.12.7.1 | すべて            | 2021/07/21 | 2027/09/30 | current |
| 15.0.2.7.1  | すべて            | 2021/01/22 | 2021/04/20 | **End** |
| 16.0.2.7.1  | すべて            | 2021/07/24 | 2021/10/19 | **End** |
| 17.0.0.35.1 | すべて            | 2021/09/16 | TBD        | current |

* * *
