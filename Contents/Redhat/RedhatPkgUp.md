---
layout: default
title:  ":computer: Linux"
description: ":wrench: RedHat系コマンド・更新"
date: "2023/05/07"
lastmod: "2023/05/07"
---

## 1. アップデートできるパッケージのチェック  

### 1-1. アップデートできるパッケージの一覧表示  
アップデートできるパッケージの一覧を表示するには`dnf check-update`と入力し実行します。  
※下記の例では、Oracle Linux 8で実行しOracle Linux 8と表示されていますがご使用のディストリビューションに対応する項目が表示されると思います。  

```
[username@localhost ~]$ dnf check-update
Oracle Linux 8 BaseOS Latest (x86_64)            24 MB/s |  57 MB     00:02    
Oracle Linux 8 Application Stream (x86_64)       16 MB/s |  44 MB     00:02    
Latest Unbreakable Enterprise Kernel Release 7   20 MB/s |  14 MB     00:00    
メタデータの期限切れの最終確認: 0:00:02 時間前の 2023年05月07日 10時11分39秒 に実施しました。

NetworkManager.x86_64                1:1.40.0-6.0.1.el8_7      ol8_baseos_latest
NetworkManager-adsl.x86_64           1:1.40.0-6.0.1.el8_7      ol8_baseos_latest
NetworkManager-bluetooth.x86_64      1:1.40.0-6.0.1.el8_7      ol8_baseos_latest

・・・＜＜多いため省略＞＞・・・

zlib.x86_64                          1.2.11-21.el8_7           ol8_baseos_latest
パッケージの廃止
grub2-tools.x86_64                   1:2.02-142.0.3.el8_7.1    ol8_baseos_latest
    grub2-tools.x86_64               1:2.02-142.0.1.el8        @anaconda        
grub2-tools-efi.x86_64               1:2.02-142.0.3.el8_7.1    ol8_baseos_latest
    grub2-tools.x86_64               1:2.02-142.0.1.el8        @anaconda        
```

### 1-2. 個別に指定して更新パッチがあるかチェック  
例：rpmパッケージの更新パッチがあるかチェックする場合  
dnf check-updateコマンドに追加で`rpm`などのパッケージ名を入力し実行します。  

```
[username@localhost ~]$ dnf check-update rpm
メタデータの期限切れの最終確認: 0:03:12 時間前の 2023年05月07日 10時11分39秒 に実施しました。

rpm.x86_64                   4.14.3-24.el8_7                   ol8_baseos_latest

```

### 1-3. セキュリティ項目のみの更新パッチがあるかチェックする  
dnf check-updateコマンドにオプションで`--security`を追加で入力し実行します。  

```
[username@localhost ~]$ dnf check-update --security
メタデータの期限切れの最終確認: 0:06:25 時間前の 2023年05月07日 10時11分39秒 に実施しました。

bpftool.x86_64                         5.15.0-100.96.32.el8uek ol8_UEKR7        
buildah.x86_64                         1:1.27.3-1.module+el8.7.0+20930+90b24198
                                                               ol8_appstream    
cockpit-podman.noarch                  53-1.module+el8.7.0+20930+90b24198
                                                               ol8_appstream    
conmon.x86_64                          3:2.1.4-1.module+el8.7.0+20930+90b24198
                                                               ol8_appstream    
container-selinux.noarch               2:2.189.0-1.module+el8.7.0+20930+90b24198
                                                               ol8_appstream    

・・・＜＜多いため省略＞＞・・・

webkit2gtk3.x86_64                     2.36.7-1.el8_7.3        ol8_appstream    
webkit2gtk3-jsc.x86_64                 2.36.7-1.el8_7.3        ol8_appstream    
パッケージの廃止
grub2-tools.x86_64                     1:2.02-142.0.3.el8_7.1  ol8_baseos_latest
    grub2-tools.x86_64                 1:2.02-142.0.1.el8      @anaconda        
grub2-tools-efi.x86_64                 1:2.02-142.0.3.el8_7.1  ol8_baseos_latest
    grub2-tools.x86_64                 1:2.02-142.0.1.el8      @anaconda        
grub2-tools-extra.x86_64               1:2.02-142.0.3.el8_7.1  ol8_baseos_latest
    grub2-tools.x86_64                 1:2.02-142.0.1.el8      @anaconda        
```

