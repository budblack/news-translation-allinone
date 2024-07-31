---
title: macOS 有什么新变化？如何安装 Sequoia Beta 版
date: 2024-07-31T06:34:09.832Z
author: Daniel Kehoe
authorURL: https://www.freecodecamp.org/news/author/danielkehoe/
OriginalURL: https://www.freecodecamp.org/news/whats-new-in-macos-how-to-install-the-sequoia-beta/
Proofreader: ""

---

macOS Sequoia 公测版现已推出。

<!-- more -->

尽管 macOS Sequoia（macOS 15）的最终版本要到 2024 年 9 月底或 10 月初才会发布，我将向你展示如何安装公测版以提前体验。这实际上已经足够稳定，可以日常使用。

任何想要尝试 macOS Sequoia 公测版的人都可以下载，但你需要注册 [Apple Beta Software Program][1] 才能获得。

## 目录

1.  [macOS Sequoia 稳定吗？][2]
2.  [安装所需时间][3]
3.  [macOS Sequoia 有什么新变化][4]
4.  [macOS Sequoia 的特性][5]
5.  [macOS Sequoia 的一些小变化][6]
6.  [macOS Sequoia 的要求][7]
7.  [首先备份你的 Mac][8]
8.  [注册以获得公测版][9]
9.  [在哪里安装 macOS 测试版][10]  
    – [安装在备用 Mac 上][11]  
    – [安装在外置硬盘上][12]  
    – [安装在独立的卷宗上][13]
10.  [使用启动管理器][14]
11.  [暂停 macOS 测试版更新][15]
12.  [返回 macOS Sonoma][16]
13.  [下一个步骤][17]

## macOS Sequoia 稳定吗？

到目前为止，用户报告该测试版本只是有一些小问题。他们表示该测试版 “出奇地稳定”。

有报告称外部显示器存在问题，用户建议预期会与外部第三方设备有问题。屏幕共享、视频会议（特别是 Zoom）或在网络浏览器中进行流媒体播放可能也会存在问题。

## 安装所需时间

从 macOS Sonoma 升级到 macOS Sequoia 可能需要一个多小时。所需时间因更新大小、互联网速度以及你的 Mac 的年龄和性能而异。

## macOS Sequoia 有什么新变化

用户报告称 macOS Sequoia 更快，笔记本电脑的电池寿命更长，但我们要等到最终版本发布后才能确定。

仔细查看 [macOS Sequoia][18]，显然这并不是操作系统的重大改造。最有用的特性是窗口平铺和新的密码应用程序，以及 iPhone 镜像和设备之间的无缝拖放。

我在另一篇文章中比较了 [Sonoma vs Sequoia][19]，并提供了一些建议来回答 [你是否应该更新到 macOS Sequoia？][20]

## macOS Sequoia 的特性

