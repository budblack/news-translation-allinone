---
title: How to Write And Run C and C++ Code in Visual Studio Code
date: 2024-08-02T08:20:37.523Z
author: Md. Fahim Bin Amin
authorURL: https://www.freecodecamp.org/news/author/fahimbinamin/
originalURL: https://www.freecodecamp.org/news/how-to-write-and-run-c-cpp-code-on-visual-studio-code/
translator: ""
reviewer: ""
---

Visual Studio Code (or VS Code for short) is a very common and widely used text editor and IDE (Integrated Development Environment). You can make VS Code very powerful like an IDE using a lot of extensions.

<!-- more -->

Before approaching the process of running your first C or C++ code on Visual Studio Code, let me guide you through the process and get it all set up based on the operating system you are using on your computer.

## C and C++ compilers

For running C or C++ code, you just need to have a valid C/C++ compiler installed on your computer. If you are using a Linux operating system, then there is a high chance that it is already installed on your system. But we need to make sure that it is correctly installed.

For checking whether or not you have the compiler (GCC/G++/MinGW) installed on your system or not, you have to check the compiler version first.

Simply open your terminal and use `gcc --version` and `g++ --version`. If you get the version number, then the compiler is already installed on your system.

You can check the version using the same commands on any operating system, whether that is a Windows, Linux, or macOS-based operating system.

If you get feedback on your terminal that it does not know anything about GCC or G++, then you have to install the compiler correctly.

If you are using the most used Windows operating system, then I already have written an in-depth article showing you all the processes step-by-step on freeCodeCamp. Make sure to read the entire article first, as it also contains a complete video to provide you with complete support.

