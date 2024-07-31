---
title: macOS 的新功能？如何安装 Sequoia 测试版
date: 2024-07-31T06:34:09.832Z
author: Daniel Kehoe
authorURL: https://www.freecodecamp.org/news/author/danielkehoe/
OriginalURL: https://www.freecodecamp.org/news/whats-new-in-macos-how-to-install-the-sequoia-beta/
Proofreader: ""

---

macOS Sequoia 公共测试版现已推出。

<!-- more -->

尽管 macOS Sequoia（macOS 15）的最终版本要到 2024 年 9 月底或 10 月初才会发布，但我将向您展示如何安装公共测试版以提前预览。事实上，它已经足够稳定，可以日常使用。

macOS Sequoia 公共测试版对任何想尝试的人都开放，您需要注册 [Apple Beta Software Program][1] 才能获取。

## 目录

1.  [macOS Sequoia 稳定吗？][2]
2.  [安装所需的时间][3]
3.  [macOS Sequoia 的新功能][4]
4.  [macOS Sequoia 的功能][5]
5.  [macOS Sequoia 的小改动][6]
6.  [macOS Sequoia 的要求][7]
7.  [首先备份您的 Mac][8]
8.  [注册以获取公共测试版][9]
9.  [在哪里安装 macOS 测试版][10]  
    – [在备用 Mac 上安装][11]  
    – [在外部驱动器上安装][12]  
    – [在独立分区上安装][13]
10.  [使用启动管理器][14]
11.  [停止 macOS 测试版更新][15]
12.  [返回 macOS Sonoma][16]
13.  [接下来是什么][17]

## macOS Sequoia 稳定吗？

目前，用户反馈测试版只有少量小问题。他们表示这个测试版“意外地稳定”。

有报告指出外接显示器存在问题，用户还表示可能会遇到外部第三方设备的问题。可能还会有屏幕共享、视频会议（特别是 Zoom）或网浏览器中的流媒体问题。

## 安装所需的时间

从 macOS Sonoma 更新到 macOS Sequoia 可能需要超过一个小时。所需时间受诸如更新大小、互联网速度以及 Mac 的年龄和性能等因素的影响而有很大差异。

## macOS Sequoia 的新功能

用户报告 macOS Sequoia 更快，笔记本电脑的电池续航更好，但我们要等到最终发布才能确定。

仔细查看 [macOS Sequoia][18]，可以清楚地看到这并不是操作系统的重大改革。最有用的功能是窗口拼接和新的密码应用程序，以及 iPhone 镜像和设备之间无缝的拖放。

我在另一篇文章中比较了 [Sonoma 和 Sequoia的区别][19]，还提供了一些建议来回答“[是否应更新到 macOS Sequoia？][20]”的问题。

## macOS Sequoia 的功能

