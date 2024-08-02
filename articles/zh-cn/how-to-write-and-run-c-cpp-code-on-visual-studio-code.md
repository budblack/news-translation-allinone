---
title: 如何在 Visual Studio Code 中编写和运行 C 及 C++ 代码
date: 2024-08-02T08:20:37.523Z
author: Md. Fahim Bin Amin
authorURL: https://www.freecodecamp.org/news/author/fahimbinamin/
originalURL: https://www.freecodecamp.org/news/how-to-write-and-run-c-cpp-code-on-visual-studio-code/
translator: ""
reviewer: ""
---

Visual Studio Code（或简称 VS Code）是一个非常常见且广泛使用的文本编辑器和 IDE（集成开发环境）。通过使用大量扩展，你可以将 VS Code 变得像 IDE 一样强大。

<!-- more -->

在开始介绍如何在 Visual Studio Code 上运行你的第一个 C 或 C++ 代码之前，让我根据你计算机上使用的操作系统，带你了解设置的整个过程。

## C 和 C++ 编译器

要运行 C 或 C++ 代码，你只需要在你的计算机上安装一个有效的 C/C++ 编译器。如果你使用的是 Linux 操作系统，那么很有可能它已经安装在你的系统上了。但我们需要确保它已正确安装。

要检查你的系统上是否安装了编译器（GCC/G++/MinGW），你需要先检查编译器版本。

只需打开终端并使用 `gcc --version` 和 `g++ --version`。如果你得到版本号，那么说明编译器已经安装在你的系统上。

你可以在任何操作系统上使用相同的命令来检查版本，无论是 Windows、Linux 还是 macOS 系统。

如果你的终端反馈说它不知道 GCC 或 G++，那么你需要正确安装编译器。

如果你使用的是最常用的 Windows 操作系统，那么我已经在 freeCodeCamp 上写了一篇详细的文章，一步步展示所有过程。确保先阅读整篇文章，因为它还包含一个完整的视频，为你提供全面的支持。

