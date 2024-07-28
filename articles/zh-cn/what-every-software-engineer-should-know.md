---
title: 自学计算机科学 —— 你应该知道的关键计算机科学概念
date: 2024-07-25T02:53:50.986Z
author: Tamerlan Gudabayev
authorURL: https://www.freecodecamp.org/news/author/tamerlan/
OriginalURL: https://www.freecodecamp.org/news/what-every-software-engineer-should-know/
Proofreader: ""
 
---
 
软件开发可能让人感觉像是在追赶新技术的比赛。

<!-- more -->

总有新的前端框架要学习，或一个新数据库或语言，它们通常是其他语言的变种。感觉总是没有尽头，必须不停地学习。

但其实不必如此。

## 一切都建立在基础之上

如果你学会了基础知识，那么其他一切都会变得更容易。

例如，如果你 [学会了 TCP/IP 协议的工作原理][1]，那么你可以很容易地学会建立在它之上的所有其他协议。

你其实需要覆盖的范围更少。你了解的基础知识越多，学新东西时遇到的困难就越少。

我相信有 10 个核心主题，如果你学会了它们，将会为你打下坚实的基础。

## 为什么你应该学习这些关键概念？

学习基础知识会让你进入程序员的前 5%。

从另一个角度看，这里有一段来自 Ras Bodik 的名言很棒。

> 不要做一个模板程序员。 相反，要为用户和其他程序员构建工具。历史上，纺织和钢铁工业有记载：你是想构建机器和工具，还是想操作那些机器？

## 但有成千上万的课程可以选择

好吧，别再寻找了。

在下文中，我为每个主题整理了一些有用的资源——当然还有一些替代选项。这样你可以专注于学习，而不是无意识地研究哪本书/视频/课程是最好的。

### 一些注意事项

本文非常适合自学的开发者或对某些计算机科学概念不太熟悉的开发者。

如果你是第一次学习编程，我推荐去 Reddit 上的 [r/learnprogramming][2] 社区。

本文深受 [Oz Nova][3] 和 [Myles Byrne][4] 的启发，他们是 [teachyourselfcs.com][5] 网站的作者。如果你喜欢本文，可以随时查看和分享他们的网站。

## 目录

-   [编程][6]
-   [计算机体系结构][7]
-   [算法和数据结构][8]
-   [计算机科学的数学][9]
-   [操作系统][10]
-   [计算机网络][11]
-   [数据库][12]
-   [语言和编译器][13]
-   [分布式系统][14]
-   [网络安全][15]
-   [结论][16]

## 编程