[

How to Install C and C++ Compilers on Windows

If you want to run C or C++ programs in your Windows operating system, then youneed to have the right compilers. The MinGW compiler is a well known and widely used software for installing GCCand G++ compilers for the C and C++ programming languages. But many devs face difficulties when install…

![favicon](https://cdn.freecodecamp.org/universal/favicons/favicon.ico)Md. Fahim Bin AminfreeCodeCamp.org

![banner_freeCodeCamp](https://www.freecodecamp.org/news/content/images/2022/02/banner_freeCodeCamp.png)

][1]

If you are using another operating system, and you don't have the compilers installed, then make sure to install them before proceeding.

## How to Install VS Code or VS Code Insiders

You have to download Visual Studio Code directly from the official website: [https://code.visualstudio.com/][2].

If you want, you can also install VS Code Insiders, and the same process is applicable for that as well.

Visual Studio Code Insiders is actually the "Insiders" build of Visual Studio Code, which contains all the latest features that are shipped daily. You can think of VS Code as the stable release and the VS Code Insiders as the Insiders release of that.

If you want to experience the latest updates instantly, then you might also try Visual Studio Code Insiders (I use it myself). For downloading VS Code Insiders, you can visit the official website for VS Code Insiders here: [https://code.visualstudio.com/insiders/][3]

Make sure to download the exact file for your operating system.

![image-163](https://www.freecodecamp.org/news/content/images/2023/01/image-163.png)

**Download Page: VS Code**

![image-164](https://www.freecodecamp.org/news/content/images/2023/01/image-164.png)

**Download Page: VS Code Insiders**

The installation process is pretty basic. But I am going to show you all the steps sequentially. For now, I am going to show you the installation process using VS Code Insiders, but everything you will see here is going to be exactly the same for VS Code as well.

Make sure to click the box on the "I accept the agreement " box and click on **Next**.

![image-165](https://www.freecodecamp.org/news/content/images/2023/01/image-165.png)

**Accept the agreement and click Next**

Keep everything as it is. Do not change anything from here.

![image-168](https://www.freecodecamp.org/news/content/images/2023/01/image-168.png)

**Click Next**

Click **Next**. Again, simply click **Next**.

![image-170](https://www.freecodecamp.org/news/content/images/2023/01/image-170.png)

**Click Next**

Make sure to add the checkmark (✔) on all of the boxes. Then click on **Next**.

![image-171](https://www.freecodecamp.org/news/content/images/2023/01/image-171.png)

**Check all of the boxes, and click Next**

Click on **Install**.

![image-172](https://www.freecodecamp.org/news/content/images/2023/01/image-172.png)

**Click Install**

It might take a little time to finish the installation.

![image-173](https://www.freecodecamp.org/news/content/images/2023/01/image-173.png)

**Let it finish...**

Click on **Finish**.

![image-175](https://www.freecodecamp.org/news/content/images/2023/01/image-175.png)

**Click Finish**

Congrats - you've successfully installed VS Code/VS Code Insiders on your system. Now, cheers! 🥂

## How to Prepare VS Code/VS Code Insiders For C and C++ Code

First, open VS Code or VS Code Insiders.

Go to the Extension tab. Search for "C" or "C++" and install the first one that is already verified by Microsoft itself.

![image-178](https://www.freecodecamp.org/news/content/images/2023/01/image-178.png)

**Install C/C++ extension**

Also, install **C/C++ Extension Pack**. It should also be verified by Microsoft.

![image-179](https://www.freecodecamp.org/news/content/images/2023/01/image-179.png)

**Install C/C++ Extension Pack**

Then you have to search for **Code Runner** and install the extension as well.

![image-180](https://www.freecodecamp.org/news/content/images/2023/01/image-180.png)

**Install Code Runner Extension**

Now, we need to change some settings.

![image-177](https://www.freecodecamp.org/news/content/images/2023/01/image-177.png)

**Change some settings**

Click the **gear** box (It is called the Manage section), and then click **Settings**. Alternatively, you can also use the shortcut keys `Ctrl` + `,`. You need to replace the `Ctrl` key with the Command key for Mac.

![image-182](https://www.freecodecamp.org/news/content/images/2023/01/image-182.png)

**Type "Run code in terminal" and press Enter key**

In the search bar, type "Run code in terminal" and press the Enter key.

Scroll down a little bit until you find `Code-runner: Run In Terminal`. Make sure that the box is checked (✔).

![image-184](https://www.freecodecamp.org/news/content/images/2023/01/image-184.png)

**Make sure to check the box**

Now you need to restart your VS Code/VS Code Insiders. Simply close and reopen the program.

## How to Test Your Code

Simply open VS Code/VS Code Insiders, open any folder, and create any file with the extension `.c` for the C file and `.cpp` for the C++ file.

After writing your code, you can run the code directly using the play button you'll find in the upper right corner.

![image-185](https://www.freecodecamp.org/news/content/images/2023/01/image-185.png)

**This is how you can run any C/C++ program from VS Code/Insiders**

It will compile and then run the code directly. After running a code, the code runner button would be set default to run directly. So, your computer is 100% ready for compiling and running any C/C++ programming code.  😀

## Conclusion

Thanks for reading the entire article. If it helps you then you can also check out other articles of mine at [freeCodeCamp][4].

If you want to get in touch with me, then you can do so using [Twitter][5], [LinkedIn][6], and [GitHub][7].

You can also [SUBSCRIBE to my YouTube channel][8] (Code With FahimFBA) if you want to learn various kinds of programming languages with a lot of practical examples regularly.

If you want to check out my highlights, then you can do so at my [Polywork timeline][9].

You can also [visit my website][10] to learn more about me and what I'm working on.

Thanks a bunch!

---

![Md. Fahim Bin Amin](https://www.freecodecamp.org/news/content/images/size/w60/2024/06/Md.-Fahim-Bin-Amin.jpg)

Read [more posts][11].

---

If you read this far, thank the author to show them you care. Say Thanks

Learn to code for free. freeCodeCamp's open source curriculum has helped more than 40,000 people get jobs as developers. [Get started][12]

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