[

如何在 Windows 上安装 C 和 C++ 编译器

如果你想在 Windows 操作系统中运行 C 或 C++ 程序，那么你需要拥有合适的编译器。MinGW 编译器是一款知名并且广泛使用的软件，用于为 C 和 C++ 编程语言安装 GCC 和 G++ 编译器。但是很多开发者在安装时会遇到困难...

![favicon](https://cdn.freecodecamp.org/universal/favicons/favicon.ico)Md. Fahim Bin AminfreeCodeCamp.org

![banner_freeCodeCamp](https://www.freecodecamp.org/news/content/images/2022/02/banner_freeCodeCamp.png)

][1]

如果你使用的是其他操作系统，并且没有安装编译器，请确保在继续之前安装它们。

## 如何安装 VS Code 或 VS Code Insiders

你需要直接从官方网站下载 Visual Studio Code: [https://code.visualstudio.com/][2]。

如果你愿意，你也可以安装 VS Code Insiders，同样的过程也适用于它。

Visual Studio Code Insiders 实际上是 Visual Studio Code 的 "Insiders" 版本，它包含每天发布的所有最新功能。你可以将 VS Code 视为稳定版，VS Code Insiders 视为 Insiders 版。

如果你想立即体验最新的更新，那么你也可以尝试 Visual Studio Code Insiders（我自己也在使用）。要下载 VS Code Insiders，可以访问其官方网站: [https://code.visualstudio.com/insiders/][3]

确保下载与你的操作系统匹配的文件。

![image-163](https://www.freecodecamp.org/news/content/images/2023/01/image-163.png)

**下载页面：VS Code**

![image-164](https://www.freecodecamp.org/news/content/images/2023/01/image-164.png)

**下载页面：VS Code Insiders**

安装过程非常简单。但我会按顺序向你展示所有步骤。现在，我将展示使用 VS Code Insiders 的安装过程，但你在这里看到的一切，VS Code 也完全相同。

确保勾选“我接受协议”框，然后点击 **Next**。

![image-165](https://www.freecodecamp.org/news/content/images/2023/01/image-165.png)

**接受协议并点击 Next**

保持所有设置不变。不用更改任何内容。

![image-168](https://www.freecodecamp.org/news/content/images/2023/01/image-168.png)

**点击 Next**

点击 **Next**。再次点击 **Next**。

![image-170](https://www.freecodecamp.org/news/content/images/2023/01/image-170.png)

**点击 Next**

确保勾选所有框（✔），然后点击 **Next**。

![image-171](https://www.freecodecamp.org/news/content/images/2023/01/image-171.png)

**勾选所有框，并点击 Next**

点击 **Install**。

![image-172](https://www.freecodecamp.org/news/content/images/2023/01/image-172.png)

**点击 Install**

完成安装可能需要一些时间。

![image-173](https://www.freecodecamp.org/news/content/images/2023/01/image-173.png)

**等待安装完成...**

点击 **Finish**。

![image-175](https://www.freecodecamp.org/news/content/images/2023/01/image-175.png)



恭喜 - 您已经成功在系统上安装了 VS Code/VS Code Insiders。现在，干杯！🥂

## 如何为 C 和 C++ 代码准备 VS Code/VS Code Insiders

首先，打开 VS Code 或 VS Code Insiders。

进入扩展选项卡。搜索 "C" 或 "C++" 并安装第一个已被微软验证的扩展。

![image-178](https://www.freecodecamp.org/news/content/images/2023/01/image-178.png)

**安装 C/C++ 扩展**

还需要安装 **C/C++ Extension Pack**。这个扩展包同样应当由微软验证。

![image-179](https://www.freecodecamp.org/news/content/images/2023/01/image-179.png)

**安装 C/C++ Extension Pack**

接下来，搜索 **Code Runner** 并安装该扩展。

![image-180](https://www.freecodecamp.org/news/content/images/2023/01/image-180.png)

**安装 Code Runner 扩展**

现在，我们需要更改一些设置。

![image-177](https://www.freecodecamp.org/news/content/images/2023/01/image-177.png)

**更改一些设置**

点击 **齿轮** 箱（它被称为管理部分），然后点击 **设置**。或者，你也可以使用快捷键 `Ctrl` + `,`。对于 Mac 系统，需要将 `Ctrl` 键替换为 Command 键。

![image-182](https://www.freecodecamp.org/news/content/images/2023/01/image-182.png)

**输入 "Run code in terminal" 并按下 Enter 键**

在搜索栏里输入 "Run code in terminal" 并按下 Enter 键。

向下滚动直到找到 `Code-runner: Run In Terminal`。确保该选项被勾选（✔）。

![image-184](https://www.freecodecamp.org/news/content/images/2023/01/image-184.png)

**确保勾选该选项**

现在你需要重新启动你的 VS Code/VS Code Insiders。简单地关闭并重新打开程序即可。

## 如何测试你的代码

只需打开 VS Code/VS Code Insiders，打开任何文件夹，并创建扩展名为 `.c` 的 C 文件和扩展名为 `.cpp` 的 C++ 文件。

写好代码后，你可以使用右上角的播放按钮直接运行代码。

![image-185](https://www.freecodecamp.org/news/content/images/2023/01/image-185.png)

**这就是你如何从 VS Code/Insiders 运行任何 C/C++ 程序的方法**

它将直接编译并运行代码。运行代码后，代码运行按钮会默认直接运行。所以，你的电脑已经 100% 准备好编译和运行任何 C/C++ 编程代码了。😀

## 结论

感谢阅读整篇文章。如果这篇文章对你有帮助，你也可以查看我的其他文章 [freeCodeCamp][4]。

如果你想与我联系，你可以通过 [Twitter][5]、[LinkedIn][6] 和 [GitHub][7] 与我联系。

如果你想定期学习各种编程语言和大量实际案例，你也可以 [订阅我的 YouTube 频道][8] (Code With FahimFBA)。

如果你想查看我的亮点，你可以在我的 [Polywork 时间线][9] 上查看。

你也可以 [访问我的网站][10] 来了解更多关于我的信息和我的工作内容。

非常感谢！

---

![Md. Fahim Bin Amin](https://www.freecodecamp.org/news/content/images/size/w60/2024/06/Md.-Fahim-Bin-Amin.jpg)

阅读 [更多文章][11]。

---

如果你读到了这里，请感谢作者以表示关心。说声谢谢

免费学习编程。freeCodeCamp 的开源课程帮助超过 40,000 人找到开发人员的工作。[开始学习][12]

[1]: https://www.freecodecamp.org/news/how-to-install-c-and-cpp-compiler-on-windows/
[2]: https://code.visualstudio.com/
[3]: https://code.visualstudio.com/insiders/
[4]: https://www.freecodecamp.org/news/author/fahimbinamin/
[5]: https://twitter.com/Fahim_FBA
[6]: https://www.linkedin.com/in/fahimfba/
[7]: https://github.com/FahimFBA
[8]: https://www.youtube.com/@FahimAmin?sub_confirmation=1
[9]: https://www.polywork.com/fahimbinamin
[10]: https://fahimbinamin.com/
[11]: /news/author/fahimbinamin/
[12]: https://www.freecodecamp.org/learn/