![mac-passwords-app](https://www.freecodecamp.org/news/content/images/2024/07/mac-passwords-app.png)

macOS Sequoia 密码应用程序

### 密码管理器

macOS Sequoia 增加了一款名为“密码”的新应用，改进了用户管理登录凭据的方式。

基于 Apple Keychain 的现有框架，这款应用将密码、密钥、Wi-Fi 密码和其他重要凭据整合到一个安全的中央位置。

以前可以在系统设置中编辑凭据，但它们埋得深入且难以找到。新的密码应用程序将大大减少使用第三方密码管理器（如 1Password、LastPass 或 Bitwarden）的需求。

![mac-sequoia-tiling](https://www.freecodecamp.org/news/content/images/2024/07/mac-sequoia-tiling.png)

macOS Sequoia 窗口拼接

### 窗口拼接

多年来，Windows 用户一直抱怨 macOS 缺乏拼接窗口管理器。macOS Sequoia 增加了一个名为窗口拼接的新功能，允许用户将窗口拖到屏幕边缘，以便并排、上下或网格方式放置。第三方实用程序提供更多功能，但内置的窗口拼接是一个受欢迎的补充。

这两个功能使得升级非常值得。此外，Apple 还宣布了其他能力。

### iPhone 镜像

这个功能允许在 macOS 窗口内使用 iPhone 应用程序。用户现在可以直接在 Mac 上查看 iPhone 通知，使 Mac 成为 iPhone 的延伸。

一位用户指出：“当我在家里坐在 Mac 前面时，不再需要找手机来查看通知。”

### 无缝设备间拖放

这个功能旨在提高 iPhone 和 Mac 之间文件传输的可靠性，解决了 AirDrop 的问题。一位用户提到：“从 Mac 向 iPhone 应用传输文件不再需要 5+ 繁琐步骤。”

### Apple 智能

macOS Sequoia 将首次引入 Apple 智能，这是 Apple 的 AI 计划。Apple 智能包括新的系统级功能，利用 Apple 定制芯片进行本地和云端处理。

这是一个更未来的前景，因为 AI 会融入更多应用程序，但我们可能会在 macOS Sequoia 中看到 Siri 的改进。需要注意的是，当您在搭载 Intel 的 Mac 上安装 macOS Sequoia 时，这些功能不会存在。

## macOS Sequoia 的小改动

- **系统设置：** 各个菜单已重新排列，以便更快访问常用菜单。
- **Safari：** 网页浏览器加载页面更快，有一个新的起始页，以及类似于 iOS“紧凑模式”的全新统一菜单。它可以总结网站并突出显示相关信息。
- **备忘录：** 小改进包括可折叠章节和多种高亮样式选择。此外，备忘录增加了对实时音频转录和数学方程的支持。
- **视频会议：** 在视频通话中预览共享内容用于演示和屏幕共享。此外，背景替换功能已内置于 macOS 视频流中，因此无需在 Zoom 或其他会议应用中使用背景替换。

[1]: https://beta.apple.com/sp/betaprogram/
[2]: #is-macos-sequoia-stable
[3]: #time-needed-to-install
[4]: #whats-new-in-macos-sequoia
[5]: #features-in-macos-sequoia
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
[18]: https://developer.apple.com/macos/sequoia-preview/
[19]: https://www.freecodecamp.org/news/sonoma-vs-sequoia/
[20]: https://www.freecodecamp.org/news/should-you-update-to-macos-sequoia/



[检查你的 macOS 版本][21]并在安装 macOS Sequoia 测试版之前，[更新 macOS][22]到 Sonoma (macOS 14)。

在你的 Mac 上保留当前的 macOS Sonoma，以防在测试版中遇到问题。这意味着你应该在一个单独的卷、外部硬盘或第二台 Mac 上安装 macOS Sequoia 测试版。

此外，macOS Sequoia 确实可以在较旧的基于 Intel 的 Mac 上运行，但可能会很慢。所以我建议只在装有 M1、M2 或 M3 苹果硅芯片的 Mac 上安装它。

你可以在任何运行 macOS Sonoma 的电脑上安装 macOS Sequoia 测试版，除了有 Intel Amber Lake 芯片的 2018-2019 款 MacBook Air。苹果提供了[支持 macOS Sequoia 的型号列表][23]。

## 备份你的 Mac

如果你有一台未使用过的新 Mac，那么你不需要备份文件。或者，如果你和许多开发者一样，如果你将所有重要文件存储在云端，你也不需要备份你的 Mac。

否则，如果你的电脑上有重要文件，请确保在安装 macOS 测试版之前有 Mac 的备份。

## 注册以获得公测版

苹果提供公测版和开发者测试版。开发者测试版首先发布，旨在让软件开发者测试应用程序的兼容性，而公测版则在几周后发布。公测版更加稳定，错误也更少。

![macOS Sequoia Public Beta](https://www.freecodecamp.org/news/content/images/2024/07/apple-beta-program.png)

公测版现已免费提供。请在 [Apple Beta Software Program][24] 网站注册以获得公测版。使用你的 Apple ID 注册后，你的系统设置将显示有测试版更新可用。

## 在哪里安装 macOS 测试版

最佳选择是在备用 Mac 上安装 macOS 测试版，如果你有一台额外的电脑。理想情况下，你有一台相对较新的装有 Apple Silicon M1、M2 或 M3 芯片的 Mac。如果你的 Mac 比较旧，你可能会想要避免使用测试版，因为它可能会减慢你的电脑速度。

在备用 Mac 上安装可以让你在不影响日常生产力的情况下尝试新 macOS 版本。

另外，你可以在你的 Mac 上的一个单独卷上安装 macOS 测试版。这允许你在想要试用时启动到测试版。

你也可以将测试版安装到一个外部硬盘上。在任一情况下，你都需要按住电源按钮直到看到启动管理器菜单，这让你可以选择除默认启动磁盘之外的其他选项。

以下是将 macOS Sequoia 测试版安装到备用 Mac、外部硬盘或单独卷上的说明。

### 在备用 Mac 上安装

这是在运行 macOS Sonoma 的 Mac 上安装 macOS Sequoia 测试版的方法。

1.  打开 `系统设置` 并导航到 `通用` 和 `软件更新`。
2.  点击 `测试版更新` 中的 "圆圈 I" 信息按钮。
3.  将 `测试版更新` 设置为 `macOS Sequoia 公测版`。
4.  点击 "完成"，你的 Mac 将检查软件更新。
5.  检查后，升级名称会出现并带有一个 "立即升级" 按钮。
6.  软件更新需要至少 20% 的电池电量，因此如果电池电量低，你可能需要连接电源。
7.  输入你的密码以开始软件更新。使用快速网络连接，下载大约需要 30 分钟。下载后，"准备" 过程大约需要 15 分钟。
8.  安装完成后，Mac 将重新启动。你会看到苹果标志和进度条。安装过程大约需要 15 分钟，并会自动多次重新启动。
9.  安装完成后，你会看到登录屏幕。输入你的 Mac 密码，然后输入你的 Apple ID 密码，并在各种协议和设置中点击"继续"或"稍后设置"。
10.  macOS Sequoia 桌面将会出现，并打开反馈助手应用程序。使用反馈助手报告你遇到的任何错误或问题。
11.  检查 `关于本机` 以确认你正在运行 macOS 15。

如果你在 `测试版更新` 中没有看到 `macOS Sequoia 公测版` 选项，请注册 [Apple Beta Software Program][25]。使用你的 Apple ID 注册后，你的系统设置将显示有测试版更新可用。

### 在外部硬盘上安装

现在云存储很流行，使用外部硬盘的用户不多了。但如果你有一个外部硬盘，你可以在其上安装 macOS 测试版。

你需要格式化硬盘，所以你必须删除硬盘上已有的文件。最好拥有一个带有 USB-C 或 Thunderbolt 接口的快速 SSD 硬盘以运行操作系统。你也可以使用 USB 闪存盘，但需要至少 32 GB 空间。

#### 如何格式化外部硬盘

1.  将外部硬盘连接到你的 Mac。
2.  在 Spotlight 中搜索并打开 `磁盘工具`。
3.  在左侧栏中选择外部硬盘。
4.  点击 `抹掉` 以重新格式化硬盘。
5.  将硬盘命名为 `macOS Sequoia` 或你喜欢的名称。
6.  选择 `Mac OS 扩展（日志式）` 作为格式。
7.  选择 `GUID 分区图` 作为方案。
8.  点击 `抹掉` 以格式化硬盘。
9.  硬盘格式化完成后关闭 `磁盘工具`。

你需要下载 `*.pkg` 文件以在外部驱动器上安装。有几个网站提供 macOS 测试版的安装程序 `*.pkg` 文件的链接。请查看：

-   [betaprofiles.dev][26]
-   [mrmacintosh.com][27]

下载最新的 `InstallAssistant.pkg`。这些文件非常大（14GB 或更多），即使是在快速的互联网连接下，下载也可能需要超过 30 分钟。

#### 如何安装 macOS Sequoia 测试版

双击 `InstallAssistant.pkg` 文件开始安装。点击“更改安装位置”以选择外部驱动器。在“选择目标”步骤中，您可以选择外部驱动器作为安装目标。

### 安装在单独的卷上

如果你想在单独的卷上安装 macOS 测试版，请按照以下步骤操作。你可能会听到这个过程被称为“双重引导”或“单独分区”安装。Apple 的 APFS 文件系统引入了“卷”，它们类似于分区但更灵活。

你的 Mac 上将有两个卷，一个用于 macOS Sonoma，一个用于 macOS Sequoia。你可以使用启动管理器选择从哪个卷启动。

#### 如何创建新卷

1.  在 Spotlight 中搜索并打开 `磁盘工具`。
2.  在左侧边栏中选择内部驱动器。
3.  点击顶部栏中的 `+` 按钮以添加新卷（或者在菜单中选择“编辑” > “添加 APFS 卷”）。
4.  将卷命名为 `macOS Sequoia` 或你喜欢的名字。
5.  选择格式（通常是“APFS”）。
6.  点击 `添加` 以创建卷。
7.  完成卷创建后，点击“完成”并关闭 `磁盘工具`。

#### 获取 macOS Sequoia 测试版

你需要下载 `*.pkg` 文件以在单独的卷上安装。有几个网站提供 macOS 测试版的安装程序 `*.pkg` 文件的链接。请查看：

-   [betaprofiles.dev][28]
-   [mrmacintosh.com][29]

下载最新的 `InstallAssistant.pkg`。这些文件非常大（14GB 或更多），即使是在快速的互联网连接下，下载也可能需要超过 30 分钟。

#### 安装 macOS Sequoia 测试版

双击 `InstallAssistant.pkg` 文件开始安装。点击“更改安装位置”以选择你创建的卷。在“选择目标”步骤中，你可以选择新卷作为安装目标。

### 使用启动管理器

启动你的 Mac 时，按住电源按钮进入启动管理器。将会显示“加载启动选项”。你可以选择从内部驱动器、外部驱动器（如果已连接）、磁盘卷或“选项”启动。

选择外部驱动器或卷进行启动。你可以在 `系统设置` > `启动磁盘` 中设置外部驱动器或卷的默认启动。

## 停止 macOS 测试版更新

如果你不想继续使用 macOS Sequoia 测试版，你可以关闭测试版更新。

进入 `系统设置` > `常规` > `软件更新`。点击 `Beta软件更新` 中的“圆圈 I”信息按钮，并将 `Beta软件更新` 设置为 `关闭`。这将停止 macOS 测试版更新。

这是一个必要的步骤，如果你不想使用 macOS 测试版。如果你不这样做，你的 Mac 将继续更新到最新的测试版。

## 返回 macOS Sonoma

如果你使用外部驱动器或单独的卷运行 macOS 测试版，你的 Mac 上仍然有 macOS Sonoma 作为内部驱动器上的主卷。如果你不再想使用 macOS 测试版，可以重新格式化外部驱动器或删除卷。

## 恢复备用 Mac 上的 macOS Sonoma

如果你在备用 Mac 上使用 macOS Sequoia，可以通过重新安装来恢复 macOS Sonoma。

你可以从 Mac App Store 下载并安装 macOS Sonoma。 在 Mac App Store 中搜索“macOS Sonoma”或使用此链接查看 [macOS Sonoma][30] 的列表。点击“获取”，App Store 将会打开 `系统设置` > `常规` > `软件更新` 并开始下载 macOS Sonoma。

从 App Store 下载的速度很慢，因此预计需要一个小时或更长时间等待。App Store 会在 `应用程序` 文件夹中安装一个名为 `安装 macOS Sonoma` 的应用程序。

下载完成后，`安装 macOS Sonoma` 应用程序会自动启动。按照说明安装 macOS Sonoma。

或者，你可以直接下载一个安装程序 `*.pkg` 文件来恢复 macOS Sonoma。下载速度比 App Store 更快。请查看：

-   [mrmacintosh.com][31]

双击 `InstallAssistant.pkg` 文件开始安装。

## 接下来

在你安装 macOS Sequoia 之后，我有一个 [Mac 设置][32] 的推荐列表，包括 [Mac 名称设置][33]、[Dock 设置][34] 和 [Finder 设置][35]。

要在 Mac 上开发软件，你需要：

-   [安装 Xcode 命令行工具][36] 以补全缺失的命令行工具
-   [安装 Homebrew][37] 作为软件包管理器
-   [安装 Git][38] 以进行版本控制

当你更新 macOS 时，你可能还会想要安装更新的软件。这里有一些 macOS Sequoia 新推荐的应用程序：

-   [终端][39] 替代品
-   [文本编辑器][40] 选项
-   [ChatGPT 桌面应用程序][41] 以更好地使用 ChatGPT

## 结论

在 2024 年 10 月之后，你需要从 macOS Sonoma 更新到 macOS Sequoia 以保持最新的错误修复、安全性和软件兼容性，尤其是如果你是一名软件开发人员。



虽然 macOS Sequoia 并没有带来显著的变化，但像窗口平铺和密码应用这样的新功能是很有用的。

安装 macOS 测试版需要一个小时或更长时间，但你可能会发现它足够稳定，可以日常使用，让你现在就能体验新功能。

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