![mac-passwords-app](https://www.freecodecamp.org/news/content/images/2024/07/mac-passwords-app.png)

macOS Sequoia 密码应用程序

### 密码管理器

MacOS Sequoia 添加了一款名为密码的新应用程序，改进了用户管理登录凭证的方式。

基于 Apple Keychain 的现有框架，此应用程序将密码、密钥、Wi-Fi 密码和其他重要凭证集中在一个安全的中心位置。

以前，凭证可以在系统设置中编辑，但它们被埋藏且难以找到。新的密码应用程序大大减少了使用第三方密码管理器（如 1Password、LastPass 或 Bitwarden）的需求。

![mac-sequoia-tiling](https://www.freecodecamp.org/news/content/images/2024/07/mac-sequoia-tiling.png)

macOS Sequoia 窗口平铺

### 窗口平铺

多年以来，Windows 用户一直抱怨 MacOS 缺乏窗口平铺管理器。MacOS Sequoia 添加了一个名为窗口平铺的新功能，允许用户将窗口拖到屏幕边缘，进行并排、上下或网格排列。第三方实用程序有更多功能，但内置的窗口平铺功能是一个受欢迎的补充。

这两个功能让升级变得有价值。此外，Apple 还宣布了其他功能。

### iPhone 镜像

此功能允许在 macOS 窗口中使用 iPhone 应用程序。用户现在可以直接在 Mac 上查看 iPhone 通知，使 Mac 成为 iPhone 的延伸。

一位用户指出，“我再也不必在家里坐在 Mac 前仅为了查看通知而找手机。”

### 无缝设备间拖放

此功能旨在改进 iPhone 和 Mac 之间传输文件的可靠性，解决 AirDrop 的问题。一位用户提到，“从 Mac 到 iPhone 应用程序传输文件不再需要 5 个或更多繁琐的步骤。”

### Apple 智能

MacOS Sequoia 将推出 Apple 智能的首次使用，这是 Apple 的 AI 计划。Apple 智能包括新的系统级功能，利用 Apple 定制硅片进行本地和云处理。

这更像是未来的前景，因为 AI 将融入更多应用程序，但我们可能会看到 macOS Sequoia 中 Siri 的改进。请注意，如果你在基于 Intel 的 Mac 上安装 macOS Sequoia，这些功能将不可用。

## macOS Sequoia 的一些小变化

-   **系统设置：** 各个菜单已重新排列，以便更快地访问常用菜单。
-   **Safari：** 这个网络浏览器页面加载速度更快，有了新的开始页面，以及类似于 iOS 上“紧凑模式”的全新统一菜单。它可以总结网站并突出显示相关信息。
-   **备忘录：** 小改进包括可折叠部分和高亮样式选择。此外，备忘录增加了对实时音频转录和数学公式的支持。
-   **视频会议：** 预览你在视频通话中共享的内容，用于演示和屏幕共享。此外，背景替换已内置在 macOS 视频流中，因此你不需要在 Zoom 或其他会议应用中使用背景替换。



[检查你的 macOS 版本][21] 并在安装 macOS Sequoia 测试版之前 [更新 macOS][22] 到 Sonoma（macOS 14）。

你应该在 Mac 上保留当前的 macOS Sonoma，以防在测试版中遇到问题。这意味着你应该在一个单独的卷、外部硬盘或第二台 Mac 上安装 macOS Sequoia 测试版。

此外，macOS Sequoia 确实可以运行在较老的基于 Intel 的 Mac 上，但可能会很慢。所以我建议只在搭载 M1、M2 或 M3（Apple Silicon 芯片）的 Mac 上安装。

你可以在任何运行 macOS Sonoma 的计算机上安装 macOS Sequoia 测试版，但不包括搭载 Intel Amber Lake 芯片的 2018-2019 年款 MacBook Air 型号。Apple 有一个 [macOS Sequoia 支持的型号列表][23]。

## 备份你的 Mac

如果你有一台全新的 Mac 并且还没有使用过，你不需要备份文件。或者，如果你像许多开发者一样，如果你所有的重要文件都存储在云端，你也不需要备份你的 Mac。

否则，如果你的计算机上有重要文件，在安装 macOS 测试版之前，请确保你有一个 Mac 的备份。

## 注册以获取公开测试版

Apple 提供了公开测试版和开发者测试版。开发者测试版首先发布，旨在让软件开发者测试应用程序的兼容性，而公开测试版会在几周后发布。公开测试版比开发者测试版更稳定，错误更少。

![macOS Sequoia Public Beta](https://www.freecodecamp.org/news/content/images/2024/07/apple-beta-program.png)

公开测试版现在免费提供。可以在 [Apple Beta Software Program][24] 网站上注册公开测试版。在你用 Apple ID 注册之后，系统设置将显示可以使用测试版更新。

## 在哪里安装 macOS 测试版

如果你有额外的计算机，最好的选择是在备用 Mac 上安装 macOS 测试版。理想情况下，你有一台相对较新的装有 Apple Silicon M1、M2 或 M3 芯片的 Mac。如果你有较旧的 Mac，你可能会想避开测试版，因为它可能会使你的计算机变慢。

在备用 Mac 上安装可以让你尝试新的 macOS 版本而不会影响你的日常生产力。

或者，你可以在 Mac 上的一个单独的卷上安装 macOS 测试版。这允许你在想试用时启动测试版。

你也可以在外部硬盘上安装测试版。在这两种情况下，你都需要按住电源按钮，直到看到启动管理器菜单，它让你选择一个非默认的启动磁盘。

以下是如何在备用 Mac、外部硬盘或单独的卷上安装 macOS Sequoia 测试版的说明。

### 在备用 Mac 上安装

以下是在运行 macOS Sonoma 的 Mac 上安装 macOS Sequoia 测试版的方法。

1.  打开 `系统设置` 并导航到 `通用` 和 `软件更新`。
2.  在 `测试版更新` 中点击“圆圈 I”信息按钮。
3.  将 `测试版更新` 设置为 `macOS Sequoia Public Beta`。
4.  点击“完成”，你的 Mac 将检查软件更新。
5.  检查后，升级名称会出现一个“立即升级”按钮。
6.  软件更新至少需要 20% 的电池电量，因此如果你的电池电量低，可能需要连接电源。
7.  输入你的密码开始软件更新。使用快速的互联网连接，下载大约需要 30 分钟。下载后，“准备”过程大约需要 15 分钟。
8.  安装完成后你的 Mac 将重新启动。你会看到 Apple 标志和一个进度条。安装过程大约需要 15 分钟，会有几次自动重启。
9.  安装完成后，你会看到登录屏幕。输入你的 Mac 密码，然后是你的 Apple ID 密码，单击“继续”或“稍后设置”通过各种协议和设置。
10.  macOS Sequoia 桌面会出现，并打开反馈助手应用程序。使用反馈助手报告你遇到的任何错误或问题。
11.  检查 `关于本机` 以确认你正在运行 macOS 15。

如果你在 `测试版更新` 中没有看到 `macOS Sequoia Public Beta` 选项，请注册 [Apple Beta Software Program][25]。在你用 Apple ID 注册后，系统设置将显示有测试版更新可用。

### 在外部硬盘上安装

现在的用户不多拥有外部硬盘，因为云存储很流行。但如果你有外部硬盘，可以在其上安装 macOS 测试版。

你需要格式化硬盘，所以必须擦除硬盘上已有的所有文件。最好是拥有一个速度快、带有 USB-C 或 Thunderbolt 连接的 SSD 硬盘来使用操作系统。你可以使用一个 USB 闪存驱动器，但需要至少 32 GB 的空间。

#### 如何格式化外部硬盘

1.  将外部硬盘连接到你的 Mac。
2.  在 Spotlight 中搜索并打开 `磁盘工具`。
3.  在左侧栏选择外部硬盘。
4.  点击 `抹掉` 以重新格式化硬盘。
5.  将硬盘命名为 `macOS Sequoia` 或你喜欢的任何名字。
6.  选择 `Mac OS 扩展（日志式）` 作为格式。
7.  选择 `GUID 分区图` 作为方案。
8.  点击 `抹掉` 以格式化硬盘。
9.  当硬盘格式化完成后，关闭 `磁盘工具`。

你需要下载 `*.pkg` 文件以便在外部驱动器上安装。几个网站提供 macOS 测试版安装程序 `*.pkg` 文件的链接。查看以下网站：

-   [betaprofiles.dev][26]
-   [mrmacintosh.com][27]

下载最新的 `InstallAssistant.pkg`。这些文件非常大（14GB 或更多），所以即使使用快速的互联网连接，下载也可能需要超过 30 分钟。

#### 如何安装 macOS Sequoia 测试版

双击 `InstallAssistant.pkg` 文件以开始安装。点击“更改安装位置”选择外部驱动器。在“选择目标”步骤中，你可以选择外部驱动器作为安装目标。

### 安装在单独的卷上

如果你想在单独的卷上安装 macOS 测试版，请按照以下步骤操作。你可能会听到这个过程被称为“双启动”或“单独分区”安装。苹果的 APFS 文件系统引入了“卷”，它们类似于分区但更灵活。

你的 Mac 上将有两个卷，一个用于 macOS Sonoma，一个用于 macOS Sequoia。你可以使用启动管理器选择从哪个卷启动。

#### 如何创建新卷

1.  在 Spotlight 中搜索并打开 `磁盘工具`。
2.  在左侧边栏中选择内部驱动器。
3.  点击顶部栏中的 `+` 按钮添加新卷（或在菜单中选择“编辑” > “添加 APFS 卷”）。
4.  命名卷为 `macOS Sequoia` 或你喜欢的名称。
5.  选择格式（通常为“APFS”）。
6.  点击 `Add` 创建卷。
7.  创建卷完成后，点击“完成”并关闭 `磁盘工具`。

#### 获取 macOS Sequoia 测试版

你需要下载 `*.pkg` 文件以便在单独的卷上安装。几个网站提供 macOS 测试版安装程序 `*.pkg` 文件的链接。查看以下网站：

-   [betaprofiles.dev][28]
-   [mrmacintosh.com][29]

下载最新的 `InstallAssistant.pkg`。这些文件非常大（14GB 或更多），所以即使使用快速的互联网连接，下载也可能需要超过 30 分钟。

#### 安装 macOS Sequoia 测试版

双击 `InstallAssistant.pkg` 文件以开始安装。点击“更改安装位置”选择你创建的卷。在“选择目标”步骤中，你可以选择新卷作为安装目标。

### 使用启动管理器

启动 Mac 时按住电源按钮进入启动管理器。会出现“加载启动选项”。你可以选择从内部驱动器、外部驱动器（如果连接了）、磁盘卷或“选项”启动。

选择外部驱动器或卷进行启动。你可以在 `系统设置` > `启动磁盘` 中为外部驱动器或卷设置默认值。

## 停止 macOS Beta 更新

如果你不想继续使用 macOS Sequoia 测试版，你可以关闭测试版更新。

前往 `系统设置` > `通用` > `软件更新`。点击 `Beta 更新` 中的“圆圈 I” 信息按钮，并将 `Beta 更新` 设置为 `关闭`。这将停止 macOS 测试版更新。

如果你不想使用 macOS 测试版，这是必要的步骤。如果你不进行此操作，你的 Mac 将继续更新到最新的测试版。

## 返回到 macOS Sonoma

如果你使用外部驱动器或单独的卷运行 macOS 测试版，你的 Mac 上仍有 macOS Sonoma 作为内部驱动器上的主卷。如果你不再想使用 macOS 测试版，可以重新格式化外部驱动器或删除卷。

## 在备用 Mac 上恢复 macOS Sonoma

如果你在备用 Mac 上使用 macOS Sequoia，你可以通过重新安装来恢复 macOS Sonoma。

你可以从 Mac App Store 下载并安装 macOS Sonoma。在 Mac App Store 中搜索 “macOS Sonoma”，或者用这个链接查看 [macOS Sonoma][30] 的列表。点击“获取”，App Store 会打开 `系统设置` > `通用` > `软件更新` 并开始下载 macOS Sonoma。

从 App Store 下载速度很慢，所以需要等待一个小时或更长时间。App Store 将在 `应用程序` 文件夹中安装一个 `Install macOS Sonoma` 应用程序。

下载完成后，`Install macOS Sonoma` 应用程序会自动启动。按照说明安装 macOS Sonoma。

或者，你可以直接下载一个安装程序 `*.pkg` 文件来恢复 macOS Sonoma。这种下载比 App Store 快。查看以下网站：

-   [mrmacintosh.com][31]

双击 `InstallAssistant.pkg` 文件以开始安装。

## 下一步

安装 macOS Sequoia 后，我有一些 [Mac 设置推荐][32]，包括 [Mac 名称设置][33]、[Dock 设置][34] 和 [Finder 设置][35]。

要在 Mac 上开发软件，你需要：

-   安装 [Xcode 命令行工具][36] 以获取缺失的命令行工具
-   安装 [Homebrew][37] 作为软件包管理器
-   安装 [Git][38] 进行版本控制

在更新 macOS 时，你可能还希望安装更新的软件。以下是 macOS Sequoia 的新应用和推荐应用：

-   [终端][39] 替代品
-   [文本编辑器][40] 选项
-   更好的 ChatGPT 可用性的 [ChatGPT 桌面应用][41]

## 结论

在 2024 年 10 月之后，你需要从 Sonoma 更新到 Sequoia 以保持最新的错误修复、安全性和软件兼容性，尤其是如果你是软件开发者的话。


虽然 macOS Sequoia 并没有带来显著的变化，但像窗口平铺和密码应用这样的新功能还是很有用的。

安装 macOS 测试版需要一个小时或更长的时间，但你可能会发现它已经足够稳定，可以每天使用，从而让你现在就能体验到新功能。

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

