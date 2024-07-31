---
title: macOSの新機能？ Sequoiaベータ版をインストールする方法
date: 2024-07-31T06:34:09.832Z
author: Daniel Kehoe
authorURL: https://www.freecodecamp.org/news/author/danielkehoe/
OriginalURL: https://www.freecodecamp.org/news/whats-new-in-macos-how-to-install-the-sequoia-beta/
Proofreader: ""

---

macOS Sequoiaのパブリックベータ版が公開されました。

<!-- more -->

macOS Sequoia (macOS 15) の最終リリースは2024年9月末から10月初めになる予定ですが、パブリックベータ版を先行してインストールする方法をご紹介します。日常的に使用するには十分安定しています。

macOS Sequoiaのパブリックベータ版は試したい人なら誰でも利用できますが、取得するには[Apple Beta Software Program][1]に登録する必要があります。

## 目次

1.  [macOS Sequoiaは安定しているか？][2]
2.  [インストールに必要な時間][3]
3.  [macOS Sequoiaの新機能][4]
4.  [macOS Sequoiaの特徴][5]
5.  [macOS Sequoiaの小さな変更点][6]
6.  [macOS Sequoiaの要件][7]
7.  [先にMacをバックアップする][8]
8.  [パブリックベータ版を取得するためにサインアップ][9]
9.  [macOSベータ版をどこにインストールするか][10]  
    – [予備のMacにインストール][11]  
    – [外部ドライブにインストール][12]  
    – [別のボリュームにインストール][13]
10.  [スタートアップマネージャを使用する][14]
11.  [macOSベータ版のアップデートを停止する][15]
12.  [macOS Sonomaに戻る][16]
13.  [次は何か][17]

## macOS Sequoiaは安定しているか？

現時点で、ユーザーはベータ版に少数の軽微な問題があると報告していますが、それでも「驚くほど安定している」とのことです。

外部モニターに関する問題や、サードパーティ製の外部デバイスに関する問題が予想されます。また、画面共有やビデオ会議（特にZoom）、ウェブブラウザーでのストリーミングにも問題があるかもしれません。

## インストールに必要な時間

macOS Sonoma から macOS Sequoia へのアップデートには1時間以上かかることがあります。時間は、アップデートのサイズ、インターネットの速度、Macの年式やパフォーマンスなど、さまざまな要因によって大きく異なります。

## macOS Sequoiaの新機能

ユーザーはmacOS Sequoiaが以前よりも高速で、ノートパソコンのバッテリー寿命も向上していると報告していますが、最終リリースを見るまでは確信できません。

[macOS Sequoia][18]に注目すると、これはオペレーティングシステムの大規模なオーバーホールではないことが分かります。最も便利な機能はウィンドウタイルと新しいパスワードアプリケーション、iPhoneミラーリング、デバイス間のシームレスなドラッグ＆ドロップです。

私は別の記事で[SonomaとSequoiaの比較][19]をし、さらに[macOS Sequoiaにアップデートすべきか？][20]という質問に対するアドバイスも提供しています。

## macOS Sequoiaの特徴

