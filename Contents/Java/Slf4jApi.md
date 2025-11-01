---
layout: default
title: ":page_with_curl: Oracle Java"
description: ":exclamation: Slf4J-apiを使用する"
date: "2023/04/15"
lastmod: "2023/04/15"
---

## 0. はじめに  
`slf4j-api.x.x.x.jar`を別途ライブラリが必要であり単独で使用すると以下のエラーメッセージが表示されます。  

```
SLF4J: No SLF4J providers were found.
SLF4J: Defaulting to no-operation (NOP) logger implementation
SLF4J: See https://www.slf4j.org/codes.html#noProviders for further details.
```

Slf4Jは、まだ良く分かっていませんが取り合えずエラーメッセージが出ないように対策します。  

<br />

## 1. 対策  
エラーメッセージに、URLがありましたので公式ページで確認してみます。  
[Slf4J noProviders](https://www.slf4j.org/codes.html#noProviders)  

> ### No SLF4J providers were found.  

> This warning, i.e. not an error, message is reported when no SLF4J providers could be found on the class path.  
> Placing one (and only one) of the many available providers such as slf4j-nop.jar slf4j-simple.jar, slf4j-reload4j.jar,  
> slf4j-jdk14.jar or logback-classic.jar on the class path should solve the problem.  

> In the absence of a provider, SLF4J will default to a no-operation (NOP) logger provider.  

> Please note that slf4j-api version 2.0.x and later use the [ServiceLoader](https://docs.oracle.com/javase/8/docs/api/java/util/ServiceLoader.html) mechanism.  
> `Earlier versions relied on the static binder mechanism which is no longer honored by slf4j-api.`  
> Please read the FAQ entry [What has changed in SLF4J version 2.0.0?](https://www.slf4j.org/faq.html#changesInVersion200) for further important details.  

> If you are responsible for packaging an application and do not care about logging, then placing slf4j-nop.jar on the class path of your application will get rid of this warning message.  
> Note that embedded components such as libraries or frameworks should not declare a dependency on any SLF4J providers but only depend on slf4j-api.  
> When a library declares a compile-time dependency on a SLF4J provider, it imposes that provider on the end-user, thus negating SLF4J's purpose.  

**日本語訳**  

> #### SLF4J プロバイダーが見つかりませんでした。  

> この警告 (エラーではない) メッセージは、クラスパスに SLF4J プロバイダーが見つからない場合に報告されます。  
> slf4j-nop.jar slf4j-simple.jar、slf4j-reload4j.jar、slf4j-jdk14.jarまたはlogback-classic.jarなどの
> 多くの使用可能なプロバイダーの1つ(および1つだけ)をクラスパスに配置すると、問題が解決するはずです。  

> プロバイダーがない場合、SLF4J はデフォルトで無操作 (NOP) ロガー プロバイダーになります。  

> slf4j-api バージョン 2.0.x 以降では ServiceLoader メカニズムを使用することに注意してください。  
> 以前のバージョンは、slf4j-api では受け入れられなくなった静的バインダー メカニズムに依存していました。  
> FAQ エントリ SLF4J バージョン 2.0.0 の変更点をお読みください。さらに重要な詳細については。  

> アプリケーションをパッケージ化する責任があり、ロギングを気にしない場合は、アプリケーションのクラス パスに slf4j-nop.jar を配置すると、この警告メッセージが表示されなくなります。  
> ライブラリやフレームワークなどの組み込みコンポーネントは、SLF4J プロバイダーへの依存を宣言するべきではなく、slf4j-api のみに依存することに注意してください。  
> ライブラリが SLF4J プロバイダーに対するコンパイル時の依存関係を宣言すると、そのプロバイダーがエンドユーザーに課され、SLF4J の目的が無効になります。  

よって、`slf4j-api-x.x.x.jar`とセットで追加で以下のいずれかが必要のようです。  
このライブラリが無いとエラーが表示されます。  

**slf4j-simple-x.x.x.jar**
**slf4j-nop-x.x.x.jar**  
**slf4j-reload4j.jar**  
**slf4j-jdk14.jarまたはlogback-classic.jar**  

※x.x.xまたはx.xはVersion番号が入り適応なものを入手してください。  

___
