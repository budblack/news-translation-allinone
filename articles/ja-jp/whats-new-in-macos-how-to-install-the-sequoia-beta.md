---
title: macOSの新機能とは？Sequoiaベータ版のインストール方法
date: 2024-07-31T06:34:09.832Z
author: Daniel Kehoe
authorURL: https://www.freecodecamp.org/news/author/danielkehoe/
OriginalURL: https://www.freecodecamp.org/news/whats-new-in-macos-how-to-install-the-sequoia-beta/
Proofreader: ""

---

macOS Sequoiaのパブリックベータ版が利用可能になりました。

<!-- more -->

macOS Sequoia (macOS 15) の最終リリースは2024年9月下旬から10月上旬にかけての予定ですが、一足先にパブリックベータ版をインストールする方法をご紹介します。実際には日常使用に耐えうるほど安定しています。

macOS Sequoiaのパブリックベータ版は、試してみたい人なら誰でも入手可能ですが、[Apple Beta Software Program][1]に登録する必要があります。

## 目次

1.  [macOS Sequoiaは安定している？][2]
2.  [インストールにかかる時間][3]
3.  [macOS Sequoiaの新機能][4]
4.  [macOS Sequoiaの機能][5]
5.  [macOS Sequoiaの小さな変更][6]
6.  [macOS Sequoiaの要件][7]
7.  [まずMacをバックアップする][8]
8.  [パブリックベータを取得するためのサインアップ][9]
9.  [macOSベータ版のインストール場所について][10]  
    – [予備のMacにインストールする][11]  
    – [外付けドライブにインストールする][12]  
    – [別のボリュームにインストールする][13]
10.  [スタートアップマネージャを使用する][14]
11.  [macOSベータ版の更新を停止する][15]
12.  [macOS Sonomaに戻る][16]
13.  [次に期待すること][17]

## macOS Sequoiaは安定している？

現在のところ、ユーザーからはベータ版に関していくつかの軽微な問題のみが報告されています。彼らはベータ版は「驚くほど安定している」と言います。

外部モニターに関する問題の報告があり、外部のサードパーティデバイスに関しても問題が予想されます。また、画面共有、ビデオ会議（特にZoom）、またはウェブブラウザでのストリーミングにも問題があるかもしれません。

## インストールにかかる時間

macOS SonomaからmacOS Sequoiaへの更新は1時間以上かかることがあります。必要な時間は、更新のサイズ、インターネットの速度、およびMacの年齢とパフォーマンスなどの要因によって大きく異なります。

## macOS Sequoiaの新機能

macOS Sequoiaはユーザーにより、ラップトップでのバッテリー寿命が向上し、より高速になると報告されていますが、最終リリースを見ないと確信は持てません。

[macOS Sequoia][18]を詳しく見ると、これはオペレーティングシステムの大きなオーバーホールではないことが明らかです。最も有用な機能は、ウィンドウタイル管理、新しいパスワードアプリケーション、iPhoneのミラーリング、およびデバイス間のシームレスなドラッグアンドドロップです。

別の記事で[Sonoma vs Sequoia][19]を比較し、また[macOS Sequoiaにアップデートするべきか？][20]という質問へのアドバイスも提供しています。

## macOS Sequoiaの機能