<br />

## 2. パッケージのアップデート  
パッケージのアップデートを行うには`dnf update`を入力し実行します。  
また、パッケージのアップデートはrootアカウントなどのパッケージをアップデートできる権限を持ったアカウントでなければできません。  
権限を持っていないアカウントで実行すると以下のようなメッセージが出ます。  

```
[username@localhost ~]$ dnf update
エラー: このコマンドはスーパーユーザー特権(大概のシステムではrootユーザー)で実行しなければいけません。
```

よって、**sudo**コマンドを扱うことにします。  

### 2-1. セキュリティのみのアップデート  
オプションに`--security`を付けて実行します。  
まず、ダウンロード予定の一覧が表示され**yes/no**の判断を促されます。  

```
[username@localhost ~]$ sudo dnf update --security
[sudo] username のパスワード: ＜＜表示されませんが構わず入力＞＞
Oracle Linux 8 BaseOS Latest (x86_64)                       23 kB/s | 3.6 kB     00:00    
Oracle Linux 8 BaseOS Latest (x86_64)                       25 MB/s |  57 MB     00:02    
Oracle Linux 8 Application Stream (x86_64)                  52 kB/s | 3.9 kB     00:00    
Oracle Linux 8 Application Stream (x86_64)                  29 MB/s |  44 MB     00:01    
Latest Unbreakable Enterprise Kernel Release 7 for Oracle   25 kB/s | 3.0 kB     00:00    
依存関係が解決しました。
===========================================================================================
 パッケージ                         Arch   バージョン              リポジトリー      サイズ
===========================================================================================
インストール:
 kernel                             x86_64 4.18.0-425.19.2.el8_7   ol8_baseos_latest 8.9 M
アップグレード:
 bpftool                            x86_64 5.15.0-100.96.32.el8uek ol8_UEKR7         2.1 M
 buildah                            x86_64 1:1.27.3-1.module+el8.7.0+20930+90b24198
                                                                   ol8_appstream     8.1 M
 cockpit-podman                     noarch 53-1.module+el8.7.0+20930+90b24198
                                                                   ol8_appstream     547 k
 conmon                             x86_64 3:2.1.4-1.module+el8.7.0+20930+90b24198
                                                                   ol8_appstream      56 k
 container-selinux                  noarch 2:2.189.0-1.module+el8.7.0+20930+90b24198
                                                                   ol8_appstream      60 k
 containernetworking-plugins        x86_64 1:1.1.1-3.module+el8.7.0+20930+90b24198
                                                                   ol8_appstream      18 M

・・・＜＜多いので省略＞＞・・・

 webkit2gtk3                        x86_64 2.36.7-1.el8_7.3        ol8_appstream      19 M
 webkit2gtk3-jsc                    x86_64 2.36.7-1.el8_7.3        ol8_appstream     6.8 M
group/moduleパッケージをインストール:
 kernel-uek                         x86_64 5.15.0-100.96.32.el8uek ol8_UEKR7         1.4 M
依存関係のインストール:
 grub2-tools-efi                    x86_64 1:2.02-142.0.3.el8_7.1  ol8_baseos_latest 480 k
 kernel-core                        x86_64 4.18.0-425.19.2.el8_7   ol8_baseos_latest  41 M
 kernel-modules                     x86_64 4.18.0-425.19.2.el8_7   ol8_baseos_latest  33 M
 kernel-uek-core                    x86_64 5.15.0-100.96.32.el8uek ol8_UEKR7          52 M
 kernel-uek-modules                 x86_64 5.15.0-100.96.32.el8uek ol8_UEKR7          61 M

トランザクションの概要
===========================================================================================
インストール      7 パッケージ
アップグレード  115 パッケージ

ダウンロードサイズの合計: 742 M
これでよろしいですか? [y/N]: y
```

`y`を入力しエンターキーを押します。  
ダウンロードが開始します。

