---
title: How to Install C and C++ Compilers on Windows
date: 2024-08-02T09:13:22.812Z
author: Md. Fahim Bin Amin
authorURL: https://www.freecodecamp.org/news/author/fahimbinamin/
originalURL: https://www.freecodecamp.org/news/how-to-install-c-and-cpp-compiler-on-windows/
translator: ""
reviewer: ""
---

If you want to run C or C++ programs in your Windows operating system, then you need to have the right compilers.

<!-- more -->

The MinGW compiler is a well known and widely used software for installing GCC and G++ compilers for the C and C++ programming languages.

But many devs face difficulties when installing the compiler, so I am going to show you all the steps to do so in this article with screenshots to help you get it done.

I will be using Windows 11, but the same process is applicable for all other Windows operating systems unless you are using Windows XP (You need to change some steps in Windows XP).

If you'd like to watch the video I made on this topic as well, here it is:

<iframe width="356" height="200" src="https://www.youtube.com/embed/c7FjV8Gwk_M?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" title="How to Install C and C++ Compilers on Windows 10 / 11" name="fitvid0"></iframe>

## Install MSYS2

Firstly we need to download an executable file from MSYS2. Go to the official website of MSYS2: [https://www.msys2.org/][1]. The website looks like below as of today.

![Screenshot--8-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--8-.png)

Scroll down a little bit until you find the download button for the executable file.

![Screenshot--9-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--9-.png)

Simply click on the installer button and save the installer file in any place you want.

![Screenshot--10--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--10--1.png)

Finish downloading the executable file. It should not take much time depending on your internet speed.

![Screenshot--11-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--11-.png)

After downloading the file, we will get this executable file.

![Screenshot--12-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--12-.png)

Double click on the executable file. Then click `Next`.

![Screenshot--13-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--13-.png)

Keep the name as it is, and click `Next`.

![Screenshot--14--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--14--1.png)

Keep all this as it is, and click `Next`.

![Screenshot--15-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--15-.png)

Give it some time to finish the installation process.

![Screenshot--16-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--16-.png)

If you keep the checkmark, then the MSYS2 terminal will open once you click `Finish`.

![Screenshot--17-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--17-.png)

I prefer to do it this way, but if you want to do the remaining tasks later, then you need to open the terminal by yourself from the start menu.

In that case, you have to click the start button > Search for `MSYS2` and click on the terminal like in the following picture:

![Screenshot--26-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--26-.png)

Let me assume that we have opened the **MSYS2 MSYS** terminal successfully.

Apply the command `pacman -Syu` to update the package database and the base packages.

![Screenshot--19-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--19-.png)

Type `Y` and press the enter key if you get this type of installation prompt.

![Screenshot--20-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--20-.png)

![Screenshot--21-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--21-.png)

![Screenshot--22-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--22-.png)

Type `Y` and press the enter key.

![Screenshot--23-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--23-.png)

![Screenshot--24-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--24-.png)

The terminal will be closed. We have to open the terminal manually and update the rest of the packages.

Click the start button.

![Screenshot--25-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--25-.png)

Search the folder named **MSYS2 64bit**. Click on the folder to expand and get the terminal. Open the terminal by clicking **MSYS2 MSYS**.

![Screenshot--26--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--26--1.png)

Update the rest of the packages by applying the command, `pacman -Su`. You might need to apply the command `pacman -Sy` if the terminal tells you to do that.

![Screenshot--27-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--27-.png)

If you get any installation prompt, then you need to type `Y` or `y` and press the enter key.

![Screenshot--28-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--28-.png)

![Screenshot--29-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--29-.png)

Wait a little to finish the installation.

![Screenshot--30-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--30-.png)

![Screenshot--31-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--31-.png)

Close the window after finishing the installation.

## Install the GCC and G++ Compilers

Click the start button. Find the **MSYS2 64bit** folder. Click on that folder to expand it.

![Screenshot--32-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--32-.png)

If you are using a **64 bit** operating system like I am, then we need to use the **MSYS2 MinGW x64** terminal. Click on the terminal to open that.

![Screenshot--33-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--33-.png)

⚠️ But, if you are using a **32 bit** operating system, then you have to use the **MSYS2 MinGW x86** terminal. Then, you need to open that terminal.

![Screenshot--34-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--34-.png)

As I am using a **64 bit** operating system, I have opened the terminal for 64 bit. Apply the command `pacman -S mingw-w64-x86_64-gcc` to install the compilers.

⚠️ If you are using a **32 bit** operating system, then you have to apply the command `pacman -S mingw-w64-i686-gcc` in your 32 bit terminal.

![Screenshot--35-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--35-.png)

Wait for a little while.

![Screenshot--36-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--36-.png)

Type `Y` or `y` and press the enter key if you get the installation prompts.

![Screenshot--37-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--37-.png)

![Screenshot--38-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--38-.png)

Give it some time to finish the installation process.

![Screenshot--39-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--39-.png)

![Screenshot--39--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--39--1.png)

You've now finished installing the compilers.

## How to Install the Debugger

If you are using a **64 bit** operating system like I am, then you have to apply the command `pacman -S mingw-w64-x86_64-gdb`.

⚠️ If you are using a **32 bit** operating system, then you have to apply the command `pacman -S mingw-w64-i686-gdb` in your 32 bit terminal.

![Screenshot--41-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--41-.png)

If you get any installation prompt, then simply type `Y` or `y` and press the enter key.

![Screenshot--42-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--42-.png)

![Screenshot--38--1](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--38--1.png)

Give it some time to finish the installation.

![Screenshot--44-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--44-.png)

![Screenshot--45-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--45-.png)

You can close the terminal.

## How to Add the Directory to the Path of the Environment Variables

Open the file explorer.

![Screenshot--46-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--46-.png)

I am assuming that you have installed the MSYS into the default directory like I have. If you used custom directories, then you need to go to the directory where you installed it.

![Screenshot--47-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--47-.png)

If you are using a 64 bit operating system like I am, then go to the **mingw64** folder.

⚠️ If you are using a 32 bit operating system, then go to the **mingw32** folder.

![Screenshot--48-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--48-.png)

We have to go to the binary folder now. Go to the **bin** folder.

![Screenshot--49-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--49-.png)

⚠️ If you are using a 32 bit operating system, then you have to go into your **mingw32** folder > **bin** folder.

Copy the directory.

![Screenshot--51-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--51-.png)

⚠️ If you are using a 32 bit operating system, and you also installed the MSYS2 in the default directory, then your directory should be like the following:

```
C:\msys64\mingw32\bin
```

Open the **Advanced System Settings**. You can do that in many ways. A simple way is to simply click the start button and search for it like the below screenshot.

![Screenshot--52-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--52-.png)

Click **Environment Variables** from the Advanced tab.

![Screenshot--54-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--54-.png)

Click on **Path** and select that. Then click **Edit**.

![Screenshot--57-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--57-.png)

A window will appear as below:

![Screenshot--58-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--58-.png)

Click **New**.

![Screenshot--59-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--59-.png)

A blank box will appear.

![Screenshot--60-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--60-.png)

Paste the directory here.

![Screenshot--61-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--61-.png)

![Screenshot--62-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--62-.png)

Click **OK**.

![Screenshot--63-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--63-.png)

Click **OK**.

![Screenshot--65-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--65-.png)

Click **OK**.

![Screenshot--66-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--66-.png)

If you want to get all the steps in a video, then you can watch [this video][2] as well.

## Check the Install

Now it is time to check whether we have successfully installed all of the above or not.

Open the terminal / PowerShell / CMD and apply the commands serially:

For checking the **GCC** version:

```powershell
gcc --version
```

![Screenshot--68-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--68-.png)

For checking the **G++** version:

```powershell
g++ --version
```

![Screenshot--69-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--69-.png)

For checking the **GDB** version:

```powershell
gdb --version
```

![Screenshot--70-](https://www.freecodecamp.org/news/content/images/2022/02/Screenshot--70-.png)

## Conclusion

I hope this article helps you install your compilers on the Windows operating system for C and C++ programs.

Thanks for reading the entire article. If it helps you then you can also check out other articles of mine at [freeCodeCamp][3].

If you want to get in touch with me, then you can do so using [Twitter][4], [LinkedIn][5], and [GitHub][6].

You can also [SUBSCRIBE to my YouTube channel][7] (Code With FahimFBA) if you want to learn various kinds of programming languages with a lot of practical examples regularly.

If you want to check out my highlights, then you can do so at my [Polywork timeline][8].

You can also [visit my website][9] to learn more about me and what I'm working on.

Thanks a bunch!

---

![Md. Fahim Bin Amin](https://www.freecodecamp.org/news/content/images/size/w60/2024/06/Md.-Fahim-Bin-Amin.jpg)

Read [more posts][10].

---

If you read this far, thank the author to show them you care. Say Thanks

Learn to code for free. freeCodeCamp's open source curriculum has helped more than 40,000 people get jobs as developers. [Get started][11]

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