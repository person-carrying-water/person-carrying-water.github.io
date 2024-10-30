---
layout: default
title: ":newspaper: サポート表"
description: ":paperclip: Microsoft SQL Server サポート表"
date: "2021/04/18"
lastmod: "2024/04/30"
---

## 0. はじめに  
<br />
#### SQL Server 2022  
Microsoftは、2021年11月2日に時期バージョンの`SQL Server 2022`のプライベートプレビューを発表した。  
[SQL Server 2022](https://www.microsoft.com/en-us/sql-server/sql-server-2022)  

#### SQL Server 2012および2008  
Microsoftは、2021年7月14日SQL Server 2012についても**Extended Security Update(ESU)**を発表している。  
`SQL Server 2008、SQL Server 2008 R2およびSQL Server 2012は、拡張セキュリティ更新プログラム(ESU)を受けセキュリティサポートをさらに最大３年延長できる。`  
[拡張セキュリティ更新プログラム](https://docs.microsoft.com/ja-jp/lifecycle/faq/extended-security-updates)  
[SQL Server 用の延長セキュリティ更新プログラムとは](https://docs.microsoft.com/ja-jp/sql/sql-server/end-of-support/sql-server-extended-security-updates?view=sql-server-ver15)  

SP=Service Packの略  
GA=General Availability(一般出荷予定・製品版)の略  
CU=Cumulative Update(累積アップデート)の略  
GDR=General Distribution Release(一般向け修正プログラム)  
広範囲にわたって重要な問題を解決する一般的なソフトウェア更新プログラムの事を指します  
QFE=Quick Fix Engineering(応急的な修正プログラム)  
ソフトウェアの問題を修正するために応急的に作成される修正プログラムのこと
QFEはService Packとは違い、広範な環境でのテストが行われておらず、システムの構成や環境によっては効果がなかったり  
（不具合が修正できなかったり）、別の不具合が発生したりする可能性もある  

延長サポートはリリースから10年程度受けられると思われる。  

[アプリケーションとそのコンポーネントのバージョン、エディション、および更新SQL Server決定する](https://docs.microsoft.com/ja-jp/troubleshoot/sql/general/determine-version-edition-update-level)  
[アプリケーションとそのコンポーネントのバージョン、エディション、および更新SQL Server決定する(us)](https://docs.microsoft.com/en-us/troubleshoot/sql/general/determine-version-edition-update-level)  
[Microsoft SQL Server の最新の更新プログラム](https://docs.microsoft.com/ja-jp/sql/database-engine/install-windows/latest-updates-for-microsoft-sql-server?view=sql-server-ver15)  
[Microsoft SQL Server の最新の更新プログラム(US)](https://docs.microsoft.com/en-us/sql/database-engine/install-windows/latest-updates-for-microsoft-sql-server?view=sql-server-ver15)  
[更新プログラム、修正プログラムについて](https://support.microsoft.com/ja-jp/help/935897/an-incremental-servicing-model-is-available-from-the-sql-server-team-t)  

[SQL Server Compact 4.0ライフサイクル](https://docs.microsoft.com/ja-jp/lifecycle/products/microsoft-sql-server-compact-40)  
[SQL Server 2019リリースノート](https://docs.microsoft.com/ja-jp/sql/sql-server/sql-server-version-15-release-notes?view=sql-server-ver15)  
[SQL Server 2017ダウンロード](https://www.microsoft.com/ja-jp/sql-server/sql-server-downloads)  
[SQL Server 2019ダウンロード(US)](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)  

## SQL Server 2022  
**ビルド番号：16.0**  
**コードネーム：**  

### リリース、サポート期限  
[SQL Server 2022 サポート期限](https://learn.microsoft.com/ja-jp/lifecycle/products/sql-server-2022)  
[SQL Server 2022 リリースノート(jp)](https://docs.microsoft.com/ja-jp/sql/sql-server/sql-server-2022-release-notes?view=sql-server-ver16)  
[SQL Server 2022 リリースノート(us)](https://docs.microsoft.com/en-us/sql/sql-server/sql-server-2022-release-notes?view=sql-server-ver16)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
|すべてのエディション| 16.0.1000.6　　  | 2022/11/16 | 固定サイクル | 2022/11/16 | 2024/04/09 | 2028/01/11 | 2033/01/11 | 現在 |

### 更新プログラム  
[SQL Server2022の更新プログラム]()  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |   状態   |
| :-----------: | :---------- | ---------: | :-------: | :----------: | :-----: |
| CU12 GDR      | 16.0.4120.1 | 2024/04/09 | KB5036343 | 重大累積プログラム |  現在  |
| GDR           | 16.0.1115.1 | 2024/04/09 | KB5035432 | 重大更新プログラム |  現在  |
| CU12          | 16.0.43.229 | 2024/03/14 | KB5033663 | 累積更新プログラム |  現在  |
| CU11          | 16.0.4105.2 | 2024/01/11 | KB5032679 | 累積更新プログラム |  有効  |
| CU10 GDR      | 16.0.4100.1 | 2024/01/09 | KB5033592 | 重大累積プログラム |  有効  |
| GDR           | 16.0.1110.1 | 2024/01/09 | KB5032968 | 重大更新プログラム |  有効  |
| CU10          | 16.0.4095.4 | 2023/11/16 | KB5031778 | 累積更新プログラム |  有効  |
| CU9           | 16.0.4085.2 | 2023/10/12 | KB5030731 | 累積更新プログラム |  有効  |
| CU8           | 16.0.4075.1 | 2023/09/14 | KB5029666 | 累積更新プログラム |  有効  |
| CU7           | 16.0.4065.3 | 2023/08/10 | KB5028743 | 累積更新プログラム |  有効  |
| CU6           | 16.0.4055.4 | 2023/07/13 | KB5027505 | 累積更新プログラム |  有効  |
| CU5           | 16.0.4045.3 | 2023/06/15 | KB5026806 | 累積更新プログラム |  有効  |
| CU4           | 16.0.4035.4 | 2023/05/11 | KB5026717 | 累積更新プログラム |  有効  |
| CU3           | 16.0.4025.1 | 2023/04/13 | KB5024396 | 累積更新プログラム |  有効  |
| CU2           | 16.0.4015.1 | 2023/03/16 | KB5023127 | 累積更新プログラム |  有効  |
| CU1           | 16.0.4003.1 | 2023/02/16 | KB5022375 | 累積更新プログラム |  有効  |
| GDR           | 16.0.1050.5 | 2023/02/14 | KB5021522 | 重大更新プログラム |  有効  |
| GA(RTM)       | 16.0.1000.6 | 2022/11/16 | N/A       | N/A          |  有効  |
| RC1           | 16.0.950.9  | 2022/09/22 | N/A       | N/A          | rc |
| RC0           | 16.0.900.6  | 2022/08/23 | N/A       | N/A          | rc |
| CTP2.1        | 16.0.700.4  | 2022/07/27 | N/A       | N/A          | ctp |
| CTP2.0        | 16.0.600.9  | 2022/05/20 | N/A       | N/A          | ctp |

<br />

## SQL Server 2019  
**ビルド番号：15.0**  
**コードネーム：Seattle**  

### リリース、サポート期限  
[SQL Server 2019 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/sql-server-2019)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
|すべてのエディション| 15.0.2000.5    | 2019/11/04 | 固定サイクル | 2019/11/04 | 2024/04/09 | 2025/01/07 | 2030/01/08 |  現在  |

### 更新プログラム  
[SQL Server2019の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb4518398-sql-server-2019-%E3%83%93%E3%83%AB%E3%83%89-%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3-782ed548-1cd8-b5c3-a566-8b4f9e20293a)  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |   状態   |
| :------------: | :----------- | ---------: | :-------: | :-------------: | :-----: |
| CU26 GDR       | 15.0.4360.2  | 2024/04/09 | KB5036335 |重大累積プログラム |  現在  |
| GDR            | 15.0.2110.4  | 2024/04/09 | KB5035434 |重大更新プログラム |  現在  |
| CU26           | 15.0.4365.2  | 2024/04/09 | KB5035123 |累積更新プログラム|   現在  |
| CU25           | 15.0.4355.3  | 2024/02/15 | KB5033688 |累積更新プログラム|   有効  |
| CU24           | 15.0.4345.5  | 2023/12/14 | KB5031908 |累積更新プログラム|   有効  |
| CU23           | 15.0.4335.1  | 2023/10/12 | KB5030333 |累積更新プログラム|   有効  |
| CU22 GDR       | 15.0.4326.1  | 2024/10/10 | KB5029378 |重大累積プログラム |  有効  |
| GDR            | 15.0.2104.1  | 2023/10/10 | KB5029377 |重大更新プログラム |  有効  |
| CU22           | 15.0.4322.2  | 2023/08/14 | KB5027702 |累積更新プログラム|   有効  |
| CU21           | 15.0.4316.3  | 2023/06/15 | KB5025808 |累積更新プログラム|   有効  |
| CU20           | 15.0.4312.2  | 2023/04/13 | KB5024276 |累積更新プログラム|   有効  |
| CU19           | 15.0.4298.1  | 2023/02/16 | KB5023049 |累積更新プログラム|   有効  |
| CU18 GDR       | 15.0.4280.7  | 2023/02/14 | KB5021124 |重大累積プログラム| 有効 |
| GDR            | 15.0.2101.7  | 2023/02/14 | KB5021125 |重大更新プログラム| 有効 |
| CU18           | 15.0.4261.1  | 2022/09/28 | KB5017593 |累積更新プログラム|   有効  |
| CU17           | 15.0.4249.2  | 2022/08/11 | KB5016394 |累積更新プログラム|   有効  |
| CU16 GDR       | 15.0.4236.7  | 2022/06/14 | KB5014353 |重大累積プログラム| 有効 |
| GDR            | 15.0.2095.3  | 2022/06/14 | KB5014356 |重大更新プログラム| 有効 |
| CU16(Linux)    | 15.0.4223.1  | 2022/05/16 | KB5011644 |累積更新プログラム|   有効  |
| CU16(Big Data Clusters) | 15.0.4223.1  | 2022/05/10 | KB5011644 |累積更新プログラム|   有効  |
| CU16(Windows)  | 15.0.4223.1  | 2022/04/18 | KB5011644 |累積更新プログラム|   有効  |
| CU15           | 15.0.4198.2  | 2022/01/27 | KB5008996 |累積更新プログラム|   有効  |
| CU14           | 15.0.4188.2  | 2021/11/22 | KB5007182 |累積更新プログラム|  valid  |
| CU13           | 15.0.4178.1  | 2021/10/05 | KB5005679 |累積更新プログラム|  valid  |
| CU12           | 15.0.4153.1  | 2021/08/04 | KB5004524 |累積更新プログラム|  valid  |
| CU11           | 15.0.4138.2  | 2021/06/10 | KB5003249 |累積更新プログラム|  valid  |
| CU10           | 15.0.4123.1  | 2021/04/06 | KB5001090 |累積更新プログラム|  valid  |
| CU9            | 15.0.4102.2  | 2021/02/11 | KB5000642 |累積更新プログラム|  valid  |
| CU8 GDR        | 15.0.4083.2  | 2021/01/12 | KB4583459 |重大更新プログラム| current |
| GDR            | 15.0.2080.9  | 2021/01/12 | KB4583458 |重大更新プログラム| 有効 |
| CU8            | 15.0.4073.23 | 2020/10/01 | KB4577194 |累積更新プログラム|   ng?   |
| CU7            | 15.0.4063.15 | 2020/09/02 | KB4570012 |累積更新プログラム|   ng    |
| GDR1           | 15.0.2070.41 | 2019/11/04 | KB4517790 |重大更新プログラム|   old   |
| RTM            | 15.0.2000.5  | 2019/11/04 | N/A       | N/A              |  valid  |

<br />

## SQL Server 2017  
**ビルド番号：14.0**  
**コードネーム：Helsinki**  

### リリース、サポート期限  
[SQL Server 2017 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/sql-server-2017)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | ------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
|すべてのエディション| 14.0.1000.169  | 2017/10/02 | 固定サイクル | 2017/09/29 | 2023/10/10 | 2022/10/11 | 2027/10/12 |  現在  |

### 更新プログラム  
[SQL Server2017の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb4047329-sql-server-2017-%E3%83%93%E3%83%AB%E3%83%89-%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3-346e8fcd-c07c-5eeb-e10b-e3411ba8d8dd)  

|更新プログラム名 |  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |   状態   |
| :------------: | :----------- | ---------: | :-------: | :-------------: | :------: |
| CU31 GDR       | 14.0.3465.1  | 2023/10/10 | KB5029376 |重大累積プログラム| 現在 |
| GDR            | 14.0.2052.1  | 2023/10/10 | KB5029375 |重大更新プログラム| 現在 |
| CU31 GDR       | 14.0.3460.9  | 2023/02/14 | KB5021126 |重大累積プログラム| 有効 |
| GDR            | 14.0.2047.8  | 2023/02/14 | KB5021127 |重大更新プログラム| 有効 |
| CU31           | 14.0.3456.2  | 2022/09/20 | KB5016884 |累積更新プログラム| 有効 |
| CU30           | 14.0.3451.2  | 2022/07/13 | KB5013756 |累積更新プログラム| 有効 |
| CU29 GDR       | 14.0.3445.2  | 2022/06/14 | KB5014553 |重大累積プログラム| 有効 |
| GDR            | 14.0.2042.3  | 2022/06/14 | KB5014354 |重大更新プログラム| 有効 |
| CU29           | 14.0.3436.1  | 2022/03/30 | KB5010786 |累積更新プログラム| 有効 |
| CU28           | 14.0.3430.2  | 2022/01/13 | KB5008084 |累積更新プログラム|  valid  |
| CU27           | 14.0.3421.10 | 2021/10/27 | KB5006944 |累積更新プログラム|  valid  |
| CU26           | 14.0.3411.3  | 2021/09/14 | KB5005226 |累積更新プログラム|  valid  |
| CU25           | 14.0.3401.7  | 2021/07/12 | KB5003830 |累積更新プログラム|  valid  |
| CU24           | 14.0.3391.2  | 2021/05/10 | KB5001228 |累積更新プログラム|  valid  |
| CU23           | 14.0.3381.3  | 2021/02/24 | KB5000685 |累積更新プログラム|  valid  |
| CU22 GDR       | 14.0.3370.1  | 2021/01/21 | KB4583457 |重大更新プログラム| 有効 |
| GDR            | 14.0.2037.2  | 2021/01/21 | KB4583456 |重大更新プログラム| 有効 |
| CU22           | 14.0.3356.20 | 2020/09/10 | KB4577467 |累積更新プログラム|  valid  |
| CU21           | 14.0.3335.7  | 2020/07/01 | KB4557397 |累積更新プログラム|  valid  |
| GDR            | 14.0.2027.2  | 2019/07/09 | KB4505224 |重大更新プログラム|   old   |
| RTM            | 14.0.1000.169| 2017/09/29 | N/A       | N/A             |  valid  |

<br />

## SQL Server 2016  
**ビルド番号：13.0**  
**コードネーム：SQL16**  

### リリース、サポート期限  
[SQL Server 2016 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/sql-server-2016)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
| Service Pack3      | 13.0.6419.1    | 2021/09/15 | 固定サイクル | 2021/09/15 | 2023/10/10 | 2021/07/13 | 2026/07/14 | 現在 |
| Service Pack2      | 13.0.5026.0    | 2018/04/24 | 固定サイクル | 2018/04/24 | 2022/06/14 | 2021/07/13 | 2022/10/11 | **終了** |
| Service Pack1      | 13.0.4001.0    | 2016/11/17 | 固定サイクル | 2016/11/16 | 2019/07/09 | 2019/07/09 | 2019/07/09 | **終了** |
| Original Release   | 13.0.1601.5    | 2016/06/01 | 固定サイクル | 2016/06/01 | 2018/01/06 | 2018/01/09 | 2018/01/09 | **終了** |

### 更新プログラム  
[SQL Server2016の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb3177312-sql-server-2016-%E3%83%93%E3%83%AB%E3%83%89-%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3-d6cd8e5f-4aa3-20ac-f38f-8faef950840f)  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |  状態   |
| :------------: | :----------- | ---------: | :-------: | :--------------: | :-----: |
| Azure Connect Pack GDR | 13.0.7029.3  | 2023/10/10 | KB5029187 |重大更新プログラム|  現在  |
| SP3 GDR        | 13.0.6435.1  | 2023/10/10 | KB5029186 |重大更新プログラム|  現在  |
| SP3 GDR        | 13.0.6430.49 | 2023/02/14 | KB5021129 |重大更新プログラム|  有効  |
| SP3 GDR        | 13.0.6419.1  | 2022/06/14 | KB4052908 |重大更新プログラム|  有効  |
| SP2 CU17 + GDR | 13.0.5893.48 | 2022/06/14 | KB5014351 |重大累積プログラム| **終了** |
| SP2 GDR        | 13.0.5108.50 | 2022/06/14 | KB5014365 |重大更新プログラム| **終了** |
| SP3            | 13.0.6300.2  | 2021/09/15 | KB5003279 | サービスパック   |  有効  |
| SP2 CU17       | 13.0.5888.11 | 2021/03/29 | KB5001092 |累積更新プログラム| **終了** |
| SP2 CU16       | 13.0.5882.1  | 2021/02/11 | KB5000645 |累積更新プログラム| **終了** |
| SP2 CU15 + GDR | 13.0.5865.1  | 2021/01/12 | KB4583461 |重大更新プログラム| **終了** |
| SP2 GDR        | 13.0.5103.6  | 2021/01/12 | KB4583460 |重大更新プログラム| **終了** |
| SP2 CU15       | 13.0.5850.14 | 2020/09/28 | KB4577775 |累積更新プログラム| **終了** |
| SP2 CU11       | 13.0.5622.0  | 2020/02/11 | KB4535706 |累積セキュリティ更新| **終了** |
| SP2 GDR        | 13.0.5102.14 | 2020/02/11 | KB4532097 |重大更新プログラム| 非推奨 |
| SP2 CU11       | 13.0.5598.27 | 2019/12/09 | KB4527378 |累積更新プログラム| **終了** |
| SP2            | 13.0.5026.0  | 2018/04/24 | KB4052908 | サービスパック   | **終了** |
| SP1 CU15 + GDR | 13.0.4604.0  | 2019/07/09 | KB4505221 |重大更新プログラム| **終了** |
| SP1 GDR        | 13.0.4259.0  | 2019/07/09 | KB4505219 |重大更新プログラム| **終了** |
| SP1 CU15       | 13.0.4574.0  | 2019/05/16 | KB4495257 |累積更新プログラム| **終了** |
| SP1            | 13.0.4001.0  | 2016/11/17 | KB3182545 | サービスパック   | **終了** |
| GDR            | 13.0.1745.2  | 2018/01/06 | KB4058560 |重大更新プログラム| **終了** |
| CU9            | 13.0.2216.0  | 2017/11/21 | KB4037357 |累積更新プログラム| **終了** |

<br />

## SQL Server 2014  
**ビルド番号：12.0**  
**コードネーム：Hekaton**  

#### リリース、サポート期限  
[SQL Server 2014 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/sql-server-2014)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
| Service Pack3      | 12.0.6024.0    | 2018/10/30 | 固定サイクル | 2018/10/30 | 2023/10/10 | 2019/07/09 | 2024/07/09 | 現在 |
| Service Pack2      | 12.0.5000.0    | 2016/07/12 | 固定サイクル | 2016/07/14 | 2019/07/29 | 2019/07/09 | 2020/01/14 | **終了** |
| Service Pack1      | 12.0.4100.1    | 2015/05/04 | 固定サイクル | 2015/04/14 | 2017/08/08 | 2017/10/10 | 2017/10/10 | **終了** |
| Original Release   | 12.0.2000.8    | 2014/04/01 | 固定サイクル | 2014/06/05 | 2016/06/21 | 2016/07/12 | 2016/07/12 | **終了** |

### 更新プログラム  
[SQL Server2014の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb2936603-sql-server-2014-%E3%83%93%E3%83%AB%E3%83%89%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3-6f75da99-d86f-53fa-23ce-3d2b4825eccb)  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |  状態   |
| :------------: | :----------- | ---------: | :-------: | :--------------: | :-----: |
| SP3 CU4 + GDR  | 12.0.6449.1  | 2023/10/10 | KB5029185 |累積セキュリティ更新| 現在 |
| SP3 GDR        | 12.0.6179.1  | 2023/10/10 | KB5029184 |重大更新プログラム| 現在 |
| SP3 CU4 + GDR  | 12.0.6444.4  | 2023/02/14 | KB5021045 |累積セキュリティ更新| 非推奨 |
| SP3 GDR        | 12.0.6174.8  | 2023/02/14 | KB5021037 |重大更新プログラム| 非推奨 |
| SP3 CU4 + GDR  | 12.0.6439.10 | 2022/06/14 | KB5014164 |累積セキュリティ更新| 非推奨 |
| SP3 GDR        | 12.0.6169.19 | 2022/06/14 | KB5014165 |重大更新プログラム| 非推奨 |
| SP3 CU4 + GDR  | 12.0.6433.1  | 2021/01/12 | KB4583462 |累積セキュリティ更新| 非推奨 |
| SP3 GDR        | 12.0.6164.21 | 2021/01/12 | KB4583463 |重大更新プログラム| 非推奨 |
| SP3 CU4 + GDR  | 12.0.6372.1  | 2020/02/11 | KB4535288 |累積セキュリティ更新|   非推奨   |
| SP3 GDR        | 12.0.6118.4  | 2020/02/11 | KB4532095 |重大更新プログラム|   非推奨   |
| SP3 CU4        | 12.0.6329.1  | 2019/07/29 | KB4500181 |累積更新プログラム|  valid  |
| SP3            | 12.0.6024.0  | 2018/10/30 | KB4022619 | サービスパック   |  valid  |
| SP2 CU18       | 12.0.5687.1  | 2019/07/29 | KB4500180 |累積更新プログラム| **終了** |
| SP2 GDR        | 12.0.5223.6  | 2019/07/29 | KB4505217 |重大更新プログラム| **終了** |
| SP2            | 12.0.5000.0  | 2016/07/14 | KB3171021 | サービスパック   | **終了** |
| SP1 CU13       | 12.0.4520.0  | 2017/08/08 | KB4019099 |累積更新プログラム| **終了** |
| SP1 GDR        | 12.0.4522.0  | 2017/08/08 | KB4032542 |重大更新プログラム| **終了** |
| SP1            | 12.0.4100.1  | 2015/05/04 | KB3058865 | サービスパック   | **終了** |
| CU14           | 12.0.2569.0  | 2016/06/21 | KB3158271 |累積更新プログラム| **終了** |
| GDR(MS15-058)  | 12.0.2269.0  | 2015/07/14 | KB3045324 |重大更新プログラム| **終了** |

<br />

## SQL Server 2012  
**ビルド番号：11.0**  
**コードネーム：Denali**  

### リリース、サポート期限  
[SQL Server 2012 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/microsoft-sql-server-2012)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
| Extended Security Update Year 3 | 11.0.xxxx.0    | 2024/07/09 | 固定サイクル | 2024/07/09 | xxxx/xx/xx | 2025/07/08 | 2025/07/08 | 次期  |
| Extended Security Update Year 2 | 11.0.xxxx.0    | 2023/07/11 | 固定サイクル | 2023/07/11 | xxxx/xx/xx | 2024/07/09 | 2024/07/09 | 現在 |
| Extended Security Update Year 1 | 11.0.xxxx.0    | 2022/07/12 | 固定サイクル | 2022/07/12 | 2023/02/14 | 2023/07/11 | 2023/07/11 | **終了** |
| Service Pack4      | 11.0.7001.0    | 2017/10/02 | 固定サイクル | 2017/10/05 | 2021/01/12 | 2017/07/11 | 2022/07/12 | **終了** |
| Service Pack3      | 11.0.6020.0    | 2015/11/21 | 固定サイクル | 2015/12/01 | 2018/01/17 | 2017/07/11 | 2018/10/09 | **終了** |
| Service Pack2      | 11.0.5058.0    | 2014/06/10 | 固定サイクル | 2014/06/10 | 2017/01/18 | 2017/01/10 | 2017/01/10 | **終了** |
| Service Pack1      | 11.0.3000.00   | 2013/11/07 | 固定サイクル | 2012/11/07 | 2015/07/14 | 2015/07/14 | 2015/07/14 | **終了** |
| Original Release   | 11.0.2100.60   | 2012/03/06 | 固定サイクル | 2012/05/20 | 2013/12/17 | 2014/01/14 | 2014/01/14 | **終了** |

### 更新プログラム  
[SQL Server2012 SP2の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb2983249-sql-server-2012-sp2-%E3%81%AE%E3%83%93%E3%83%AB%E3%83%89%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3-2df8ef67-599a-b846-f0f8-c0193ea0ebad)  
[SQL Server2012 SP3の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb3133750-sql-server-2012-sp3-%E3%83%93%E3%83%AB%E3%83%89%E3%83%90%E3%83%BC%E3%82%B8%E3%83%A7%E3%83%B3-a2566e34-4930-8204-1e29-a7d61ad2373a)  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |  状態   |
| :------------: | :----------- | ---------: | :-------: | :--------------: | :-----: |
| SP4 GDR        | 11.0.7512.11 | 2023/02/14 | KB5021123 |重大更新プログラム| **終了** |
| SP4 GDR        | 11.0.7507.2  | 2021/01/12 | KB4583465 |重大更新プログラム| **終了** |
| SP4 GDR        | 11.0.7493.4  | 2020/02/11 | KB4532098 |重大更新プログラム|   old   |
| SP4            | 11.0.7001.0  | 2017/10/02 | KB4018073 | サービスパック   | **終了** |
| SP3 GDR        | 11.0.6260.1  | 2018/01/17 | KB4057115 |重大更新プログラム| **終了** |
| SP3 CU10       | 11.0.6607.3  | 2017/08/08 | KB4057121 |累積更新プログラム| **終了** |
| SP3            | 11.0.6020.0  | 2015/11/21 | KB3072779 | サービスパック   | **終了** |
| SP2 CU16       | 11.0.5678.0  | 2017/01/18 | KB3205054 |累積更新プログラム| **終了** |
| SP2 GDR(MS 16-136)| 11.0.5388.0  | 2016/11/08 | KB3194719 |重大更新プログラム| **終了** |
| SP2            | 11.0.5058.0  | 2014/06/10 | KB2958429 | サービスパック   | **終了** |
| SP1 CU16       | 11.0.3492.0  | 2015/05/18 | KB3052476 |累積更新プログラム| **終了** |
| SP1 GDR(MS 15-058)| 11.0.3156.0  | 2015/07/14 | KB3045318 |重大更新プログラム| **終了** |
| SP1            | 11.0.3000.00 | 2013/11/07 | KB2674319 | サービスパック   | **終了** |
| CU11           | 11.0.2424.0  | 2013/12/17 | KB2908007 |累積更新プログラム| **終了** |

<br />

## SQL Server 2008 R2  
**ビルド番号：10.50**  
**コードネーム：Kilimanjaro**  

### リリース、サポート期限  
[SQL Server 2008 R2 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/microsoft-sql-server-2008-r2)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
| Extended Security Update Year 4(Azure only) | 10.50.xxxx.0   | 2022/07/13 | 固定サイクル | 2022/07/13 | 2023/02/14 | 2023/07/11 | 2023/07/11 | **終了** |
| Extended Security Update Year 3 | 10.50.xxxx.0   | 2021/07/14 | 固定サイクル | 2021/07/14 | xxxx/xx/xx | 2022/07/12 | 2022/07/12 | **終了** |
| Extended Security Update Year 2 | 10.50.xxxx.0   | 2020/07/15 | 固定サイクル | 2020/07/15 | xxxx/xx/xx | 2021/07/13 | 2021/07/13 | **終了** |
| Extended Security Update Year 1 | 10.50.xxxx.0   | 2019/07/09 | 固定サイクル | 2019/07/09 | xxxx/xx/xx | 2020/07/14 | 2020/07/14 | **終了** |
| Service Pack3      | 10.50.6000.34    | 2014/09/26 | 固定サイクル | 2014/07/07 | 2018/01/07 | 2014/07/08 | 2019/07/09 | **終了** |
| Service Pack2      | 10.50.4000.0   | 2012/07/26 | 固定サイクル | 2012/07/26 | 2015/07/14 | 2015/10/13 | 2015/10/13 | **終了** |
| Service Pack1      | 10.50.2500.0   | 2011/07/12 | 固定サイクル | 2011/07/12 | 2013/06/17 | 2013/10/08 | 2013/10/08 | **終了** |
| Original Release   | 10.50.1600.1   | 2010/04/22 | 固定サイクル | 2010/07/20 | 2012/06/18 | 2012/07/10 | 2012/07/10 | **終了** |

### 更新プログラム  
[SQL Server 2008 R2 SP3 GDRの更新プログラム](https://support.microsoft.com/ja-jp/topic/sql-server-2008-r2-sp3-gdr-%E3%81%AE%E3%82%BB%E3%82%AD%E3%83%A5%E3%83%AA%E3%83%86%E3%82%A3%E6%9B%B4%E6%96%B0%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%A0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A62018-%E5%B9%B4-1-%E6%9C%88-7-%E6%97%A5-f8290bc2-5abe-934c-4672-c454db0b73f6)  
[SQL Server 2008 R2 SP2 CU13の更新プログラム](https://support.microsoft.com/ja-jp/topic/kb2967540-%E7%B4%AF%E7%A9%8D%E7%9A%84%E3%81%AA%E6%9B%B4%E6%96%B0%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%A0%E3%83%91%E3%83%83%E3%82%B1%E3%83%BC%E3%82%B8-13-sql-server-2008-r2-sp2-52262f9a-2889-d571-56b4-62ed1dc67f3a)  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |  状態   |
| :------------: | :----------- | ---------: | :-------: | :--------------: | :-----: |
| SP3 GDR        | 10.50.6785.2 | 2023/02/14 | KB5021112 |重大更新プログラム| **終了** |
| SP3 GDR        | 10.50.6560.0 | 2018/01/07 | KB4057113 |重大更新プログラム| **終了** |
| SP3 MS15-058   | 10.50.6525.0 | 2015/07/14 | KB3045314 |累積更新プログラム| **終了** |
| SP3            | 10.50.6000.34| 2014/07/07 | KB2979597 | サービスパック   | **終了** |
| SP2 GDR(MS 15-058)| 10.50.4042.0 | 2015/07/14 | KB3045313 |重大更新プログラム| **終了** |
| SP2 CU13       | 10.50.4319.0 | 2014/06/30 | KB2967540 |累積更新プログラム| **終了** |
| SP2            | 10.50.4000.0 | 2012/07/26 | KB2630458 | サービスパック   | **終了** |
| SP1 CU13       | 10.50.2876.0 | 2013/06/17 | KB2567616 |累積更新プログラム| **終了** |
| SP1            | 10.50.2500.0 | 2011/07/12 | KB2528583 | サービスパック   | **終了** |
| CU14           | 10.50.1817.0 | 2012/06/18 | KB2703280 |累積更新プログラム| **終了** |

<br />

## SQL Server 2008  
**ビルド番号：10.00**  
**コードネーム：Katmai**  

### リリース、サポート期限  
[SQL Server 2008 サポート期限](https://docs.microsoft.com/ja-jp/lifecycle/products/microsoft-sql-server-2008)  

| エディション       | 初回ビルド番号 | リリース日 | ﾗｲﾌｻｲｸﾙﾎﾟﾘｼｰ | ﾗｲﾌｻｲｸﾙ<br />の開始日 | 最新更新日 | ﾒｲﾝｽﾄﾘｰﾑ<br />ｻﾎﾟｰﾄ期限 | 延長<br>ｻﾎﾟｰﾄ期限 | 状態 |
| :----------------- | -------------: | ---------: |:------------:| ---------: | ---------: | ---------: | ---------: | :-----: |
| Extended Security Update Year 4(Azure only) | 10.00.xxxx.0   | 2022/07/13 | 固定サイクル | 2022/07/13 | 2023/02/14 | 2023/07/11 | 2023/07/11 | **終了** |
| Extended Security Update Year 3 | 10.00.xxxx.0   | 2021/07/14 | 固定サイクル | 2021/07/14 | xxxx/xx/xx | 2022/07/12 | 2022/07/12 | **終了** |
| Extended Security Update Year 2 | 10.00.xxxx.0   | 2020/07/15 | 固定サイクル | 2020/07/15 | xxxx/xx/xx | 2021/07/13 | 2021/07/13 | **終了** |
| Extended Security Update Year 1 | 10.00.xxxx.0   | 2019/07/09 | 固定サイクル | 2019/07/09 | xxxx/xx/xx | 2020/07/14 | 2020/07/14 | **終了** |
| Service Pack4      | 10.00.6000.29  | 2014/09/30 | 固定サイクル | 2014/07/07 | 2018/01/07 | 2014/07/08 | 2019/07/09 | **終了** |
| Service Pack3      | 10.00.5500.00  | 2011/10/06 | 固定サイクル | 2011/10/06 | 2015/07/14 | 2015/10/13 | 2015/10/13 | **終了** |
| Service Pack2      | 10.00.4000.00  | 2010/09/29 | 固定サイクル | 2010/09/24 | 2012/10/09 | 2012/10/09 | 2012/10/09 | **終了** |
| Service Pack1      | 10.00.2531.00  | 2009/04/07 | 固定サイクル | 2009/03/31 | 2011/09/19 | 2011/10/11 | 2011/10/11 | **終了** |
| Original Release   | 10.00.1600.22  | 2008/08/07 | 固定サイクル | 2008/11/06 | 2010/03/15 | 2010/04/13 | 2010/04/13 | **終了** |

### 更新プログラム  
[SQL Server 2008 SP4 GDRの更新プログラム](https://support.microsoft.com/ja-jp/topic/sql-server-2008-sp4-gdr-%E3%81%AE%E3%82%BB%E3%82%AD%E3%83%A5%E3%83%AA%E3%83%86%E3%82%A3%E6%9B%B4%E6%96%B0%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%A0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A62018-%E5%B9%B4-1-%E6%9C%88-7-%E6%97%A5-32b923c1-7af9-5c4b-5b3d-3522cab972fe)  
[SQL Server 2008 SP3 QFEの更新プログラム](https://support.microsoft.com/ja-jp/topic/-ms15-058-sql-server-2008-service-pack-3-qfe-%E3%81%AE%E3%82%BB%E3%82%AD%E3%83%A5%E3%83%AA%E3%83%86%E3%82%A3%E6%9B%B4%E6%96%B0%E3%83%97%E3%83%AD%E3%82%B0%E3%83%A9%E3%83%A0%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6-2015-%E5%B9%B4-7-%E6%9C%88-14-%E6%97%A5-9842908a-8d97-e474-aabd-927a3fab4380)  

|更新プログラム名|  ビルド番号  | 更新発表日 | ﾅﾚｯｼﾞﾍﾞｰｽ | 提供プログラム名 |  状態   |
| :------------: | :----------- | ---------: | :-------: | :--------------: | :-----: |
| SP4 GDR        | 10.0.6814.4  | 2023/02/14 | KB5020863 |重大更新プログラム| **終了** |
| SP4 GDR        | 10.00.6556.0 | 2018/01/07 | KB4057114 |重大更新プログラム| **終了** |
| SP4            | 10.00.6000.29| 2014/09/30 | KB2979596 | サービスパック   | **終了** |
| SP3 QFE(MS 15-058)| 10.00.5890.0 | 2015/07/14 | KB3045303 |重大更新プログラム| **終了** |
| SP3 CU17       | 10.00.5861.0 | 2014/05/19 | KB2958696 |累積更新プログラム| **終了** |
| SP3            | 10.00.5500.00| 2011/10/06 | KB2546951 | サービスパック   | **終了** |
| SP2 MS12-070   | 10.00.4371.0 | 2012/10/09 | KB2494089 |重要セキュリティ  | **終了** |
| SP2 CU11       | 10.00.4333.0 | 2012/07/16 | KB2715951 |累積更新プログラム| **終了** |
| SP2            | 10.00.4000.00| 2010/09/29 | KB2285068 | サービスパック   | **終了** |
| SP1 CU16       | 10.00.2850.0 | 2011/09/19 | KB2582282 |累積更新プログラム| **終了** |
| SP1            | 10.00.2531.00| 2009/04/07 | KB968369  | サービスパック   | **終了** |
| CU10           | 10.00.1835.0 | 2010/03/15 | KB979064  |累積更新プログラム| **終了** |

<br />

| 名称                   | ビルド番号         | ﾅﾚｯｼﾞﾍﾞｰｽ<br />番号 |      リリース日 | ライフサイクル<br>開始日 | サポート期限<br />ﾒｲﾝｽﾄﾘｰﾑ | サポート期限<br />延長 |    状態   |   ｺｰﾄﾞﾈｰﾑ   |
| :------------------- | :------------ | :---------------- | ---------: | -------------: | -------------------: | -------------: | :-----: | :---------: |
| 4.2                  | --            | --                | 1994/02/xx |             -- |           1999/07/01 |     1999/07/01 | **End** |    SQLNT    |
| 6.0 RTM              | 6.00.121      | --                | 1996/01/xx |             -- |           1999/03/31 |     1999/03/31 | **End** |    SQL95    |
| 6.0 SP1              | 6.00.124      | --                |         -- |             -- |                   -- |             -- | **End** |    SQL95    |
| 6.0 SP2              | 6.00.139      | --                |         -- |             -- |                   -- |             -- | **End** |    SQL95    |
| 6.0 SP3              | 6.00.151      | --                |         -- |             -- |                   -- |             -- | **End** |    SQL95    |
| 6.5 RTM              | 6.50.201      | --                | 1996/06/30 |     1996/06/30 |           2002/01/01 |     2002/01/01 | **End** |    Hydra    |
| 6.5 SP1              | 6.50.213      | --                |         -- |             -- |                   -- |             -- | **End** |    Hydra    |
| 6.5 SP2              | 6.50.240      | --                |         -- |             -- |                   -- |             -- | **End** |    Hydra    |
| 6.5 SP3              | 6.50.252      | --                |         -- |             -- |                   -- |             -- | **End** |    Hydra    |
| 6.5 SP3a             | 6.50.258      | --                |         -- |             -- |                   -- |             -- | **End** |    Hydra    |
| 6.5 SP4              | 6.50.281      | --                |         -- |             -- |           1999/03/24 |     1999/03/24 | **End** |    Hydra    |
| 6.5 SP5              | 6.50.416      | --                |         -- |             -- |                   -- |             -- | **End** |    Hydra    |
| 6.5 SP5a             | 6.50.416      | --                | 1998/12/24 |     1998/12/24 |           2002/01/01 |     2002/01/01 | **End** |    Hydra    |
| 6.5 SP5a<br>Update   | 6.50.479      | --                | 2000/09/12 |     2000/09/12 |           2002/01/01 |     2002/01/01 | **End** |    Hydra    |
| 7.0 RTM              | 7.00.623      | --                | 1998/11/27 |     1999/03/01 |           2005/12/31 |     2011/01/11 | **End** |    Sphinx   |
| 7.0 SP1              | 7.00.699      | --                | 1999/07/01 |             -- |                   -- |             -- | **End** |    Sphinx   |
| 7.0 SP2              | 7.00.842      | --                | 2000/03/20 |                |           2000/03/20 |     2000/03/20 | **End** |    Sphinx   |
| 7.0 SP3              | 7.00.961      | --                | 2000/12/15 |                |           2002/07/26 |     2002/07/26 | **End** |    Sphinx   |
| 7.0 SP4              | 7.00.1063     | --                | 2002/04/26 |     2002/04/26 |           2003/04/26 |     2003/04/26 | **End** |    Sphinx   |
| 2000 RTM             | 8.00.194      | --                | 2000/10/27 |     2000/11/30 |           2002/07/11 |     2002/07/11 | **End** |    Shiloh   |
| 2000 SP1             | 8.00.384      | --                | 2001/06/12 |     2001/06/12 |           2002/02/28 |     2002/02/28 | **End** |    Shiloh   |
| 2000 SP2             | 8.00.534      | --                | 2001/11/30 |     2001/11/30 |           2003/04/07 |     2003/04/07 | **End** |    Shiloh   |
| 2000 SP3             | 8.00.760      | --                | 2003/01/17 |     2003/01/07 |          2007/07/10? |    2007/07/10? | **End** |    Shiloh   |
| 2000 SP3a            | 8.00.0760.09  | --                | 2003/05/19 |     2003/01/07 |           2007/07/10 |     2007/07/10 | **End** |    Shiloh   |
| 2000 SP4             | 8.00.2039     | KB290211          | 2005/05/06 |     2005/05/06 |           2008/04/08 |     2013/04/09 | **End** |    Shiloh   |
| 2005 RTM             | 9.00.1399     | N/A               | 2005/12/15 |     2006/01/14 |           2007/07/10 |     2007/07/10 | **End** |    Yukon    |
| 2005 SP1             | 9.00.2047     | KB913090          | 2006/04/18 |     2006/04/18 |           2008/04/08 |     2008/04/08 | **End** |    Yukon    |
| 2005 SP2             | 9.00.3042     | KB921896          | 2007/02/13 |     2007/02/19 |           2010/01/12 |     2010/01/12 | **End** |    Yukon    |
| 2005 SP2 CU17        | 9.0.3356      | KB976952          | 2009/12/21 |     2007/02/19 |           2010/01/12 |     2010/01/12 | **End** |    Yukon    |
| 2005 SP3             | 9.00.4035     | KB955706          | 2008/12/15 |     2008/12/15 |           2012/01/10 |     2012/01/10 | **End** |    Yukon    |
| 2005 SP3 CU15        | 9.0.4325      | KB2507766         | 2011/03/22 |     2008/12/15 |           2012/01/10 |     2012/01/10 | **End** |    Yukon    |
| 2005 SP4             | 9.00.5000.00  | KB2463332         | 2010/12/17 |     2010/12/13 |           2011/04/12 |     2016/04/12 | **End** |    Yukon    |
| 2005 SP4 CU3         | 9.0.5266      | KB2507769         | 2011/03/22 |     2010/12/13 |           2011/04/12 |     2016/04/12 | **End** |    Yukon    |

* * *