```
パッケージのダウンロード:
(1/122): grub2-tools-efi-2.02-142.0.3.el8_7.1.x86_64.rpm   3.3 MB/s | 480 kB     00:00    
(2/122): kernel-4.18.0-425.19.2.el8_7.x86_64.rpm            11 MB/s | 8.9 MB     00:00    
(3/122): kernel-uek-5.15.0-100.96.32.el8uek.x86_64.rpm     7.4 MB/s | 1.4 MB     00:00    
(4/122): kernel-core-4.18.0-425.19.2.el8_7.x86_64.rpm      5.6 MB/s |  41 MB     00:07    
(5/122): kernel-modules-4.18.0-425.19.2.el8_7.x86_64.rpm   3.8 MB/s |  33 MB     00:08    
(6/122): curl-7.61.1-25.el8_7.3.x86_64.rpm                 5.5 MB/s | 352 kB     00:00    

・・・＜＜多いので省略＞＞・・・

(116/122): tigervnc-license-1.12.0-9.el8_7.3.noarch.rpm    629 kB/s |  40 kB     00:00    
(117/122): tigervnc-server-minimal-1.12.0-9.el8_7.3.x86_64 3.6 MB/s | 1.1 MB     00:00    
(118/122): qemu-kvm-core-6.2.0-22.module+el8.7.0+21024+31a 2.1 MB/s | 3.4 MB     00:01    
(119/122): webkit2gtk3-2.36.7-1.el8_7.3.x86_64.rpm         7.3 MB/s |  19 MB     00:02    
(120/122): firefox-102.10.0-1.0.1.el8_7.x86_64.rpm         6.9 MB/s | 109 MB     00:15    
(121/122): bpftool-5.15.0-100.96.32.el8uek.x86_64.rpm      2.7 MB/s | 2.1 MB     00:00    
(122/122): webkit2gtk3-jsc-2.36.7-1.el8_7.3.x86_64.rpm     2.2 MB/s | 6.8 MB     00:03    
-------------------------------------------------------------------------------------------
合計                                                        21 MB/s | 742 MB     00:35     
Oracle Linux 8 BaseOS Latest (x86_64)                      3.0 MB/s | 3.1 kB     00:00    
GPG 鍵 0xXXXXXXXX をインポート中:
 Userid     : "Oracle OSS group (Open Source Software group) <build@oss.oracle.com>"
 Fingerprint: XXXX XXXX XXXX XXXX XXXX XXXX XXXX XXXX XXXX XXXX
 From       : /etc/pki/rpm-gpg/RPM-GPG-KEY-oracle
これでよろしいですか? [y/N]: y
```

ダウンロードが終了しアップデートを開始する**yes/No**が促されます。  
`y`を入力しエンターキーを押します。  
アップデート処理が開始しその後検証も行います。  