![mac-passwords-app](https://www.freecodecamp.org/news/content/images/2024/07/mac-passwords-app.png)

macOS Sequoia パスワードアプリケーション

### パスワードマネージャ

MacOS Sequoiaには「Passwords」という新しいアプリが追加され、ユーザーがログイン認証情報を管理する方法が改善されました。

Appleの既存のKeychainフレームワークに基づいて、このアプリはパスワード、パスキー、Wi-Fiパスワード、その他の重要な認証情報を1つの安全な集中場所に統合します。

以前はシステム設定で認証情報を編集できましたが、それらは深く埋もれて見つけにくいものでした。新しいPasswordsアプリは、1Password、LastPass、Bitwardenなどのサードパーティ製のパスワードマネージャを使用する必要性を大幅に削減します。

![mac-sequoia-tiling](https://www.freecodecamp.org/news/content/images/2024/07/mac-sequoia-tiling.png)

macOS Sequoia ウィンドウタイル

### ウィンドウタイル

長年、WindowsユーザーはMacOSにタイルウィンドウマネージャがないことを不満に思っていました。MacOS Sequoiaには「Window Tiling」という新機能が追加され、ウィンドウを画面の端にドラッグして並べることができるようになりました。サードパーティのユーティリティにはもっと多くの機能がありますが、組み込みのWindow Tilingは歓迎すべき追加です。

これらの2つの機能でアップグレードする価値があります。さらに、Appleは他の機能も発表しました。

### iPhoneミラーリング

この機能により、iPhoneアプリをmacOSウィンドウ内で使用できます。ユーザーはMac上でiPhoneの通知を直接確認でき、MacをiPhoneの拡張として利用できます。

あるユーザーは、「家でMacの前に座っているときに通知を確認するために電話を探す必要がない」と述べています。

### デバイス間のシームレスなドラッグ＆ドロップ

この機能により、iPhoneとMac間でファイルを転送する際の信頼性が向上します。AirDropに関する問題を解決します。「MacからiPhoneアプリへのファイル転送に5つ以上の手間のかかるステップが必要なくなった」とユーザーは述べています。

### Apple Inspector (AI機能)

MacOS Sequoiaでは、AppleのAIイニシアチブであるApple Intelligenceの最初の使用が導入されます。Apple Intelligenceは、Appleのカスタムシリコンを活用し、ローカルおよびクラウドベースの処理の新しいシステムレベルの機能を提供します。

これは、将来的にAIがより多くのアプリケーションに組み込まれることで進展する見通しですが、macOS SequoiaではSiriの改善が見られるかもしれません。これらの機能は、IntelベースのMacにmacOS Sequoiaをインストールした場合には利用できません。

## macOS Sequoiaの小さな変更点

-   **システム設定:** 個々のメニューが再配置され、頻繁に使用されるメニューに迅速にアクセスできるようになりました。
-   **Safari:** ウェブブラウザはページ読み込み時間が速くなり、新しいスタートページと、iOSの「コンパクトモード」に似た新しい統合メニューが追加されました。ウェブサイトを要約し、関連情報をハイライトします。
-   **ノート:** 折りたたみセクションやハイライトスタイルの選択など、微小な改善が含まれます。また、ライブ音声の書き起こしや数学の式のサポートも追加されました。
-   **ビデオ会議:** プレゼンテーションや画面共有中に共有内容をプレビューします。さらに、macOSのビデオフィードに背景置換が組み込まれているため、Zoomや他の会議アプリで背景置換を使用する必要がありません。



[macOSのバージョンを確認][21] し、Sonoma (macOS 14) へアップデートしてください。その後、macOS Sequoiaベータ版をインストールします。

現在のmacOS SonomaをそのままMacに保持しておくことをお勧めします。ベータ版で問題が発生した場合に備えてです。したがって、macOS Sequoiaベータ版は別のボリューム、外付けドライブ、またはサブMacにインストールしてください。

また、macOS Sequoiaは古いIntelベースのMacでも動作しますが、遅くなる可能性があります。そのため、M1、M2、M3のApple Siliconチップを搭載したMacにインストールすることをお勧めします。

macOS Sequoiaベータ版は、Intel Amber Lakeチップの2018–2019年モデルのMacBook Airを除き、macOS Sonomaが動作するすべてのコンピュータにインストールできます。Appleは[macOS Sequoiaのサポート対象モデル一覧][23]を提供しています。

## Macのバックアップを取る

新しく購入した未使用のMacがある場合は、ファイルのバックアップは不要です。また、多くの開発者と同様に、重要なファイルをクラウドに保存している場合もバックアップは不要です。

そうでない場合、コンピュータ上に重要なファイルがある場合は、macOSベータ版をインストールする前にMacのバックアップを必ず取りましょう。

## パブリックベータ版を取得するためのサインアップ

Appleはパブリックベータ版と開発者ベータ版の両方を提供しています。最初にリリースされる開発者ベータ版はアプリケーションの互換性をテストするためのもので、数週間後により安定してバグの少ないパブリックベータ版がリリースされます。

![macOS Sequoia Public Beta](https://www.freecodecamp.org/news/content/images/2024/07/apple-beta-program.png)

パブリックベータ版は現在無料で提供されています。パブリックベータ版を取得するには、[Apple Beta Software Program][24]ウェブサイトでサインアップしてください。Apple IDでサインアップすると、システム設定にベータアップデートが利用可能であることが表示されます。

## macOSベータ版のインストール場所

予備のMacがある場合は、そこにmacOSベータ版をインストールするのが最良の選択です。できれば、Apple Silicon M1、M2、M3チップを搭載した比較的新しいMacが理想です。古いMacの場合は、コンピュータが遅くなる可能性があるため、ベータ版を避けることを検討してください。

予備のMacにインストールすることで、日常の生産性に影響を与えることなく新しいmacOSを試すことができます。

あるいは、Macの別のボリュームにmacOSベータ版をインストールすることもできます。これにより、試したいときにベータ版にブートできます。

外付けドライブにベータ版をインストールすることもできます。いずれの場合も、電源ボタンを押し続けて起動マネージャメニューを表示させ、デフォルトの起動ディスク以外のものを選択する必要があります。

ここでは、予備のMac、外付けドライブ、または別のボリュームにmacOS Sequoiaベータ版をインストールする手順を説明します。

### 予備のMacにインストールする

macOS Sonomaを実行しているMacにmacOS Sequoiaベータ版をインストールする方法を以下に示します。

1. `システム設定`を開き、`一般`および`ソフトウェアアップデート`に移動します。
2. `ベータアップデート`の`丸i`情報ボタンをクリックします。
3. `ベータアップデート`を`macOS Sequoia Public Beta`に設定します。
4. `完了`をクリックすると、Macはソフトウェアアップデートをチェックします。
5. チェックが完了すると、アップグレード名と`今すぐアップグレード`ボタンが表示されます。
6. ソフトウェアアップデートには少なくとも20%のバッテリーパワーが必要です。バッテリーが少ない場合は、電源に接続する必要があります。
7. パスワードを入力してソフトウェアアップデートを開始します。高速なインターネット接続の場合、ダウンロードには約30分かかります。ダウンロード後、`準備`プロセスは約15分かかります。
8. インストールが完了すると、Macは再起動します。Appleロゴと進行状況バーが表示されます。インストールプロセスには、自動再起動を含めて約15分かかります。
9. インストールが完了すると、ログイン画面が表示されます。Macのパスワード、次にApple IDのパスワードを入力し、さまざまな契約や設定を`続行`または`後で設定`します。
10. macOS Sequoiaのデスクトップが表示され、フィードバックアシスタントアプリケーションが開きます。フィードバックアシスタントを使用して、バグや問題を報告してください。
11. `このMacについて`を確認して、macOS 15が実行されていることを確認します。

`macOS Sequoia Public Beta`オプションが`ベータアップデート`で表示されない場合は、[Apple Beta Software Program][25]にサインアップしてください。Apple IDでサインアップすると、システム設定にベータアップデートが利用可能であることが表示されます。

### 外付けドライブにインストールする

クラウドストレージが普及している現在、外付けドライブを所有しているユーザーは少ないですが、外付けドライブをお持ちの場合はそこにmacOSベータ版をインストールできます。

ドライブをフォーマットする必要があるため、すでにドライブにあるファイルをすべて消去する必要があります。オペレーティングシステムの利用には、USB-CまたはThunderbolt接続の高速SSDドライブを所有しているのが望ましいです。USBメモリを使用することもできますが、少なくとも32GBの空き容量が必要です。

#### 外付けドライブのフォーマット方法

1. 外付けドライブをMacに接続します。
2. Spotlightで検索して`ディスクユーティリティ`を開きます。
3. 左側のサイドバーで外付けドライブを選択します。
4. `消去`をクリックしてドライブを再フォーマットします。
5. ドライブに`macOS Sequoia`などの名前を付けます。
6. `Mac OS拡張（ジャーナリング）`をフォーマットとして選択します。
7. `GUIDパーティションマップ`をスキームとして選択します。
8. `消去`をクリックしてドライブをフォーマットします。
9. ドライブのフォーマットが完了したら、`ディスクユーティリティ`を閉じます。

`*.pkg`ファイルをダウンロードして外付けドライブにインストールする必要があります。macOSベータのインストーラー`*.pkg`ファイルへのリンクを提供するサイトはいくつかあります。以下を確認してください:

-   [betaprofiles.dev][26]
-   [mrmacintosh.com][27]

最新の`InstallAssistant.pkg`をダウンロードしてください。これらのファイルは非常に大きく（14GB以上）、高速なインターネット接続でもダウンロードに30分以上かかることがあります。

#### macOS Sequoiaベータをインストールする方法

`InstallAssistant.pkg`ファイルをダブルクリックしてインストールを開始します。「インストール場所を変更」をクリックして外付けドライブを選択します。「インストール先を選択」ステップでは、インストール先として外付けドライブを選択できます。

### 別のボリュームにインストール

macOSベータを別のボリュームにインストールしたい場合は、以下の手順に従ってください。このプロセスは「デュアルブート」や「別パーティション」インストールと呼ばれることがあります。AppleのAPFSファイルシステムは「ボリューム」を導入しており、これはパーティションのようなものですが、より柔軟です。

MacにmacOS Sonoma用のボリュームとmacOS Sequoia用のボリュームの2つが存在することになります。起動マネージャを使ってどちらのボリュームから起動するかを選択できます。

#### 新しいボリュームを作成する方法

1.  Spotlightで検索して`ディスクユーティリティ`を開きます。
2.  左サイドバーで内部ドライブを選択します。
3.  上部バーの`+`ボタンをクリックして新しいボリュームを追加します（メニューの「編集」>「APFSボリュームを追加」）。
4.  ボリュームに`macOS Sequoia`など任意の名前を付けます。
5.  フォーマットを選択します（一般的には「APFS」）。
6.  `追加`をクリックしてボリュームを作成します。
7.  ボリュームの作成が完了したら「完了」をクリックして`ディスクユーティリティ`を閉じます。

#### macOS Sequoiaベータを入手する

別のボリュームにインストールするための`*.pkg`ファイルをダウンロードする必要があります。macOSベータのインストーラー`*.pkg`ファイルへのリンクを提供するサイトはいくつかあります。以下を確認してください:

-   [betaprofiles.dev][28]
-   [mrmacintosh.com][29]

最新の`InstallAssistant.pkg`をダウンロードしてください。これらのファイルは非常に大きく（14GB以上）、高速なインターネット接続でもダウンロードに30分以上かかることがあります。

#### macOS Sequoiaベータをインストールする

`InstallAssistant.pkg`ファイルをダブルクリックしてインストールを開始します。「インストール場所を変更」をクリックして、作成したボリュームを選択します。「インストール先を選択」ステップでは、新しいボリュームをインストール先として選択できます。

### スタートアップマネージャを使用する

Macの起動時に電源ボタンを押し続けてスタートアップマネージャに入ります。「起動オプションを読み込んでいます」と表示されます。内部ドライブ、外部ドライブ（接続されている場合）、ディスクボリューム、または「オプション」から起動する選択肢があります。

起動する外付けドライブまたはボリュームを選択します。`システム設定` > `起動ディスク`で外付けドライブまたはボリュームのデフォルトを設定できます。

## macOSベータのアップデートを停止する

macOS Sequoiaベータの使用を続けたくない場合は、ベータアップデートをオフにできます。

`システム設定` > `一般` > `ソフトウェアアップデート`に移動します。`ベータアップデート`の情報ボタン「丸I」をクリックし、`ベータアップデート`を`オフ`に設定します。これでmacOSベータのアップデートが停止します。

これはmacOSベータを使用したくない場合に必須のステップです。これを行わないと、Macが最新のベータバージョンに更新され続けます。

## macOS Sonomaに戻る

外部ドライブまたは別のボリュームを使用してmacOSベータを実行している場合、内部ドライブのプライマリボリュームとしてmacOS SonomaがMacに残っています。macOSベータを使用しない場合は、外部ドライブを再フォーマットするか、ボリュームを削除します。

## 予備のMac上でmacOS Sonomaを復元する

予備のMacでmacOS Sequoiaを使用している場合、macOS Sonomaを再インストールすることで復元できます。

Mac App StoreからmacOS Sonomaをダウンロードしてインストールできます。Mac App Storeで「macOS Sonoma」を検索するか、[macOS Sonoma][30]のリストを見るためのリンクを使用します。「取得」をクリックすると、App Storeが`システム設定` > `一般` > `ソフトウェアアップデート`を開き、macOS Sonomaのダウンロードを開始します。

App Storeからのダウンロードは遅いため、1時間以上の待ち時間が発生する可能性があります。App Storeは`アプリケーション`フォルダに`macOS Sonomaをインストール`アプリケーションをインストールします。

ダウンロードが完了すると、`macOS Sonomaをインストール`アプリケーションが自動的に起動します。指示に従ってmacOS Sonomaをインストールします。

また、直接インストーラー`*.pkg`ファイルをダウンロードしてmacOS Sonomaを復元することもできます。ダウンロードはApp Storeよりも速いです。確認してください:

-   [mrmacintosh.com][31]

`InstallAssistant.pkg`ファイルをダブルクリックしてインストールを開始します。

## 次に何をすべきか

macOS Sequoiaをインストールした後、[Macの設定][32]、特に[Macの名前設定][33]、[Dockの設定][34]、[Finderの設定][35]について推奨事項があります。

Macでソフトウェアを開発するために以下が必要です:

-   足りないコマンドラインツールのために[Xcodeコマンドラインツールをインストール][36]
-   パッケージマネージャとして[Homebrewをインストール][37]
-   バージョン管理のために[Gitをインストール][38]

macOSを更新するとき、新しいソフトウェアもインストールしたいかもしれません。以下はmacOS Sequoia向けの新しい推奨アプリケーションです:

-   [ターミナル][39]代替
-   [テキストエディタ][40]オプション
-   ChatGPTの使いやすさ向上のための[ChatGPTデスクトップアプリケーション][41]

## 結論

2024年10月以降、バグの修正、セキュリティ、およびソフトウェアの互換性を維持するため、特にソフトウェア開発者である場合は、macOSをSonomaからSequoiaに更新する必要があります。

macOS Sequoia は劇的な変化をもたらさないものの、Window Tiling や Passwords アプリなどの新機能は便利です。

macOS のベータ版をインストールするのには1時間以上かかりますが、日常使用に耐える安定性があると感じるかもしれません。今すぐ新しい機能を利用できます。

[1]: https://beta.apple.com/
[2]: #is-macos-sequoia-stable
[3]: #time-needed-to-install
[4]: #whats-new-in-macos-sequoia
[5]: #new-features-in-macos-sequoia
[6]: #small-changes-in-macos-sequoia
[7]: #requirements-for-macos-sequoia
[8]: #back-up-your-mac-first
[9]: #sign-up-to-get-the-public-beta
[10]: #where-to-install-the-macos-beta
[11]: #install-on-a-spare-mac
[12]: #install-on-an-external-drive
[13]: #install-on-a-separate-volume
[14]: #use-the-startup-manager
[15]: #halt-macos-beta-updates
[16]: #return-to-macos-sonoma
[17]: #whats-next
[18]: https://mac.install.guide/macos/sequoia
[19]: https://mac.install.guide/macos/sonoma-vs-sequoia
[20]: https://mac.install.guide/macos/should-i-update
[21]: https://mac.install.guide/macos/check-version
[22]: https://mac.install.guide/macos/update
[23]: https://www.apple.com/macos/macos-sequoia-preview/
[24]: https://beta.apple.com/
[25]: https://beta.apple.com/
[26]: https://betaprofiles.dev/install/macos-15/
[27]: https://mrmacintosh.com/macos-sequoia-full-installer-database-download-directly-from-apple/
[28]: https://betaprofiles.dev/install/macos-15/
[29]: https://mrmacintosh.com/macos-sequoia-full-installer-database-download-directly-from-apple/
[30]: https://apps.apple.com/us/app/macos-sonoma/id6450717509
[31]: https://mrmacintosh.com/macos-sonoma-full-installer-database-download-directly-from-apple/
[32]: https://mac.install.guide/mac-setup/
[33]: https://mac.install.guide/mac-setup/name
[34]: https://mac.install.guide/mac-setup/dock
[35]: https://mac.install.guide/mac-setup/finder
[36]: https://mac.install.guide/commandlinetools/3
[37]: https://mac.install.guide/homebrew/3
[38]: https://mac.install.guide/git/
[39]: https://mac.install.guide/download/terminal
[40]: https://mac.install.guide/download/text-editor
[41]: https://mac.install.guide/download/chatgpt
[42]: https://mac.install.guide/macos/beta

