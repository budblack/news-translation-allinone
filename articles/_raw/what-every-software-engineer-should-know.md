---
title: Teach Yourself Computer Science – Key CS Concepts You Should Know
date: 2024-07-25T02:53:50.986Z
author: Tamerlan Gudabayev
authorURL: https://www.freecodecamp.org/news/author/tamerlan/
OriginalURL: https://www.freecodecamp.org/news/what-every-software-engineer-should-know/
Proofreader: ""

---

Software development may feel like a bit of a race to keep up with new technologies.

<!-- more -->

There's always a new frontend framework to learn, or a new database or language that's a variation of another language. It's never ending and feels like you always have to keep up.

But it doesn't have to be this way.

## Everything is Built From the Fundamentals

If you learn the fundamentals, then everything else will become easier.

For example, if you [learn how the TCP/IP protocol works][1], then from that you can easily learn all the other protocols that are built on top of it.

You're essentially having to cover less ground. The more fundamentals you know, the less you will struggle learning new things.

I believe there are 10 core subjects which, if you learn them, will give you a solid foundation.

## Why Should You Learn These Key Concepts?

Learning the fundamentals will really put you in the top 5% of all programmers.

If we look at it from a different perspective, here's a great quote from Ras Bodik.

> Don’t be a boilerplate programmer. Instead, build tools for users and other programmers. Take historical note of textile and steel industries: do you want to build machines and tools, or do you want to operate those machines?

## But There are a Million Different Courses to Choose From

Well, look no further.

Below, I've compiled a bunch of helpful resources on each subject – with some alternatives, of course. So you can focus on learning and not on mindlessly researching which books/videos/courses are the best.

### A few notes

This article is well-suited for self-taught developers or developers who don't feel quite comfortable with certain computer science concepts.

If you are learning to program for the first time, I would recommend [r/learnprogramming][2] community on Reddit.

This article was heavily inspired by [Oz Nova][3] and [Myles Byrne][4] who authored the site [teachyourselfcs.com][5]. If you enjoy this article, feel free to check out and share their site.

## Table of Contents

-   [Programming][6]
-   [Computer Architecture][7]
-   [Algorithms and Data Structures][8]
-   [Math for Computer Science][9]
-   [Operating Systems][10]
-   [Computer Networking][11]
-   [Databases][12]
-   [Languages and Compilers][13]
-   [Distributed Systems][14]
-   [Web Security][15]
-   [Conclusion][16]

## Programming