```
鍵のインポートに成功しました
トランザクションの確認を実行中
トランザクションの確認に成功しました。
トランザクションのテストを実行中
トランザクションのテストに成功しました。
トランザクションを実行中
  scriptletの実行中: linux-firmware-999:20230315-999.18.gitc761dbe8.el8.noarch         1/1 
  準備             :                                                                   1/1 
  scriptletの実行中: systemd-libs-239-68.0.2.el8_7.4.x86_64                            1/1 
  アップグレード中 : systemd-libs-239-68.0.2.el8_7.4.x86_64                          1/237 
  scriptletの実行中: systemd-libs-239-68.0.2.el8_7.4.x86_64                          1/237 
  アップグレード中 : openssl-libs-1:1.1.1k-9.el8_7.x86_64                            2/237 
  scriptletの実行中: openssl-libs-1:1.1.1k-9.el8_7.x86_64                            2/237 
  アップグレード中 : grub2-common-1:2.02-142.0.3.el8_7.1.noarch                      3/237 
  アップグレード中 : nss-util-3.79.0-11.el8_7.x86_64                                 4/237 
  アップグレード中 : libxml2-2.9.7-15.el8_7.1.x86_64                                 5/237 
  アップグレード中 : libtasn1-4.13-4.el8_7.x86_64                                    6/237 
  scriptletの実行中: libtasn1-4.13-4.el8_7.x86_64                                    6/237 

・・・＜＜多いので省略＞＞・・・

  検証             : webkit2gtk3-2.36.7-1.el8.x86_64                               233/237 
  検証             : webkit2gtk3-jsc-2.36.7-1.el8_7.3.x86_64                       234/237 
  検証             : webkit2gtk3-jsc-2.36.7-1.el8.x86_64                           235/237 
  検証             : bpftool-5.15.0-100.96.32.el8uek.x86_64                        236/237 
  検証             : bpftool-4.18.0-425.3.1.el8.x86_64                             237/237 

アップグレード済み:
  bpftool-5.15.0-100.96.32.el8uek.x86_64                                                   
  buildah-1:1.27.3-1.module+el8.7.0+20930+90b24198.x86_64                                  
  cockpit-podman-53-1.module+el8.7.0+20930+90b24198.noarch                                 
  conmon-3:2.1.4-1.module+el8.7.0+20930+90b24198.x86_64                                    
  container-selinux-2:2.189.0-1.module+el8.7.0+20930+90b24198.noarch                       
  containernetworking-plugins-1:1.1.1-3.module+el8.7.0+20930+90b24198.x86_64               

・・・＜＜多いので省略＞＞・・・

  webkit2gtk3-2.36.7-1.el8_7.3.x86_64                                                      
  webkit2gtk3-jsc-2.36.7-1.el8_7.3.x86_64                                                  
インストール済み:
  grub2-tools-efi-1:2.02-142.0.3.el8_7.1.x86_64                                            
  kernel-4.18.0-425.19.2.el8_7.x86_64                                                      
  kernel-core-4.18.0-425.19.2.el8_7.x86_64                                                 
  kernel-modules-4.18.0-425.19.2.el8_7.x86_64                                              
  kernel-uek-5.15.0-100.96.32.el8uek.x86_64                                                
  kernel-uek-core-5.15.0-100.96.32.el8uek.x86_64                                           
  kernel-uek-modules-5.15.0-100.96.32.el8uek.x86_64                                        

完了しました!
[username@localhost ~]$ 
```

### 2-2. 個別のパッケージを指定して更新  
例：rpmパッケージのみを個別に指定しアップデートする場合  
dnf updateコマンドに追加で`rpm`などのパッケージ名を入力し実行します。  

