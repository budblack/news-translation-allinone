---
title: 如何在 Windows 上安装 C 和 C++ 编译器
date: 2024-08-02T09:13:22.812Z
author: Md. Fahim Bin Amin
authorURL: https://www.freecodecamp.org/news/author/fahimbinamin/
originalURL: https://www.freecodecamp.org/news/how-to-install-c-and-cpp-compiler-on-windows/
translator: ""
reviewer: ""
---

如果你想在 Windows 操作系统上运行 C 或 C++ 程序，那么你需要有合适的编译器。

<!-- more -->

MinGW 编译器是一个知名且广泛使用的软件，用于安装 C 和 C++ 编程语言的 GCC 和 G++ 编译器。

但是许多开发人员在安装编译器时遇到了困难，所以我将在本文中向大家展示所有步骤，并附上截图来帮助你完成安装。

我将使用 Windows 11，但除非你使用的是 Windows XP（你需要更改一些步骤），否则相同的过程适用于所有其他 Windows 操作系统。

如果你也想观看我关于此主题的视频，请点击这里：

<iframe width="356" height="200" src="https://www.youtube.com/embed/c7FjV8Gwk_M?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" title="How to Install C and C++ Compilers on Windows 10 / 11" name="fitvid0"></iframe>

## 安装 MSYS2