![image-84](https://www.freecodecamp.org/news/content/images/2023/06/image-84.png)

[Source][17]

I'm not talking about syntax here. But actually programming or problem solving. Things such as abstraction, functions as data, recursion, and the different kinds of programming paradigms (object-oriented, functional, and declarative).

The book I recommend to learn programming is [Structures and Interpretations of Computer Programs][18] (SICP) (It's also known as the wizard book).

The book is free and has a set of [MIT lectures][19]. But the MIT lectures are a bit hard to watch due to the poor quality of that time (2005). So I recommend [Brian Harvey’s SICP lectures][20] (for the 61A course at Berkeley) instead.

### Why this book?

Because this book focuses on the big picture.

It doesn't care about the programming language. It uses a variation of Lisp called Scheme. Scheme is very easy to learn (you can probably learn it in less than an hour), so it let's you focus on ideas not syntax.

Because of its simplicity, it makes it possible to examine different programming paradigms. It's a functional first approach, but you can implement your own OOP.

Scheme is a great language for teaching because it takes the focus away from the language and puts it on the big ideas.

If you're worried about it not being used in the industry, it's ok – you can always learn a more commonly-used programming languages after you grasp these high-level concepts.

### But what if I REALLY don't want to learn Scheme?

Okay, you can follow the new version of the book which uses Python. The book is called [Composing Programs][21]. It also has its own [set of lectures][22].

But, I highly recommend at least trying to do the Scheme version. It's just magical once you get it.

### Okay, I've tried it but it's really hard

Yes, I understand.

Some of you will find SICP a bit too hard. It's not meant for purely beginner programmers.

If that's the case, then I would recommend [How to Design Programs (HTDP)][23]. It uses a language very similar to Scheme and is generally more slower paced. You can use this book and its [course on edX][24].

### Tips on Studying

Don't read these books like a story.

It's not meant to be read cover to cover. Instead, **focus on the exercises**. You don't have to do them all, but just make sure you know how to solve most of them.

The lectures are optional and only needed if they help. It's really up to you.

### Additional Resources

-   [Virtual meetups that talk about SICP][25]
-   [Racket][26] (IDE for Scheme) ([Checkout this StackOverFlow answer for Scheme setup][27])

## Computer Architecture

![image-128](https://www.freecodecamp.org/news/content/images/2023/06/image-128.png)

[Source][28]

You wrote some code and it magically runs.

How does that work? Well, this is what you will learn with computer architecture. This is by far the most neglected subject by most self taught engineers.

As engineers, we don't believe in magic. We have to unravel the magic behind computers. You will also learn some useful stuff such as:

-   What is the L1, L2 cache?
-   Why does cyberpunk lag?

The book I recommend here is _[Computer Systems: A Programmer's Perspective][29]_. I would also recommend an [introductory course][30] that will cover chapters 1-6 of the book (That was made by the authors of the book).

### But there's a catch

**This book is not meant to be read cover to cover**. It has a lot of content, that may not well be presented in the optimal order.

So I recommend that you follow the course and do the labs.

### What if I find it too hard?

A lot of people will find the content a bit heavy, so to ease into it, I would recommend doing the following:

-   Read [Code: The Hidden Language of Computer Hardware and Software][31]\\
-   [Read this handbook on Software Architecture][32]
-   Watch all 4 videos of [Exploring How Computers Work][33]
-   Watch all 41 videos of [Crash Course: Computer Science][34]
-   Take the course [NAnd2Tetris][35]
-   Learn a bit of C by reading the book: [C Programming a Modern Approach][36]

Once you finish that you can then come back to Computer Systems: A Programmers Perspective.

## Data Structures and Algorithms

![image-131](https://www.freecodecamp.org/news/content/images/2023/06/image-131.png)

[Source][37]

Everyone wants to work at a FAANG company, but no one wants to learn Data Structures and Algorithms.

Nevertheless, I don't want you to learn these just because of technical interviews. Data structures and algorithms are important because they help build your problem solving skills.

There are many great books and courses on Data Structures and Algorithms but the one I would recommend is a book named _[The Algorithm Design Manual][38]_ by Steven Skiena. You can also check out his course [here][39].

### Don't forget to practice

Same rules apply here. Don't just learn about data structures, but create them in whatever language you want. Don't just memorize algorithms but implement them and see where and how you can use them.

A good tip is solving some [Leetcode][40] problems while going through the book/course.

### What if I find it too hard?

If you find the material a bit heavy, then I would recommend the following resources:

-   Read the book: [Grokking Algorithms][41]
-   Read the book: [How to Solve It: A New Aspect of Mathematical Method][42]

In general there are many different books/courses that teach Data Structures and Algorithms – Here are some other great resources:

-   [Data Structures and Algorithms course on freeCodeCamp][43]
-   [Algorithms Illuminated][44]
-   [Princeton Algorithms Course][45]
-   [ThePrimegeans Data Structures and Algorithms Course][46]
-   [MIT Introduction to Algorithms][47]

## Math for Computer Science

![image-144](https://www.freecodecamp.org/news/content/images/2023/06/image-144.png)

Don't worry, this is some random math photo found [here][48]

Many new developers skip this.

But, hear me out – computer science is essentially a branch of mathematics. Learning it will make you a better developer by honing your problem solving skills.

### The most relevant area for CS is Discrete Mathematics

Discrete mathematics is the branch of mathematics that deals with countable or finite numbers.

The topics in discrete mathematics are many, but the ones which are relevant for CS are:

-   Logic
-   Combinatorics
-   Discrete Probability
-   Set Theory
-   Graph Theory
-   Number Theory

### How to Study Discrete Mathematics

I would suggest starting with a set of [lecture notes by László Lovász][49].

Professor Lovász notes are easier to digest than formal texts and are just generally fun. He starts of with a problem and solves it using discrete mathematics.

After that, you can take an MIT book called _[Mathematics for Computer Science][50]._ The book comes with video lectures that are [freely available][51].

### What if it's too hard?

Don't worry – sometimes you just have to accept that **you won't always get it right away**.

It's fine.

But if you feel like you're missing some fundamental knowledge, then it's a different story. The fundamental prerequisite subjects for discrete mathematics are:

-   Algebra
-   Geometry
-   Calculas

There are many free resources, but the ones I would recommend are:

-   [Khan Academy][52]
-   [College Algebra course][53]
-   [Calculus 1 course][54]
-   [Calculus 2 course][55]

## Operating Systems

![image-228](https://www.freecodecamp.org/news/content/images/2023/06/image-228.png)

[Source][56]

Remember when I told you that we as developers want to remove the magic in computing?

Same thing applies here – operating systems seem like some sort of magical black box. But they're not – it's just a lot of clever engineering.

If you know how these operating systems are built and work, then you will definitely be in a league of your own.

It's somewhat difficult to find good resources online for operating systems but the most recommend book is [Operating Systems: Three Easy Pieces (OSTEP).][57] There isn't any official video lecture online that fully covers the book but I found this [playlist on YouTube][58].

### Recommend Prerequisites

I would suggest learning computer architecture first and a little bit about C before embarking on the operating systems journey.

### Optional Resources

Now, I recommend finishing OSTEP first and then checking out the other recommend resources. They are all optional.

-   Want to build your own Linux system? Check out [Linux from Scratch][59].
-   Want an in-depth overview of Linux, MacOS, and Windows? [Here's a handbook for you][60].
-   Want to build your own OS? Check out [OSDEV][61]
-   Want to build your own Sockets? Check out [Beej's Guide to Network Programming][62]

## Computer Networking

![image-237](https://www.freecodecamp.org/news/content/images/2023/06/image-237.png)

[Source][63]

Since the dawn of the internet, computer networking has been one the most important subjects for software engineers.

If you don't know things like IP, TCP, UDP, HTTP, TLS, DNS, SMTP, and so on — then you should learn about computer networking (especially if you are a backend engineer).

The recommended book here is [Computer Networking: A Top-Down Approach][64]. You can also check out the [video lectures][65] from the author of the book himself.

But before beginning that I would recommend to check out this [video crash course on computer networking][66] from a bottom up approach. And [here's a helpful tutorial][67] that covers the basics well.

## Databases

![image-229](https://www.freecodecamp.org/news/content/images/2023/06/image-229.png)

[Source][68]

Databases are somewhat new – they came around the 1970s and have since become integral parts of many applications.

I highly recommend the below courses from the [CMU Database Group][69]. They're all freely available on YouTube. I would recommend going through at least the first one.

1.  [Introduction To Databases][70]
2.  [Database Seminars][71]
3.  [Advanced Databases][72]

Also, [here's a great collection of resources][73] to help you learn about SQL databases. And [here's a free course on NoSQL databases][74].

## Languages and Compilers

![image-230](https://www.freecodecamp.org/news/content/images/2023/06/image-230.png)

[Source][75]

You may know how to code in one or more programming languages.

But do you know how to create or design one? That's what you will learn by studying programming languages and compilers.

The recommended introductory book is called [Crafting Interpreters][76].

After that you can move on to _[Compilers: Principles, Techniques & Tools][77]_, also called “the Dragon Book”. The book is covers a lot of topics so I highly recommend taking a course with it. The one I recommend is from [Alex Aiken on edX][78].

And [here's a helpful beginner-friendly tutorial][79] on how the compiler works in C programming.

## Distributed Systems

![image-231](https://www.freecodecamp.org/news/content/images/2023/06/image-231.png)

[Source][80]

If you choose to study only one subject from the list, make it distributed systems. It's the holy grail for tech companies, and if you want to get a developer job, you should be proficient about distributed systems.

My recommend path in learning the subject is:

1.  Read the book: [Understanding Distributed Systems][81]
2.  Read the book: [Designing Data Intensive Applications][82] also known as the "red book"
3.  While reading the "red book", take its accompanying [MIT course on YouTube][83].
4.  Read the book: [Software Architecture: The Hard Parts][84] (Optional)
5.  You can also [check out my handbook about design patterns for distributed systems][85].

## Web Security

![image-232](https://www.freecodecamp.org/news/content/images/2023/06/image-232.png)

[Source][86]

There have been a lot of security breaches in the last 2-3 years.

It's getting dangerous out there – and as a software engineer, knowing some fundamentals of web security will give you an edge.

The course I recommend first is [CS253 Web Security by Stanford][87]. It gives a comprehensive overview of web security. So expect topics like web app vulnerabilities, injection, denial-of-service, and many more.

You can also [review these common vulnerabilities][88] and learn how to prevent attacks that take advantage of them.

Later on, if you want, you could learn how to hack using [pwn.college][89].

## Conclusion

Learning all these subjects will take you a while, and will require consistent effort. But if you like what you do and are interested in the subject, then it should feel like play and not a chore.

Regardless of the subjects you choose to study. The most important tip I can give you is...

### Don't be a passive learner

Don't just watch videos – do the exercises as well. Build the projects along with the tutorials.

Don't just read books but engage in the book by asking questions and doing your own research.

You want the information to stick, so you don't forget it. And to make it stick you have to actively engage in the subject.

I sincerely hope that I encouraged you to study some of these subjects. As always I want to end it of by thanking you for reading this article.

I wish you all the best.

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