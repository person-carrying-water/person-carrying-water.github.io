---
layout: default
title: ":newspaper: サポート表"
description: ":paperclip: Microsoft SQL Server 接続ドライバー サポート表"
date: "2021/05/17"
lastmod: "2024/08/27"
---

## .NET Framework Data Provider for SQL Server

.NET同梱により.NETのサポート状況による  

<br />

## Microsoft.EntityFrameworkCore.SqlServer

.NET Core、ASP.NET Core、EntityFramework Core、EntityFrameowrkCore SQLServerは、.NET Coreのサポート状況による。  

[NuGet EntityFrameowrkCore SQLServer](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer)  
[Entity Framework Core](https://github.com/aspnet/EntityFrameworkCore)  
[.NET Core](https://github.com/dotnet/core/blob/master/microsoft-support.md)  
[.NET Core サポートポリシー](https://dotnet.microsoft.com/platform/support/policy/dotnet-core)  

> ### Microsoft抜粋
>
> #### 対象範囲
>
> .NET Coreは、.NET Core、ASP.NET Core、Entity Framework Coreを含むいくつかのテクノロジーを指します。
> .NETプラットフォームの別の部分のサポートポリシーをお探しですか？ .NETサポートポリシーを参照してください。

> すべてのマイクロソフト製品にはライフサイクルがあります。ライフサイクルは、製品がリリースされたときに始まり、サポートされなくなったときに終わります。
> このライフサイクルの重要な日付を知ることは、ソフトウェアをいつアップグレードするか、または他の変更を行うかについて、十分な情報に基づいた決定を下すのに役立ちます。
> この製品は、Microsoftのモダンライフサイクルポリシーに準拠しています。

> .NET Coreサポートライフサイクルは、各リリースのサポートを提供します。時間の長さとサポートの程度は、いくつかの資格によって異なります。

<br />

## Microsoft JDBC Driver for SQL Server

JDBC ドライバーのバージョン 3.0、4.x、6.x、7.x、および 8.x には、ドライバーのリリース日から 5 年間のメインストリーム サポートが含まれています。  
延長サポートとカスタム サポートのオプションは、Microsoft JDBC Driver では使用できません。  
[Microsoft JDBC Driver for SQL Server サポート](https://docs.microsoft.com/ja-jp/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server-support-matrix?view=sql-server-2017)  
[Microsoft JDBC Driver for SQL Server サポート(us)](https://docs.microsoft.com/en-us/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server-support-matrix?view=sql-server-ver15)  
[Microsoft JDBC Driver for SQL Server(GitHub)](https://github.com/Microsoft/mssql-jdbc)  
[Microsoft JDBC Driver for SQL Server リリースノート](https://docs.microsoft.com/ja-jp/sql/connect/jdbc/release-notes-for-the-jdbc-driver?view=sql-server-2017)  

| Version  | ドライバー名                                    | リリースタイプ       |      リリース日 | メインストリーム<br />サポート期限 | サポートJava            |    状態   |
| :------- | :---------------------------------------- | :------------ | ---------: | -------------------: | :------------------ | :-----: |
| 12.8.1   | Microsoft JDBC Driver 12.8 for SQL Server | Hotfix&Stable | 2024/08/22 |           2029/07/31 | JRE11、JRE8               | 現在 |
| 12.8.0   | Microsoft JDBC Driver 12.8 for SQL Server | Stable        | 2024/07/31 |           2029/07/31 | JRE11、JRE8               | 有効 |
| 12.7.1   | Microsoft JDBC Driver 12.7 for SQL Server | Preview       | 2024/07/09 |           2024/07/31 | JRE11、JRE8               | プレビュー |
| 12.7.0   | Microsoft JDBC Driver 12.7 for SQL Server | Preview       | 2024/04/06 |           2024/07/31 | JRE11、JRE8               | プレビュー |
| 12.6.3   | Microsoft JDBC Driver 12.6 for SQL Server | Hotfix&Stable | 2024/06/21 |           2029/01/31 | JRE11、JRE8               | 現在 |
| 12.6.2   | Microsoft JDBC Driver 12.6 for SQL Server | Hotfix&Stable | 2024/05/25 |           2029/01/31 | JRE11、JRE8               | 有効 |
| 12.6.1   | Microsoft JDBC Driver 12.6 for SQL Server | Hotfix&Stable | 2024/02/20 |           2029/01/31 | JRE11、JRE8               | 有効 |
| 12.6.0   | Microsoft JDBC Driver 12.6 for SQL Server | Stable        | 2024/02/02 |           2029/01/31 | JRE11、JRE8               | 有効 |
| 12.5.0   | Microsoft JDBC Driver 12.5 for SQL Server | Preview       | 2023/11/17 |           202x/xx/xx | JRExx                     | プレビュー |
| 12.4.2   | Microsoft JDBC Driver 12.4 for SQL Server | Hotfix&Stable | 2023/10/28 |           2028/07/31 | JRE11、JRE8               | 現在 |
| 12.4.1   | Microsoft JDBC Driver 12.4 for SQL Server | Hotfix&Stable | 2023/08/31 |           2028/07/31 | JRE11、JRE8               | 有効 |
| 12.4.0   | Microsoft JDBC Driver 12.4 for SQL Server | Stable        | 2023/08/01 |           2028/07/31 | JRE11、JRE8               | 有効 |
| 12.2.0   | Microsoft JDBC Driver 12.2 for SQL Server | Stable        | 2023/02/02 |           2028/01/31 | JRE11、JRE8               | 現在 |
| 11.2.3   | Microsoft JDBC Driver 11.2 for SQL Server | Hotfix&Stable | 2023/01/13 |           2027/08/04 | JRE18、JRE17、JRE11、JRE8 | 現在 |
| 11.2.2   | Microsoft JDBC Driver 11.2 for SQL Server | Hotfix&Stable | 2022/12/15 |           2027/08/04 | JRE18、JRE17、JRE11、JRE8 | 有効 |
| 11.2.1   | Microsoft JDBC Driver 11.2 for SQL Server | Hotfix&Stable | 2022/09/08 |           2027/08/04 | JRE18、JRE17、JRE11、JRE8 | 有効 |
| 11.2.0   | Microsoft JDBC Driver 11.2 for SQL Server | Stable        | 2022/08/04 |           2027/08/04 | JRE18、JRE17、JRE11、JRE8 | 有効 |
| 10.2.3   | Microsoft JDBC Driver 10.2 for SQL Server | Hotfix&Stable | 2023/01/13 |           2027/01/31 | JRE17、JRE11、JRE8  | 現在 |
| 10.2.2   | Microsoft JDBC Driver 10.2 for SQL Server | Hotfix&Stable | 2022/12/15 |           2027/01/31 | JRE17、JRE11、JRE8  | 有効 |
| 10.2.1   | Microsoft JDBC Driver 10.2 for SQL Server | Hotfix&Stable | 2022/05/12 |           2027/01/31 | JRE17、JRE11、JRE8  | 有効 |
| 10.2.0   | Microsoft JDBC Driver 10.2 for SQL Server | Stable        | 2022/01/31 |           2027/01/31 | JRE17、JRE11、JRE8  | 有効 |
| 9.4.1    | Microsoft JDBC Driver 9.4 for SQL Server  | Hotfix&Stable | 2021/12/07 |           2026/07/30 | JRE16、JRE11、JRE8    | current |
| 9.4.0    | Microsoft JDBC Driver 9.4 for SQL Server  | Stable        | 2021/08/04 |           2026/07/30 | JRE16、JRE11、JRE8    |  valid  |
| 9.2.1    | Microsoft JDBC Driver 9.2 for SQL Server  | Hotfix&Stable | 2021/02/26 |           2026/01/29 | JRE15、JRE11、JRE8    | current |
| 9.2.0    | Microsoft JDBC Driver 9.2 for SQL Server  | Stable        | 2021/01/28 |           2026/01/29 | JRE15、JRE11、JRE8    |  valid  |
| 8.4.1    | Microsoft JDBC Driver 8.4 for SQL Server  | Hotfix&Stable | 2020/08/27 |           2025/07/31 | JRE14、JRE11、JRE8    | current |
| 8.4.0    | Microsoft JDBC Driver 8.4 for SQL Server  | Stable        | 2020/07/31 |           2025/07/31 | JRE14、JRE11、JRE8    |  valid  |
| 8.3.1    | Microsoft JDBC Driver 8.3 for SQL Server  | Preview       | 2020/05/29 |           2025/04/01 | JRE14、JRE11、JRE8    | preview |
| 8.2.2    | Microsoft JDBC Driver 8.2 for SQL Server  | Hotfix&Stable | 2020/03/24 |           2025/03/24 | JRE14、JRE11、JRE8    | current |
| 8.2.1    | Microsoft JDBC Driver 8.2 for SQL Server  | Hotfix&Stable | 2020/02/26 |           2025/02/26 | JRE13、JRE11、JRE8    |  valid  |
| 8.2.0    | Microsoft JDBC Driver 8.2 for SQL Server  | Stable        | 2020/01/31 |           2025/01/31 | JRE13、JRE11、JRE8    |  valid  |
| 7.4.1    | Microsoft JDBC Driver 7.4 for SQL Server  | Hotfix&Stable | 2019/08/01 |           2024/08/02 | JRE12、JRE11、JRE8    | **終了** |
| 7.4.0    | Microsoft JDBC Driver 7.4 for SQL Server  | Stable        | 2019/07/31 |           2024/07/31 | JRE12、JRE11、JRE8    | **終了** |
| 7.2.2    | Microsoft JDBC Driver 7.2 for SQL Server  | Hotfix&Stable | 2019/04/17 |           2024/04/16 | JRE11、JRE8          | **終了** |
| 7.2.1    | Microsoft JDBC Driver 7.2 for SQL Server  | Hotfix&Stable | 2019/02/11 |           2024/02/11 | JRE11、JRE8          | **終了** |
| 7.2.0    | Microsoft JDBC Driver 7.2 for SQL Server  | Stable        | 2019/01/31 |           2024/01/31 | JRE11、JRE8          | **終了** |
| 7.0.0    | Microsoft JDBC Driver 7.0 for SQL Server  | Stable        | 2018/07/31 |           2023/07/31 | JRE10、JRE8          | **終了** |
| 6.4.0    | Microsoft SQL Server 用 JDBC Driver 6.4    | Stable        | 2018/02/27 |           2023/02/27 | JRE9、JRE8、JRE7      | **終了** |
| 6.2.2    | Microsoft JDBC Driver 6.2 for SQL Server  | Hotfix&Stable | 2017/09/29 |           2022/09/29 | JRE8、JRE7           | **終了** |
| 6.2.1    | Microsoft JDBC Driver 6.2 for SQL Server  | Hotfix&Stable | 2017/07/14 |           2022/07/14 | JRE8、JRE7           | **終了** |
| 6.2.0    | Microsoft JDBC Driver 6.2 for SQL Server  | Stable        | 2017/06/30 |           2022/06/30 | JRE8、JRE7           | **終了** |
| 6.1.0    | Microsoft JDBC Driver 6.1 for SQL Server  | Stable        | 2016/11/17 |           2021/11/17 | JRE8、JRE7           | **終了** |
| 6.0.8112 | Microsoft SQL Server 用 JDBC Driver 6.0    | Stable        | 2016/07/14 |           2021/07/14 | JRE8、JRE7           | **終了** |
| 4.2.8112 | Microsoft SQL Server 用 JDBC Driver 4.2    | Stable        | 2015/08/24 |           2020/08/24 | JRE8、JRE7、JRE6、JRE5 | **終了** |
| 4.1.8112 | Microsoft SQL Server 用 JDBC Driver 4.1    | Stable        | 2014/12/12 |           2019/12/12 | JRE7、JRE6、JRE5      | **終了** |
| 4.0      | Microsoft SQL Server 用 JDBC Driver 4.0    | Stable        | 2012/03/06 |           2017/03/06 | JRE7、JRE6、JRE5      | **終了** |
| 3.0      | Microsoft SQL Server JDBC Driver 3.0      | Stable        | 2010/04/23 |           2015/04/23 | JRE6、JRE5           | **終了** |
| 2.0      | Microsoft SQL Server JDBC Driver 2.0      | Stable        | 2007/12/31 |           2012/12/31 | RE6、JRE5            | **終了** |
| 1.2      | Microsoft SQL Server 2005 JDBC ドライバー 1.2  | Stable        | 2006/06/25 |           2011/06/25 | RE6、JRE5、JRE4       | **終了** |
| 1.1      | Microsoft SQL Server 2005 JDBC Driver 1.1 | Stable        | 2006/06/25 |           2011/06/25 | JRE4                | **終了** |
| 1.0      | Microsoft SQL Server 2005 JDBC Driver 1.0 | Stable        | 2006/06/25 |           2011/06/25 | JRE4                | **終了** |
| 2000     | Microsoft SQL Server 2000 JDBC Driver     | Stable        | 2005/07/09 |           2010/07/09 | JRE4                | **終了** |

<br />

## Microsoft Drivers for PHP for SQL Server

PHP ドライバーのバージョン 3.x、4.x、5.x には、ドライバーのリリース日から 5 年間のメインストリーム サポートが含まれています。  
延長サポートとカスタム サポートのオプションは、Microsoft PHP Driver では使用できません。  
[Microsoft Drivers for PHP for SQL Server サポート](https://docs.microsoft.com/ja-jp/sql/connect/php/microsoft-php-drivers-for-sql-server-support-matrix?view=sql-server-2017)  
[Microsoft Drivers for PHP for SQL Server サポート(US)](https://docs.microsoft.com/en-us/sql/connect/php/microsoft-php-drivers-for-sql-server-support-matrix?view=sql-server-ver15)  
[Microsoft Drivers for PHP for Microsoft SQL Server(GitHub)](https://github.com/microsoft/msphpsql)  
[Microsoft Drivers for PHP for SQL Server リリースノート](https://docs.microsoft.com/ja-jp/sql/connect/php/release-notes-php-sql-driver?view=sql-server-2017)  

| Version | ドライバー名                               | リリースタイプ    |      リリース日 | メインストリーム<br />サポート期限 | サポートPHP                         |    状態   |
| :------ | :----------------------------------- | :--------- | ---------: | -------------------: | :------------------------------ | :-----: |
| 5.12.0  | SQL Server 用 Microsoft PHP ドライバー 5.12| Production | 2024/01/09 |           2029/01/31 | 8.3.0+<br />8.2.0+<br />8.1.0+  | 現在 |
| 5.12.0-beta1 | SQL Server 用 Microsoft PHP ドライバー 5.12| Production | 2023/12/09 |      2029/01/25 | 8.3.0+<br />8.2.0+<br />8.1.0+  | ベータ |
| 5.11.1  | SQL Server 用 Microsoft PHP ドライバー 5.11| Production | 2023/09/06 |           2028/02/28 | 8.2.0+<br />8.1.0+<br />8.0.0+  |   現在  |
| 5.11.0  | SQL Server 用 Microsoft PHP ドライバー 5.11| Production | 2023/03/07 |           2028/02/28 | 8.2.0+<br />8.1.0+<br />8.0.0+  |   有効  |
| 5.10.1  | SQL Server 用 Microsoft PHP ドライバー 5.10| Hotfix     | 2022/06/01 |           2027/01/31 | 8.1.0+<br />8.0.0+<br />7.4.0+  |   現在  |
| 5.10.0  | SQL Server 用 Microsoft PHP ドライバー 5.10| Production | 2022/01/31 |           2027/01/31 | 8.1.0+<br />8.0.0+<br />7.4.0+  |   有効  |
| 5.9.0   | SQL Server 用 Microsoft PHP ドライバー 5.9 | Production | 2021/01/30 |           2026/01/29 | 8.0.0+<br />7.4.0+<br />7.3.0+  | current |
| 5.8.1   | SQL Server 用 Microsoft PHP ドライバー 5.8 | Hotfix     | 2020/04/15 |           2025/01/31 | 7.4.0+<br />7.3.0+<br />7.2.1+  | current |
| 5.8.0   | SQL Server 用 Microsoft PHP ドライバー 5.8 | Production | 2020/01/31 |           2025/01/31 | 7.4.0+<br />7.3.0+<br />7.2.1+  |  valid  |
| 5.6.1   | SQL Server 用 Microsoft PHP ドライバー 5.6 | Hotfix     | 2019/03/19 |           2024/03/19 | 7.3.0+<br />7.2+<br />7.1.0+    | **終了** |
| 5.6.0   | SQL Server 用 Microsoft PHP ドライバー 5.6 | Production | 2019/02/21 |           2024/02/21 | 7.3.0+<br />7.2+<br />7.1.0+    | **終了** |
| 5.3.0   | SQL Server 用 Microsoft PHP ドライバー 5.3 | Production | 2018/07/20 |           2023/07/20 | 7.2+<br />7.1.0+<br />7.0.0+    | **終了** |
| 5.2.0   | SQL Server 用 Microsoft PHP ドライバー 5.2 | Production | 2018/03/23 |           2023/03/23 | 7.2+<br />7.1.0+<br />7.0.0+    | **終了** |
| 4.3.0   | SQL Server 用 Microsoft PHP ドライバー 4.3 | Production | 2017/07/06 |           2022/07/06 | 7.1.0+<br />7.0.0+              | **終了** |
| 4.0.8   | SQL Server 用 Microsoft PHP ドライバー 4.0 | Production | 2016/12/19 |           2021/12/19 | 7.0.0+                          | **終了** |
| 4.0     | SQL Server 用 Microsoft PHP ドライバー 4.0 | Production | 2016/07/11 |           2021/07/11 | 7.0.0+                          | **終了** |
| 3.2.0.0 | SQL Server 用 Microsoft PHP ドライバー 3.2 | Update     | 2015/03/09 |           2020/03/09 | 5.6.4+<br />5.5.16+<br />5.4.32 | **終了** |
| 3.1.0.0 | SQL Server 用 Microsoft PHP ドライバー 3.1 | Update     | 2014/12/12 |           2019/12/12 | 5.5.16+<br />5.4.32             | **終了** |
| 3.0.1   | SQL Server 用 Microsoft PHP ドライバー 3.0 | Update     | 2014/07/22 |           2019/07/22 | 5.4                             | **終了** |
| 3.0.0   | SQL Server 用 Microsoft PHP ドライバー 3.0 | Production | 2012/03/06 |           2017/03/06 | 5.4                             | **終了** |
| 2.0     | SQL Server 用 Microsoft PHP ドライバー 2.0 | Production | 2010/08/10 |           2015/08/10 | --                              | **終了** |
| 1.0     | SQL Server 用 Microsoft PHP ドライバー 1.0 | Production | 2009/04/28 |           2014/04/28 | --                              | **終了** |

* * *