首先，我们需要从 MSYS2 下载一个可执行文件。访问 MSYS2 的官方网站：[https://www.msys2.org/][1]。截至今天，网站看起来如下。

![Screenshot--8-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--8-.png)

向下滚动，直到找到可执行文件的下载按钮。

![Screenshot--9-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--9-.png)

简单地点击安装按钮，并将安装文件保存在你希望的任何位置。

![Screenshot--10--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--10--1.png)

完成可执行文件的下载。根据你的网络速度，下载时间不应该太长。

![Screenshot--11-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--11-.png)

下载文件后，我们将获得这个可执行文件。

![Screenshot--12-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--12-.png)

双击可执行文件。然后点击`Next`。

![Screenshot--13-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--13-.png)

保持名称不变，然后点击`Next`。

![Screenshot--14--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--14--1.png)

保持所有内容不变，并点击`Next`。

![Screenshot--15-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--15-.png)

给它一些时间来完成安装过程。

![Screenshot--16-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--16-.png)

如果保持选中，则一旦你点击`Finish`，MSYS2 终端将会打开。

![Screenshot--17-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--17-.png)

我更喜欢这样做，但如果你想稍后再执行剩余任务，则需要从开始菜单自行打开终端。

在这种情况下，你需要点击开始按钮 > 搜索`MSYS2`，然后像下面的图片一样点击终端：

![Screenshot--26-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--26-.png)

让我假设我们已经成功打开了**MSYS2 MSYS**终端。

应用命令`pacman -Syu`来更新软件包数据库和基础软件包。

![Screenshot--19-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--19-.png)

如果你看到这种安装提示，请输入`Y`并按回车键。

![Screenshot--20-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--20-.png)

![Screenshot--21-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--21-.png)

![Screenshot--22-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--22-.png)

输入`Y`并按回车键。

![Screenshot--23-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--23-.png)

![Screenshot--24-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--24-.png)

终端将关闭。我们必须手动打开终端并更新其余的软件包。

点击开始按钮。

![Screenshot--25-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--25-.png)

搜索名为**MSYS2 64bit**的文件夹。点击该文件夹展开并获得终端。通过点击**MSYS2 MSYS**打开终端。

![Screenshot--26--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--26--1.png)

通过应用命令`pacman -Su`来更新其余的软件包。如果终端告诉你需要执行命令`pacman -Sy`，则可能需要执行此命令。

![Screenshot--27-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--27-.png)

如果收到任何安装提示，则需要输入`Y`或`y`并按回车键。

![Screenshot--29-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--29-.png)

稍等一会儿完成安装。

![Screenshot--30-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--30-.png)

![Screenshot--31-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--31-.png)

安装完成后关闭窗口。

## 安装 GCC 和 G++ 编译器

点击开始按钮，找到 **MSYS2 64bit** 文件夹，点击该文件夹展开它。

![Screenshot--32-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--32-.png)

如果你和我一样使用的是 **64 位** 操作系统，那么我们需要使用 **MSYS2 MinGW x64** 终端。点击终端以打开它。

![Screenshot--33-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--33-.png)

⚠️但是，如果你使用的是 **32 位** 操作系统，那么你需要使用 **MSYS2 MinGW x86** 终端。然后，你需要打开该终端。

![Screenshot--34-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--34-.png)

因为我使用的是 **64 位** 操作系统，所以我打开了 64 位终端。使用命令 `pacman -S mingw-w64-x86_64-gcc` 以安装编译器。

⚠️如果你使用的是 **32 位** 操作系统，那么你需要在你的 32 位终端中使用命令 `pacman -S mingw-w64-i686-gcc`。

![Screenshot--35-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--35-.png)

稍等一会儿。

![Screenshot--36-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--36-.png)

如果收到安装提示，输入 `Y` 或 `y` 并按下回车键。

![Screenshot--37-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--37-.png)

![Screenshot--38-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--38-.png)

等待安装过程完成。

![Screenshot--39-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--39-.png)

![Screenshot--39--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--39--1.png)

编译器安装完成。

## 如何安装调试器

如果你和我一样使用的是 **64 位** 操作系统，那么你需要使用命令 `pacman -S mingw-w64-x86_64-gdb`。

⚠️如果你使用的是 **32 位** 操作系统，那么你需要在你的 32 位终端中使用命令 `pacman -S mingw-w64-i686-gdb`。

![Screenshot--41-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--41-.png)

如果收到安装提示，输入 `Y` 或 `y` 并按下回车键。

![Screenshot--42-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--42-.png)

![Screenshot--38--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--38--1.png)

等待安装过程完成。

![Screenshot--44-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--44-.png)

![Screenshot--45-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--45-.png)

你可以关闭终端。

## 如何将目录添加到环境变量的路径

打开文件资源管理器。

![Screenshot--46-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--46-.png)

假设你和我一样将 MSYS 安装到默认目录。如果你使用了自定义目录，则需要前往你安装的目录。

![Screenshot--47-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--47-.png)

如果你和我一样使用的是 64 位操作系统，则前往 **mingw64** 文件夹。

⚠️如果你使用的是 32 位操作系统，请前往 **mingw32** 文件夹。

![Screenshot--48-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--48-.png)

现在我们需要转到二进制文件夹，前往 **bin** 文件夹。

![Screenshot--49-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--49-.png)

⚠️如果你使用的是 32 位操作系统，则需要进入 **mingw32** 文件夹 > **bin** 文件夹。

复制该目录。

![Screenshot--51-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--51-.png)

⚠️如果你使用的是 32 位操作系统，并且也将 MSYS2 安装到了默认目录，那么你的目录应该如下所示：

```
C:\msys64\mingw32\bin
```

打开 **高级系统设置**。你可以通过多种方式做到这一点，一种简单的方式是点击开始按钮并搜索它，如下图所示。

![Screenshot--52-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--52-.png)

从高级选项卡中点击 **环境变量**。

![Screenshot--54-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--54-.png)

点击 **Path** 并选择它。然后点击 **编辑**。

![Screenshot--57-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--57-.png)

将出现如下窗口：

![Screenshot--58-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--58-.png)

![Screenshot--59-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--59-.png)

会出现一个空白框。

![Screenshot--60-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--60-.png)

在这里粘贴目录。

![Screenshot--61-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--61-.png)

![Screenshot--62-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--62-.png)

点击 **OK**。

![Screenshot--63-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--63-.png)

点击 **OK**。

![Screenshot--65-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--65-.png)

点击 **OK**。

![Screenshot--66-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--66-.png)

如果你想获取所有步骤的视频，你也可以观看[这个视频][2]。

## 检查安装

现在是时候检查我们是否成功安装了上述所有内容。

打开终端 / PowerShell / CMD，并逐一应用命令：

检查 **GCC** 版本：

```powershell
gcc --version
```

![Screenshot--68-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--68-.png)

检查 **G++** 版本：

```powershell
g++ --version
```

![Screenshot--69-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--69-.png)

检查 **GDB** 版本：

```powershell
gdb --version
```

![Screenshot--70-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--70-.png)

## 结论

希望本文能帮助你在Windows操作系统上为C和C++程序安装编译器。

感谢你阅读整篇文章。如果它对你有帮助，你还可以查看我在[freeCodeCamp][3]上的其他文章。

如果你想与我联系，可以通过[Twitter][4]、[LinkedIn][5]和[GitHub][6]。

如果你希望定期学习各种编程语言的实用例子，可以[订阅我的YouTube频道][7]（Code With FahimFBA）。

如果你想查看我的亮点，可以访问我的[Polywork时间线][8]。

你也可以[访问我的网站][9]以了解更多关于我的信息和我目前正在做的工作。

非常感谢！

---

![Md. Fahim Bin Amin](https://www.freecodecamp.org/news/content/images/size/w60/2024/06/Md.-Fahim-Bin-Amin.jpg)

阅读[更多文章][10]。

---

如果你读到这里，请感谢作者，表示你在乎他们的付出。说声谢谢

免费学习编程。freeCodeCamp的开源课程已帮助超过40,000人找到开发人员的工作。[开始学习][11]

[1]: https://www.msys2.org/
[2]: https://www.youtube.com/watch?v=0HD0pqVtsmw
[3]: https://www.freecodecamp.org/news/author/fahimbinamin/
[4]: https://twitter.com/Fahim_FBA
[5]: https://www.linkedin.com/in/fahimfba/
[6]: https://github.com/FahimFBA
[7]: https://www.youtube.com/@FahimAmin?sub_confirmation=1
[8]: https://www.polywork.com/fahimbinamin
[9]: https://fahimbinamin.com/
[10]: /news/author/fahimbinamin/
[11]: https://www.freecodecamp.org/learn/