![image-84](https://www.freecodecamp.org/news/content/images/2023/06/image-84.png)

[来源][17]

我不是在谈论语法，而是在谈论实际的编程或问题解决。诸如抽象、函数作为数据、递归，以及不同类型的编程范式（面向对象、函数式和声明式）。

我推荐的编程书是 [计算机程序的构造和解释][18] (SICP)（它也被称为魔法书）。

这本书是免费的，并且有一套 [MIT 讲座][19]。但是 MIT 的讲座由于当时（2005年）质量不佳，所以观看起来有点困难。因此，我推荐 [Brian Harvey 的 SICP 讲座][20]（伯克利 61A 课程）。

### 为什么这本书？

因为这本书专注于大局。

它不在意编程语言。它使用一种被称为 Scheme 的 Lisp 变体。Scheme 非常容易学习（你可能在不到一小时内就能学会），所以它让你专注于思想而不是语法。

正因为其简单性，它使得审视不同的编程范式成为可能。这是一种首先函数式的方式，但你可以实现自己的面向对象编程。

Scheme 是一种很好的教学语言，因为它将焦点从语言上移开，放到了大思想上。

如果你担心它在业界不被使用，没关系——你在掌握这些高级概念后，总是可以学习更为常用的编程语言。

### 但如果我真的不想学 Scheme 怎么办？

好吧，你可以跟随这本使用 Python 的新版本书。这本书叫做 [Composing Programs][21]。它也有一套 [自己的讲座][22]。

但是，我强烈推荐至少尝试一下 Scheme 版本。当你理解了它，简直就像魔法一样。

### 好吧，我试过了，但真的很难

是的，我理解。

有些人会觉得 SICP 有点太难，它并不是为纯粹的初学编程者设计的。

如果是这样，那我推荐 [如何设计程序][23] (HTDP)。它使用一种非常类似于 Scheme 的语言，整体上节奏更慢一些。你可以使用这本书及其在 edX 上的 [课程][24]。

### 学习建议

不要像读故事那样来读这些书。

它们不是为了从头到尾顺序阅读的。相反，**专注于练习题**。你不必完成所有练习题，但一定要确保你知道如何解决大多数问题。

讲座是可选的，只有在它们对你有帮助时才需要。这完全取决于你。

-   [讨论《计算机程序的构造和解释》的线上聚会][25]
-   [Racket][26]（Scheme 的集成开发环境） （[查看这个 StackOverFlow 回答以了解 Scheme 设置][27]）

## 计算机体系结构

![image-128](https://www.freecodecamp.org/news/content/images/2023/06/image-128.png)

[来源][28]

你写了一些代码，它神奇地运行了。

这是如何工作的呢？好了，这就是你在学习计算机体系结构时会了解到的。通过远远是大多数自学工程师最为忽视的科目。

作为工程师，我们不相信魔法。我们必须揭开计算机背后的魔法。你还会学到一些有用的东西，比如：

-   什么是 L1，L2 缓存？
-   为什么赛博朋克会卡顿？

我在这里推荐的书是 _[计算机系统：程序员的视角][29]_。我还推荐一个覆盖书中第1到第6章的 [入门课程][30]（由这本书的作者制作）。

### 但有一个问题

**这本书不适合从头到尾读**。它内容很多，可能不是按照最优顺序呈现的。

所以我建议你跟随课程并做实验练习。

### 如果我觉得太难怎么办？

许多人会觉得内容有点难，所以为了平稳过渡，我建议完成以下任务：

-   阅读 [代码：计算机硬件与软件的隐藏语言][31]
-   [阅读这本关于软件架构的手册][32]
-   观看所有 4 个 [探索计算机工作原理][33] 视频
-   观看所有 41 个 [Crash Course：计算机科学][34] 视频
-   参加 [NAnd2Tetris][35] 课程
-   通过阅读《C 语言现代方法》学一些 C 语言 [C Programming a Modern Approach][36]

完成这些后你就可以回到《计算机系统：程序员视角》这本书了。

## 数据结构与算法

![image-131](https://www.freecodecamp.org/news/content/images/2023/06/image-131.png)

[来源][37]

人人都想在 FAANG 公司工作，但没人愿意学习数据结构与算法。

不过我并不希望你仅仅为了技术面试而学习这些。数据结构和算法很重要，因为它们能提升你的问题解决能力。

有关数据结构与算法有很多很棒的书籍和课程，但我推荐 Steven Skiena 的 _[算法设计手册][38]_。你也可以看看他的课程 [此处][39]。

### 别忘了练习

同样的规则适用在这里。不仅要学习数据结构，还要在你想要的语言中创建它们。不仅要记住算法，还要实现它们，并查看它们可以在哪里和如何使用。

一个好办法是通过阅读本书或课程时解决一些 [Leetcode][40] 问题。

### 如果我觉得太难怎么办？

如果你觉得内容有点难，我会推荐以下资源：

-   阅读书籍：[图解算法][41]
-   阅读书籍：[如何解决它：数学方法的新视角][42]

总的来说，有许多教数据结构与算法的不同书籍/课程——以下是一些其他很棒的资源：

-   [freeCodeCamp 上的算法与数据结构课程][43]
-   [Algorithms Illuminated][44]
-   [普林斯顿算法课程][45]
-   [ThePrimegeans 数据结构与算法课程][46]
-   [MIT 算法导论][47]

## 计算机科学的数学

![image-144](https://www.freecodecamp.org/news/content/images/2023/06/image-144.png)

别担心，这是一张随便找到的数学图片，来源于 [这里][48]

许多新开发者跳过了这一部分。

但听我说——计算机科学本质上是数学的一个分支。学习它会通过锻炼你的问题解决能力使你成为一个更好的开发者。

### 计算机科学最相关的领域是离散数学

离散数学是处理可数或有限数字的数学分支。

离散数学的主题很多，但与计算机科学相关的有：

-   逻辑
-   组合学
-   离散概率
-   集合论
-   图论
-   数论

### 如何学习离散数学

我建议从一套 [László Lovász 的讲义笔记][49] 开始。

Lovász 教授的笔记比正规教材更易于理解，并且总体上读起来很有趣。他以一个问题开始，并使用离散数学来解决它。

之后，你可以选择一本 MIT 的书叫做 _[计算机科学的数学][50]._ 这本书配有一些[免费观看][51]的视频讲座。

### 如果它太难怎么办？

别担心——有时候你不得不接受**你并不 always 都能立刻掌握**。

没关系。

但如果你觉得自己缺乏一些基本的知识，那就是另一回事了。离散数学的基础先决科目是：

-   代数学
-   几何学
-   微积分

有很多免费的资源，但我推荐的是：

-   [可汗学院][52]
-   [大学代数课程][53]
-   [微积分 1 课程][54]
-   [微积分 2 课程][55]

## 操作系统

![image-228](https://www.freecodecamp.org/news/content/images/2023/06/image-228.png)

[来源][56]

还记得我告诉你我们作为开发者要去除计算中的魔法吗？


如果你了解这些操作系统是如何构建和工作的，那么你肯定会与众不同。

在网上找到关于操作系统的好资源有点困难，但最推荐的书是[《操作系统：三易之门》(OSTEP)][57]。虽然没有任何官方的视频讲座能完全涵盖这本书的内容，但我找到了这个[YouTube 播放列表][58]。

### 推荐的先决条件

我建议先学习计算机体系结构，并对 C 语言有一些了解，然后再开始操作系统的学习之旅。

### 可选资源

现在，我建议先完成 OSTEP，然后再检查其他推荐资源。它们都是可选的。

- 想构建自己的 Linux 系统？请查看[Linux from Scratch][59]。
- 想深入了解 Linux、MacOS 和 Windows？[这里有一本手册给你][60]。
- 想构建自己的操作系统？请查看[OSDEV][61]。
- 想构建自己的套接字？请查看[Beej 的网络编程指南][62]。

## 计算机网络

![image-237](https://www.freecodecamp.org/news/content/images/2023/06/image-237.png)

[来源][63]

自从互联网诞生以来，计算机网络一直是软件工程师最重要的课题之一。

如果你不了解 IP、TCP、UDP、HTTP、TLS、DNS、SMTP 等，那么你应该学习计算机网络（尤其是如果你是后端工程师）。

这里推荐的书是[《计算机网络：自顶向下方法》][64]。你还可以查看这本书作者自己提供的[视频讲座][65]。

但在开始之前，我建议先查看这个[自底向上的计算机网络速成课程视频][66]。这里有一个非常有用的[涵盖基础的教程][67]。

## 数据库

![image-229](https://www.freecodecamp.org/news/content/images/2023/06/image-229.png)

[来源][68]

数据库相对较新——它们出现在 20 世纪 70 年代，并且从那时起成为许多应用程序的重要组成部分。

我强烈推荐下面由[CMU 数据库小组][69]提供的课程。它们完全免费，且可在 YouTube 上观看。我建议至少完成第一个课程。

1. [数据库入门][70]
2. [数据库研讨会][71]
3. [高级数据库][72]

另外，[这里有一个非常棒的 SQL 数据库学习资源集合][73]。这是一个关于 NoSQL 数据库的免费课程][74]。

## 语言和编译器

![image-230](https://www.freecodecamp.org/news/content/images/2023/06/image-230.png)

[来源][75]

你可能知道如何用一种或多种编程语言编写代码。

但是你知道如何创建或设计一种编程语言吗？这就是你通过学习编程语言和编译器所要了解的内容。

推荐的入门书籍是[《Crafting Interpreters》][76]。

之后，你可以继续学习《编译器：原理、技术与工具》（也被称为“龙书”）。该书涵盖了很多主题，因此我强烈推荐同时进行一门课程。我推荐的是 [Alex Aiken 在 edX 上的课程][78]。

这里有一个帮助初学者理解 C 编程语言编译器工作原理的[有用教程][79]。

## 分布式系统

![image-231](https://www.freecodecamp.org/news/content/images/2023/06/image-231.png)

[来源][80]

如果你只选择学习列表中的一个科目，请选择分布式系统。它是技术公司的圣杯，如果你想找到一份开发人员的工作，你应该精通分布式系统。

我推荐的学习路径是：

1. 阅读这本书：[Understanding Distributed Systems][81]
2. 阅读这本书：[Designing Data Intensive Applications][82]，也被称为“红皮书”
3. 在阅读“红皮书”时，同时观看其配套的[麻省理工学院课程视频][83]。
4. 阅读这本书：[软件架构：难点][84]（可选）
5. 你也可以[查看我关于分布式系统设计模式的手册][85]。

## 网络安全

![image-232](https://www.freecodecamp.org/news/content/images/2023/06/image-232.png)

[来源][86]

在过去的 2-3 年里，发生了许多安全漏洞。

外界变得越来越危险——作为一名软件工程师，了解一些网络安全的基础知识会让你更有优势。

我首先推荐的课程是[斯坦福大学的 CS253 网络安全课][87]。它对网络安全进行了全面的概述，所以你可以预期会学到诸如 web 应用程序漏洞、注入、拒绝服务等主题。

你还可以[查看这些常见漏洞][88]，学习如何防止利用这些漏洞的攻击。

后来，如果你愿意，你可以通过[pwn.college][89]学习如何进行黑客攻击。

## 结论

学习所有这些科目会花费你一些时间，并且需要持续的努力。但如果你喜欢自己所做的事情，并对这些科目感兴趣，那么它应该更像是娱乐而不是任务。

无论你选择学习哪些科目。我能给你的最重要的建议是……

### 不做被动的学习者

不要只看视频——也要完成练习。与教程一起构建项目。

不要只是读书，而要通过提问和进行自己的研究来参与其中。

我真诚地希望我能鼓励你去学习一些这些科目。和往常一样，我希望感谢你阅读这篇文章。

祝你一切顺利。

[1]: https://www.freecodecamp.org/news/what-is-tcp-ip-layers-and-protocols-explained/
[2]: https://www.reddit.com/r/learnprogramming/
[3]: https://twitter.com/oznova_
[4]: https://twitter.com/quackingduck
[5]: https://teachyourselfcs.com/
[6]: #programming
[7]: #computer-architecture
[8]: #algorithms-and-data-structures
[9]: #math-for-computer-science
[10]: #operating-systems
[11]: #computer-networking
[12]: #databases
[13]: #language-and-compilers
[14]: #distributed-systems
[15]: https://www.freecodecamp.org/news/p/dfc9104e-85e4-4749-88dc-1859e6c643b9/web-security
[16]: https://www.freecodecamp.org/news/p/dfc9104e-85e4-4749-88dc-1859e6c643b9/conclusion
[17]: https://dabeaz.com/sicp.html
[18]: https://sarabander.github.io/sicp/html/index.xhtml
[19]: https://ocw.mit.edu/courses/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video_galleries/video-lectures/
[20]: https://archive.org/details/ucberkeley-webcast-PL3E89002AA9B9879E?sort=titleSorter
[21]: http://composingprograms.com/
[22]: https://cs61a.org/
[23]: https://htdp.org/
[24]: https://www.edx.org/course/how-to-code-simple-data
[25]: https://www.youtube.com/playlist?list=PLVFrD1dmDdvdvWFK8brOVNL7bKHpE-9w0
[26]: #https:/racket-lang.org/
[27]: https://stackoverflow.com/a/25096066
[28]: https://github.com/ahmeducf/computer-systems-CS-APP3e
[29]: http://csapp.cs.cmu.edu/3e/home.html
[30]: https://www.cs.cmu.edu/afs/cs/academic/class/15213-f16/www/schedule.html
[31]: https://www.amazon.com/Code-Language-Computer-Hardware-Software/dp/0735611319
[32]: https://www.freecodecamp.org/news/an-introduction-to-software-architecture-patterns/
[33]: https://www.youtube.com/playlist?list=PLFt_AvWsXl0dPhqVsKt1Ni_46ARyiCGSq
[34]: https://www.youtube.com/playlist?list=PLH2l6uzC4UEW0s7-KewFLBC1D0l6XRfye
[35]: https://www.coursera.org/learn/build-a-computer
[36]: https://www.amazon.com/C-Programming-Modern-Approach-2nd/dp/0393979504
[37]: https://twitter.com/StevenSkiena/status/1336050368875290629
[38]: https://www.amazon.com/Algorithm-Design-Manual-Steven-Skiena/dp/1849967202
[39]: https://www3.cs.stonybrook.edu/~skiena/373/videos/
[40]: https://leetcode.com/
[41]: https://www.amazon.com/Grokking-Algorithms-illustrated-programmers-curious/dp/1617292230
[42]: https://www.amazon.com/How-Solve-Mathematical-Princeton-Science/dp/069111966X#:~:text=Polya%2C%20How%20to%20Solve%20It,winning%20a%20game%20of%20anagrams.
[43]: https://www.freecodecamp.org/news/algorithms-and-data-structures-free-treehouse-course/
[44]: https://algorithmsilluminated.org/
[45]: https://www.coursera.org/learn/algorithms-part1
[46]: https://frontendmasters.com/courses/algorithms/
[47]: https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/
[48]: https://unsplash.com/photos/h3kuhYUCE9A
[49]: https://cims.nyu.edu/~regev/teaching/discrete_math_fall_2005/dmbook.pdf
[50]: https://courses.csail.mit.edu/6.042/spring17/mcs.pdf
[51]: https://ocw.mit.edu/courses/6-042j-mathematics-for-computer-science-fall-2010/video_galleries/video-lectures/
[52]: https://www.khanacademy.org/
[53]: https://www.freecodecamp.org/news/college-algebra-course-with-python-code/
[54]: https://www.freecodecamp.org/news/learn-college-calculus-in-free-course/
[55]: https://www.freecodecamp.org/news/learn-calculus-2-in-this-free-7-hour-course/
[56]: https://pages.cs.wisc.edu/~remzi/OSTEP/
[57]: https://pages.cs.wisc.edu/~remzi/OSTEP/
[58]: https://www.youtube.com/playlist?list=PLhtZD20ADU45ADsAIxlNpFowP3iYvGXvJ
[59]: https://www.linuxfromscratch.org/
[60]: https://www.freecodecamp.org/news/an-introduction-to-operating-systems/
[61]: https://wiki.osdev.org/Introduction
[62]: https://beej.us/guide/bgnet/
[63]: https://github.com/topics/top-down-approach
[64]: https://gaia.cs.umass.edu/kurose_ross/wireshark.php
[65]: https://www.youtube.com/playlist?list=PLByK_3hwzY3Tysh-SY9MKZhMm9wIfNOas
[66]: https://www.youtube.com/playlist?list=PLowKtXNTBypH19whXTVoG3oKSuOcw_XeW
[67]: https://www.freecodecamp.org/news/computer-networking-how-applications-talk-over-the-internet/
[68]: https://www.astera.com/type/blog/a-quick-overview-of-different-types-of-databases/
[69]: https://www.youtube.com/@CMUDatabaseGroup/featured
[70]: https://www.youtube.com/playlist?list=PLSE8ODhjZXjaKScG3l0nuOiDTTqpfnWFf
[71]: https://www.youtube.com/playlist?list=PLSE8ODhjZXjZKp-oX_75aBnznulk7nubu
[72]: https://www.youtube.com/playlist?list=PLSE8ODhjZXjYzlLMbX3cR0sxWnRM7CLFn
[73]: https://www.freecodecamp.org/news/learn-sql-free-relational-database-courses-for-beginners/
[74]: https://www.freecodecamp.org/news/learn-nosql-in-3-hours/
[75]: https://chidiwilliams.com/post/crafting-interpreters-a-review/
[76]: https://craftinginterpreters.com/contents.html
[77]: https://smile.amazon.com/Compilers-Principles-Techniques-Tools-2nd/dp/0321486811
[78]: https://www.edx.org/course/compilers
[79]: https://www.freecodecamp.org/news/what-is-a-compiler-in-c/
[80]: https://vvsevolodovich.dev/designing-data-intensive-applications-by-martin-kleppmann/
[81]: https://www.amazon.com/gp/product/1838430202/ref=as_li_qf_asin_il_tl?ie=UTF8&tag=utsavized0d-20&creative=9325&linkCode=as2&creativeASIN=1838430202&linkId=8f3007bbed9b958980492f5c0bb1105f
[82]: https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321
[83]: https://www.youtube.com/@6.824/videos
[84]: https://www.amazon.com/dp/1492086894?psc=1&linkCode=sl1&tag=utsavized0d-20&linkId=64e15d236bb8c1015661423e5be849ac&language=en_US&ref_=as_li_ss_tl
[85]: https://www.freecodecamp.org/news/design-patterns-for-distributed-systems/
[86]: https://www.ifourtechnolab.com/blog/principles-of-web-security
[87]: https://web.stanford.edu/class/cs253/
[88]: https://www.freecodecamp.org/news/technical-dive-into-owasp/
[89]: https://pwn.college/