![mac-passwords-app](https://www.freecodecamp.org/news/content/images/2024/07/mac-passwords-app.png)

macOS Sequoia パスワードアプリケーション

### パスワードマネージャー

MacOS SequoiaにはPasswordsと呼ばれる新しいアプリが追加され、ユーザーがログイン情報を管理する方法が改良されました。

AppleのKeychainの既存フレームワークを基に、このアプリはパスワード、パスキー、Wi-Fiパスワード、その他の重要な資格情報を一つの安全な、集中管理された場所にまとめます。

以前はシステム設定で編集できましたが、深く埋もれていて見つけにくかったです。新しいPasswordsアプリは、1Password、LastPass、Bitwardenなどのサードパーティのパスワードマネージャーを使う必要性を大幅に減少させます。

![mac-sequoia-tiling](https://www.freecodecamp.org/news/content/images/2024/07/mac-sequoia-tiling.png)

macOS Sequoia ウィンドウタイル

### ウィンドウタイル

長年にわたり、WindowsユーザーはMacOSにはタイルウィンドウ管理が欠けていると不満を述べてきました。MacOS Sequoiaでは、ウィンドウを画面の端にドラッグすることで並べて配置する新機能が追加されます。上下左右、またはグリッド配置が可能です。サードパーティのユーティリティにはより多くの機能がありますが、組み込みのウィンドウタイルは歓迎すべき追加です。

これらの二つの機能は、アップグレードする価値があります。さらに、Appleは他の機能も発表しています。

### iPhoneミラーリング

この機能により、macOSウィンドウ内でiPhoneアプリを使用できるようになります。ユーザーはMac上で直接iPhoneの通知を確認できるため、MacがiPhoneの拡張機能になります。

あるユーザーは、「もう家でMacの前に座ってiPhoneの通知を確認するためだけにiPhoneを探す必要がなくなった」と述べています。

### デバイス間のシームレスなドラッグアンドドロップ

この機能は、iPhoneとMac間のファイル転送の信頼性を向上させ、AirDropの問題に対処します。「MacからiPhoneアプリへのファイル転送にはもはや面倒な5つ以上のステップは必要ありません」とユーザーが述べています。

### Apple インテリジェンス

MacOS Sequoiaは、AppleのAIイニシアチブであるApple Intelligenceの初使用を導入します。Apple Intelligenceは新しいシステムレベルの機能を含んでおり、Appleのカスタムシリコンを使用してローカルとクラウドベースの処理を行います。

これは、AIがより多くのアプリケーションに統合される未来の可能性がありますが、macOS SequoiaでSiriの改善を目にすることができるかもしれません。ただし、これらの機能はIntelベースのMacにmacOS Sequoiaをインストールした際には存在しないことに注意してください。

## macOS Sequoiaの小さな変更

-   **システム設定:** 頻繁に使用するメニューに迅速にアクセスするために、個々のメニューが再配置されました。
-   **Safari:** ウェブブラウザはより速いページロード時間、新しいスタートページ、およびiOSの「コンパクトモード」に似た新しい統合メニューを備えています。ウェブサイトを要約し、関連情報を強調表示することができます。
-   **メモ:** 折りたたみセクションやハイライトスタイルの選択などの小さな改善。さらに、メモにはライブ音声転写と数学の式のサポートが追加されました。
-   **ビデオ会議:** プレゼンテーションや画面共有のためにビデオ通話で共有する内容をプレビューすることができます。また、背景の置き換えがmacOSのビデオフィードに組み込まれているため、Zoomやその他の会議アプリで背景置き換えを使用する必要はありません。

[あなたのmacOSバージョンを確認する][21] し、macOS Sequoiaベータ版をインストールする前にSonoma（macOS 14）に[macOSを更新してください][22]。

macOS SonomaをMacに保持しておくことをお勧めします。ベータ版で問題が発生した場合に備えるためです。つまり、macOS Sequoiaベータ版を別のボリューム、外部ドライブ、またはセカンダリのMacにインストールする必要があります。

また、macOS Sequoiaは古いIntelベースのMacでも動作しますが、遅くなる可能性があります。そのため、M1、M2、またはM3のApple Siliconチップを搭載したMacにのみインストールすることをお勧めします。

macOS Sequoiaベータ版は、Intel Amber Lakeチップを搭載した2018–2019年のMacBook Airモデルを除く、macOS Sonomaを実行する任意のコンピュータにインストールできます。Appleは[macOS Sequoiaのサポートされているモデルのリスト][23]を提供しています。

## Macをバックアップする

新しいMacを使用している場合、ファイルのバックアップは不要です。また、多くの開発者と同じように、重要なファイルをクラウドに保存している場合はバックアップは必要ありません。

それ以外の場合、コンピュータに重要なファイルがある場合は、macOSベータ版をインストールする前にMacのバックアップを確保してください。

## 公開ベータ版を登録する

Appleは公開ベータ版と開発者ベータ版の両方を提供しています。開発者ベータ版は最初にリリースされ、アプリケーションの互換性をテストすることを目的としています。公開ベータ版は数週間後にリリースされ、開発者ベータ版よりも安定していてバグが少ないです。

![macOS Sequoia Public Beta](https://www.freecodecamp.org/news/content/images/2024/07/apple-beta-program.png)

公開ベータ版は無料で利用可能です。Apple Beta Software Programの[ウェブサイトで登録][24]してください。Apple IDでサインアップすると、システム設定にベータ更新が表示されます。

## macOSベータ版をインストールする場所

余分なMacがある場合、ベストなオプションはそのマシンにmacOSベータ版をインストールすることです。理想的には、Apple SiliconのM1、M2、またはM3チップを搭載した比較的新しいMacを持っていることが望ましいです。古いMacしか持っていない場合、そのバージョンがコンピュータを遅くする可能性があるため、ベータ版を避けることをお勧めします。

予備のMacにインストールすることで、日常の生産性に影響を与えることなく新しいmacOSバージョンを試すことができます。

また、Macで別のボリュームにmacOSベータ版をインストールすることもできます。これにより、試したいときにベータ版を起動できます。

ベータ版を外部ドライブにインストールすることもできます。いずれの場合も、電源ボタンを押し続けて起動マネージャーメニューを表示し、デフォルトのスタートアップディスクの代わりに選択できるようにします。

予備のMac、外部ドライブ、または別のボリュームにmacOS Sequoiaベータ版をインストールする手順は以下の通りです。

### 予備のMacにインストール

macOS Sonomaを実行しているMacにmacOS Sequoiaベータ版をインストールする方法は次の通りです。

1.  `システム設定`を開き、`一般`および`ソフトウェアアップデート`に移動します。
2.  `ベータ更新`の「円形のI」情報ボタンをクリックします。
3.  `ベータ更新`を`macOS Sequoia Public Beta`に設定します。
4.  「完了」をクリックすると、Macがソフトウェアアップデートを確認します。
5.  確認後、アップグレード名が「今すぐアップグレード」ボタンと共に表示されます。
6.  ソフトウェアの更新には少なくとも20％のバッテリー電力が必要なため、バッテリーが少ない場合は電源に接続する必要があります。
7.  パスワードを入力してソフトウェア更新を開始します。高速インターネット接続があれば、ダウンロードには約30分かかります。ダウンロード後、「準備」プロセスには約15分かかります。
8.  インストールが完了すると、Macが再起動し、Appleロゴと進行状況バーが表示されます。インストールプロセスには、数回の自動再起動を含めて約15分かかります。
9.  インストールが完了すると、ログイン画面が表示されます。Macのパスワード、次にApple IDのパスワードを入力し、各種の同意や設定を「続ける」または「後で設定」を選択してください。
10.  macOS Sequoiaデスクトップが表示され、フィードバックアシスタントアプリケーションが開きます。フィードバックアシスタントを使用して、バグや問題を報告してください。
11.  `このMacについて`を確認して、macOS 15が実行されていることを確認します。

`ベータ更新`に`macOS Sequoia Public Beta`オプションが表示されない場合は、[Apple Beta Software Program][25]にサインアップしてください。Apple IDでサインアップすると、システム設定にベータ更新が表示されます。

### 外部ドライブにインストール

クラウドストレージが人気となった現在では、外部ドライブを所有しているユーザーはあまりいないかもしれません。しかし、外部ドライブを持っている場合は、そこにmacOSベータ版をインストールすることができます。

ドライブをフォーマットする必要があるため、既存のファイルはすべて消去されます。オペレーティングシステムで使用するための高速SSDドライブ（USB-CまたはThunderbolt接続）が最適です。USBサムドライブを使用することもできますが、32GB以上のスペースが必要です。

#### 外部ドライブをフォーマットする方法

1.  外部ドライブをMacに接続します。
2.  Spotlightで検索し、`ディスクユーティリティ`を開きます。
3.  左側のサイドバーで外部ドライブを選択します。
4.  `消去`をクリックしてドライブを再フォーマットします。
5.  ドライブに名前を付けます。例：`macOS Sequoia` 。
6.  フォーマットとして`Mac OS拡張（ジャーナリング）`を選択します。
7.  スキームとして`GUIDパーティションマップ`を選択します。
8.  `消去`をクリックしてドライブをフォーマットします。
9.  ドライブのフォーマットが完了したら、`ディスクユーティリティ`を閉じます。

`*.pkg` ファイルをダウンロードし、外付けドライブにインストールする必要があります。いくつかのサイトでは、macOS ベータ版のインストーラー `*.pkg` ファイルへのリンクを提供しています。以下を確認してください：

-   [betaprofiles.dev][26]
-   [mrmacintosh.com][27]

最新の `InstallAssistant.pkg` をダウンロードしてください。これらのファイルは非常に大きく (14GB 以上)、高速なインターネット接続でもダウンロードに30分以上かかることがあります。

#### macOS Sequoia ベータをインストールする方法

`InstallAssistant.pkg` ファイルをダブルクリックしてインストールを開始します。"インストール場所の変更" をクリックして、外付けドライブを選択します。"インストール先の選択" ステップでは、インストール先として外付けドライブを選択できます。

### 別のボリュームにインストールする

macOS ベータを別のボリュームにインストールしたい場合は、以下の手順に従ってください。この方法は "デュアルブート" や "別パーティション" と呼ばれることがあります。Apple の APFS ファイルシステムは、パーティションに似ていますが、より柔軟な "ボリューム" を導入しました。

Mac には2つのボリュームができます。1つは macOS Sonoma 用、もう1つは macOS Sequoia 用です。スタートアップマネージャーを使用して、どのボリュームから起動するかを選択できます。

#### 新しいボリュームを作成する方法

1.  Spotlight で検索して `ディスクユーティリティ` を開きます。
2.  左側のサイドバーで内部ドライブを選択します。
3.  上部バーの `+` ボタンをクリックして新しいボリュームを追加します (またはメニューの "編集" > "APFS ボリュームを追加")。
4.  ボリュームに `macOS Sequoia` などの名前を付けます。
5.  フォーマットを選択します (通常は "APFS")。
6.  `追加` をクリックしてボリュームを作成します。
7.  ボリュームの作成が完了したら "完了" をクリックし、`ディスクユーティリティ` を閉じます。

#### macOS Sequoia ベータを取得する

`*.pkg` ファイルをダウンロードして、別のボリュームにインストールする必要があります。いくつかのサイトでは、macOS ベータ版のインストーラー `*.pkg` ファイルへのリンクを提供しています。以下を確認してください：

-   [betaprofiles.dev][28]
-   [mrmacintosh.com][29]

最新の `InstallAssistant.pkg` をダウンロードしてください。これらのファイルは非常に大きく (14GB 以上)、高速なインターネット接続でもダウンロードに30分以上かかることがあります。

#### macOS Sequoia ベータをインストールする

`InstallAssistant.pkg` ファイルをダブルクリックしてインストールを開始します。"インストール場所の変更" をクリックして作成したボリュームを選択します。"インストール先の選択" ステップでは、新しいボリュームをインストール先として選択できます。

### スタートアップマネージャーを使用する

Mac の電源を入れる際に電源ボタンを長押しして、スタートアップマネージャーに入ります。"起動オプションの読み込み中" が表示されます。内部ドライブ、外付けドライブ（接続されていれば）、ディスクボリューム、または "オプション" から起動する選択肢があります。

外付けドライブまたはボリュームを選択して起動します。`システム設定` > `起動ディスク` で、外付けドライブやボリュームをデフォルトに設定することができます。

## macOS ベータ更新を停止する

macOS Sequoia ベータを使い続けたくない場合は、ベータ更新をオフにすることができます。

`システム設定` > `一般` > `ソフトウェアアップデート` に進みます。`ベータ更新` の「情報」ボタンをクリックして、`ベータ更新` を `オフ` に設定します。これにより、macOS のベータ更新が停止します。

macOS ベータを使用したくない場合は、この手順が必要です。これをしないと、Mac は最新のベータ版に継続して更新されます。

## macOS Sonoma に戻る

macOS ベータを外付けドライブまたは別のボリュームで実行している場合、内部ドライブの主要なボリュームとして macOS Sonoma は依然として存在しています。macOS ベータをもう使いたくない場合は、外付けドライブを再フォーマットするか、ボリュームを削除します。

## 予備の Mac で macOS Sonoma を復元する

予備の Mac で macOS Sequoia を使用している場合は、macOS Sonoma を再インストールして復元することができます。

Mac App Store から macOS Sonoma をダウンロードしてインストールできます。Mac App Store で "macOS Sonoma" を検索するか、このリンクを使用して [macOS Sonoma][30] のリストを表示します。`入手` をクリックすると、App Store が `システム設定` > `一般` > `ソフトウェアアップデート` を開いて macOS Sonoma のダウンロードを開始します。

App Store からのダウンロードは遅いので、1時間以上待つことになるでしょう。App Store は `アプリケーション` フォルダに `macOS Sonoma をインストール` するアプリケーションをインストールします。

ダウンロード完了後、`macOS Sonoma をインストール` アプリケーションが自動的に起動します。指示に従って macOS Sonoma をインストールします。

別の方法として、直接インストーラー `*.pkg` ファイルをダウンロードして macOS Sonoma を復元することもできます。このダウンロードは App Store より速いです。以下を確認してください：

-   [mrmacintosh.com][31]

`InstallAssistant.pkg` ファイルをダブルクリックしてインストールを開始します。

## 次のステップ

macOS Sequoia をインストールした後、[Mac の設定][32] についての推奨事項があります。[Mac の名前設定][33]、[Dock の設定][34]、および [Finder の設定][35] を含みます。

Mac でソフトウェアを開発するためには、以下が必要です：

-   [Xcode コマンドラインツールのインストール][36] - 欠落しているコマンドラインツールをインストール
-   [Homebrew のインストール][37] - ソフトウェアパッケージマネージャーとして
-   [Git のインストール][38] - バージョン管理用

macOS を更新する際には、新しいソフトウェアもインストールすることをお勧めします。macOS Sequoia 用の新しいお勧めアプリケーションは次の通りです：

-   [ターミナル][39] の代替品
-   [テキストエディタ][40] の選択肢
-   [ChatGPT デスクトップアプリケーション][41] - ChatGPT の使いやすさを向上

## 結論

2024年10月以降、バグ修正やセキュリティ、ソフトウェア互換性を保つため、特にソフトウェア開発者の場合は、macOS を Sonoma から Sequoia に更新する必要があります。

macOS Sequoiaは劇的な変化をもたらすわけではありませんが、Window TilingやPasswordsアプリのような新機能は便利です。

macOSベータ版のインストールには1時間以上かかりますが、毎日使用するのに十分安定していると感じるかもしれません。これで新機能にすぐアクセスできます。

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