```
[username@localhost ~]$ sudo dnf update rpm
[sudo] username のパスワード: ＜＜表示されませんが構わず入力＞＞
メタデータの期限切れの最終確認: 0:10:07 時間前の 2023年05月07日 10時30分56秒 に実施しました。
依存関係が解決しました。
===========================================================================================
 パッケージ                     Arch       バージョン          リポジトリー          サイズ
===========================================================================================
アップグレード:
 python3-rpm                    x86_64     4.14.3-24.el8_7     ol8_baseos_latest     155 k
 rpm                            x86_64     4.14.3-24.el8_7     ol8_baseos_latest     543 k
 rpm-build-libs                 x86_64     4.14.3-24.el8_7     ol8_baseos_latest     157 k
 rpm-libs                       x86_64     4.14.3-24.el8_7     ol8_baseos_latest     345 k
 rpm-plugin-selinux             x86_64     4.14.3-24.el8_7     ol8_baseos_latest      78 k
 rpm-plugin-systemd-inhibit     x86_64     4.14.3-24.el8_7     ol8_baseos_latest      79 k

トランザクションの概要
===========================================================================================
アップグレード  6 パッケージ

ダウンロードサイズの合計: 1.3 M
これでよろしいですか? [y/N]: y
パッケージのダウンロード:
(1/6): python3-rpm-4.14.3-24.el8_7.x86_64.rpm              975 kB/s | 155 kB     00:00    
(2/6): rpm-build-libs-4.14.3-24.el8_7.x86_64.rpm           909 kB/s | 157 kB     00:00    
(3/6): rpm-plugin-selinux-4.14.3-24.el8_7.x86_64.rpm       2.6 MB/s |  78 kB     00:00    
(4/6): rpm-4.14.3-24.el8_7.x86_64.rpm                      2.6 MB/s | 543 kB     00:00    
(5/6): rpm-libs-4.14.3-24.el8_7.x86_64.rpm                 6.9 MB/s | 345 kB     00:00    
(6/6): rpm-plugin-systemd-inhibit-4.14.3-24.el8_7.x86_64.r 3.1 MB/s |  79 kB     00:00    
-------------------------------------------------------------------------------------------
合計                                                       5.7 MB/s | 1.3 MB     00:00     
トランザクションの確認を実行中
トランザクションの確認に成功しました。
トランザクションのテストを実行中
トランザクションのテストに成功しました。
トランザクションを実行中
  準備             :                                                                   1/1 
  アップグレード中 : rpm-libs-4.14.3-24.el8_7.x86_64                                  1/12 
  scriptletの実行中: rpm-libs-4.14.3-24.el8_7.x86_64                                  1/12 
  アップグレード中 : rpm-4.14.3-24.el8_7.x86_64                                       2/12 
  アップグレード中 : rpm-build-libs-4.14.3-24.el8_7.x86_64                            3/12 
  scriptletの実行中: rpm-build-libs-4.14.3-24.el8_7.x86_64                            3/12 
  アップグレード中 : python3-rpm-4.14.3-24.el8_7.x86_64                               4/12 
  アップグレード中 : rpm-plugin-selinux-4.14.3-24.el8_7.x86_64                        5/12 
  アップグレード中 : rpm-plugin-systemd-inhibit-4.14.3-24.el8_7.x86_64                6/12 
  整理             : python3-rpm-4.14.3-24.el8_6.x86_64                               7/12 
  整理             : rpm-build-libs-4.14.3-24.el8_6.x86_64                            8/12 
  scriptletの実行中: rpm-build-libs-4.14.3-24.el8_6.x86_64                            8/12 
  整理             : rpm-plugin-systemd-inhibit-4.14.3-24.el8_6.x86_64                9/12 
  整理             : rpm-plugin-selinux-4.14.3-24.el8_6.x86_64                       10/12 
  整理             : rpm-4.14.3-24.el8_6.x86_64                                      11/12 
  整理             : rpm-libs-4.14.3-24.el8_6.x86_64                                 12/12 
  scriptletの実行中: rpm-libs-4.14.3-24.el8_6.x86_64                                 12/12 
  検証             : python3-rpm-4.14.3-24.el8_7.x86_64                               1/12 
  検証             : python3-rpm-4.14.3-24.el8_6.x86_64                               2/12 
  検証             : rpm-4.14.3-24.el8_7.x86_64                                       3/12 
  検証             : rpm-4.14.3-24.el8_6.x86_64                                       4/12 
  検証             : rpm-build-libs-4.14.3-24.el8_7.x86_64                            5/12 
  検証             : rpm-build-libs-4.14.3-24.el8_6.x86_64                            6/12 
  検証             : rpm-libs-4.14.3-24.el8_7.x86_64                                  7/12 
  検証             : rpm-libs-4.14.3-24.el8_6.x86_64                                  8/12 
  検証             : rpm-plugin-selinux-4.14.3-24.el8_7.x86_64                        9/12 
  検証             : rpm-plugin-selinux-4.14.3-24.el8_6.x86_64                       10/12 
  検証             : rpm-plugin-systemd-inhibit-4.14.3-24.el8_7.x86_64               11/12 
  検証             : rpm-plugin-systemd-inhibit-4.14.3-24.el8_6.x86_64               12/12 

アップグレード済み:
  python3-rpm-4.14.3-24.el8_7.x86_64                                                       
  rpm-4.14.3-24.el8_7.x86_64                                                               
  rpm-build-libs-4.14.3-24.el8_7.x86_64                                                    
  rpm-libs-4.14.3-24.el8_7.x86_64                                                          
  rpm-plugin-selinux-4.14.3-24.el8_7.x86_64                                                
  rpm-plugin-systemd-inhibit-4.14.3-24.el8_7.x86_64                                        

完了しました!
[username@localhost ~]$ 
```

___
