---
title: 子网备忘单 – 24 子网掩码, 30, 26, 27, 29 及其他 IP 地址 CIDR 网络参考
date: 2024-08-12T01:47:09.067Z
author: Kristofer Koishigawa
authorURL: https://www.freecodecamp.org/news/author/scissorsneedfoodtoo/
originalURL: https://www.freecodecamp.org/news/subnet-cheat-sheet-24-subnet-mask-30-26-27-29-and-other-ip-address-cidr-network-references/
translator: ""
reviewer: ""
---

作为一名开发者或网络工程师，你可能需要时不时地查找子网掩码的值并弄清它们的含义。

<!-- more -->

为了让你的生活更轻松，freeCodeCamp 社区制作了这个简单的备忘单。只需滚动或使用 Ctrl/Cmd + F 查找你要找的值。

这里是图表，后面是一些解释它们含义的内容。

| CIDR | 子网掩码 | 通配符掩码 | IP 地址数量 | 可用 IP 地址数量 |
| --- | --- | --- | --- | --- |
| /32 | 255.255.255.255 | 0.0.0.0 | 1 | 1 |
| /31 | 255.255.255.254 | 0.0.0.1 | 2 | 2\* |
| /30 | 255.255.255.252 | 0.0.0.3 | 4 | 2 |
| /29 | 255.255.255.248 | 0.0.0.7 | 8 | 6 |
| /28 | 255.255.255.240 | 0.0.0.15 | 16 | 14 |
| /27 | 255.255.255.224 | 0.0.0.31 | 32 | 30 |
| /26 | 255.255.255.192 | 0.0.0.63 | 64 | 62 |
| /25 | 255.255.255.128 | 0.0.0.127 | 128 | 126 |
| /24 | 255.255.255.0 | 0.0.0.255 | 256 | 254 |
| /23 | 255.255.254.0 | 0.0.1.255 | 512 | 510 |
| /22 | 255.255.252.0 | 0.0.3.255 | 1,024 | 1,022 |
| /21 | 255.255.248.0 | 0.0.7.255 | 2,048 | 2,046 |
| /20 | 255.255.240.0 | 0.0.15.255 | 4,096 | 4,094 |
| /19 | 255.255.224.0 | 0.0.31.255 | 8,192 | 8,190 |
| /18 | 255.255.192.0 | 0.0.63.255 | 16,384 | 16,382 |
| /17 | 255.255.128.0 | 0.0.127.255 | 32,768 | 32,766 |
| /16 | 255.255.0.0 | 0.0.255.255 | 65,536 | 65,534 |
| /15 | 255.254.0.0 | 0.1.255.255 | 131,072 | 131,070 |
| /14 | 255.252.0.0 | 0.3.255.255 | 262,144 | 262,142 |
| /13 | 255.248.0.0 | 0.7.255.255 | 524,288 | 524,286 |
| /12 | 255.240.0.0 | 0.15.255.255 | 1,048,576 | 1,048,574 |
| /11 | 255.224.0.0 | 0.31.255.255 | 2,097,152 | 2,097,150 |
| /10 | 255.192.0.0 | 0.63.255.255 | 4,194,304 | 4,194,302 |
| /9 | 255.128.0.0 | 0.127.255.255 | 8,388,608 | 8,388,606 |
| /8 | 255.0.0.0 | 0.255.255.255 | 16,777,216 | 16,777,214 |
| /7 | 254.0.0.0 | 1.255.255.255 | 33,554,432 | 33,554,430 |
| /6 | 252.0.0.0 | 3.255.255.255 | 67,108,864 | 67,108,862 |
| /5 | 248.0.0.0 | 7.255.255.255 | 134,217,728 | 134,217,726 |
| /4 | 240.0.0.0 | 15.255.255.255 | 268,435,456 | 268,435,454 |
| /3 | 224.0.0.0 | 31.255.255.255 | 536,870,912 | 536,870,910 |
| /2 | 192.0.0.0 | 63.255.255.255 | 1,073,741,824 | 1,073,741,822 |
| /1 | 128.0.0.0 | 127.255.255.255 | 2,147,483,648 | 2,147,483,646 |
| /0 | 0.0.0.0 | 255.255.255.255 | 4,294,967,296 | 4,294,967,294 |

- /31 是 [RFC 3021][1] 中详细说明的一种特殊情况，这种子网掩码类型的网络可以分配两个 IP 地址作为点对点链路。

这里是一张子网掩码和通配符八位字节的十进制到二进制转换表：

|  | 子网掩码 |  | 通配符 |
| --- | --- | --- | --- |
| 0 | 00000000 | 255 | 11111111 |
| 128 | 10000000 | 127 | 01111111 |
| 192 | 11000000 | 63 | 00111111 |
| 224 | 11100000 | 31 | 00011111 |
| 240 | 11110000 | 15 | 00001111 |
| 248 | 11111000 | 7 | 00000111 |
| 252 | 11111100 | 3 | 00000011 |
| 254 | 11111110 | 1 | 00000001 |
| 255 | 11111111 | 0 | 00000000 |

请注意，通配符只是子网掩码的反码。

如果你是网络工程的新手，可以[在这里更好地了解计算机网络的工作原理][2]。

最后，这个备忘单和整篇文章都集中在 IPv4 地址上，而不是较新的 IPv6 协议。如果你想了解更多关于 IPv6 的信息，请查看上面提到的那篇关于计算机网络的文章。

## IP 地址块如何工作？

像 `192.168.0.1` 这样的 IPv4 地址实际上只是四个二进制块的十进制表示。

每个块都是 8 位，代表 0-255 之间的数字。由于这些块是 8 位的组，每个块被称为一个**八位字节**。因为有四个 8 位块，每个 IPv4 地址是 32 位。

例如，这里是 IP 地址 `172.16.254.1` 的二进制表示：

![Image](https://www.freecodecamp.org/news/content/images/2021/03/1125px-Ipv4_address.png) _来源：[IPv4][3]_

要在十进制和二进制形式之间转换 IP 地址，你可以使用这个图表：

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| x | x | x | x | x | x | x | x |

上面的图表代表一个 8 位八位字节。

现在假设你想转换 IP 地址 `168.210.225.206`。你只需将地址分解为四个块（`168`, `210`, `225` 和 `206`），并使用上面的图表将每个块转换为二进制。

记住在二进制中，1 等价于“开”，0 等价于“关”。所以，要将第一个块 `168` 转换为二进制，只需从图表的开头开始，在每个单元格中放置 1 或 0，直到得到 `168` 的和。

例如：

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 0 | 1 | 0 | 1 | 0 | 0 | 0 |

128 + 32 + 8 = 168，二进制表示为 `10101000`。

## 什么是子网划分？

如果查看上面的表格，可能会觉得 IP 地址的数量几乎是无限的。毕竟，有将近 42 亿个可用的 IPv4 地址。

但是，考虑到互联网的增长速度，以及如今连接的设备数量，听到已经存在的 [IPv4 地址短缺][4] 可能并不令人惊讶。

由于多年前就已意识到这一短缺，开发人员提出了一种将 IP 地址拆分为较小网络的方法，称为子网。

这个过程叫子网划分，使用 IP 地址的主机部分将其分解为那些较小的网络或子网。

通常，一个 IP 地址由网络位和主机位组成：

 ![Image](https://www.freecodecamp.org/news/content/images/2021/03/network-and-host-bits.png) _来源: [什么是 IPv4][5]_

因此，通常来说，子网划分做了两件事：它为我们提供了一种将网络拆分为子网的方法，并允许设备确定另一个设备/IP 地址是否在同一个本地网络上。

一个理解子网划分的好方法是想象一下你家里的无线网络。

如果没有子网划分，每个连接到互联网的设备都需要有自己唯一的 IP 地址。

但是，由于你有一个无线路由器，你只需要为路由器分配一个 IP 地址。这个公共或外部 IP 地址通常是自动处理的，由你的互联网服务提供商 (ISP) 分配。

然后，每个连接到该路由器的设备都有自己的私人或内部 IP 地址：

![Image](https://www.freecodecamp.org/news/content/images/2021/03/home-network-diagram.png) _来源: [我的 IP 地址是什么？][6]_

现在，如果你的设备内部 IP 地址 `192.168.1.101` 想要与另一个设备通信，它会使用另一个设备的 IP 地址和子网掩码。

IP 地址和子网掩码的组合允许 `192.168.1.101` 设备确定另一个设备是否在同一网络（比如 `192.168.1.103` 设备），或在网上别处的完全不同的网络上。

有趣的是，你的 ISP 分配给路由器的外部 IP 地址可能是子网的一部分，可能包括附近家庭或企业的许多其他 IP 地址。而且就像内部 IP 地址一样，它也需要一个子网掩码才能正常工作。

### 子网掩码如何工作

子网掩码充当 IP 地址的一种过滤器。有了子网掩码，设备可以查看 IP 地址，并找出哪些部分是网络位，哪些是主机位。

然后使用这些东西，它可以找出这些设备通信的最佳方式。

如果你曾在路由器或电脑上的网络设置中闲逛过，你可能见过这个数字: `255.255.255.0`。

如果是这样，你看到了一个非常常见的简单家庭网络的子网掩码。

像 IPv4 地址一样，子网掩码也是 32 位的。就像将 IP 地址转换为二进制一样，你也可以对子网掩码进行相同的操作。

例如，这是我们早期的图表：

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| x | x | x | x | x | x | x | x |

现在转换第一个八位字节，255：

| 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 |

很简单，对吧？所以任何八位字节是 `255` 就是二进制的 `11111111`。这意味着 `255.255.255.0` 其实是二进制的 `11111111.11111111.11111111.00000000`。

现在我们一起看看子网掩码和 IP 地址，并计算 IP 地址的哪些部分是网络位和主机位。

下面是两者的十进制和二进制表示：

| 类型 | 十进制 | 二进制 |
| --- | --- | --- |
| IP 地址 | 192.168.0.101 | 11000000.10101000.00000000.01100101 |
| 子网掩码 | 255.255.255.0 | 11111111.11111111.11111111.00000000 |

通过这种方式排列的两个地址，很容易将 `192.168.0.101` 分为网络位和主机位。

每当二进制子网掩码中的一位是 1，则二进制 IP 地址中的相同位就是网络的一部分，而不是主机。

由于八位字节 `255` 在二进制中是 `11111111`，因此 IP 地址中的整个八位字节都是网络的一部分。所以前三个八位字节 `192.168.0` 是 IP 地址的网络部分，而 `101` 是主机部分。

换句话说，如果 `192.168.0.101` 设备想要与另一台设备通信，使用子网掩码，它知道任何带有 IP 地址 `192.168.0.xxx` 是在同一个本地网络上。

另一种表达方式是用网络 ID，这只是 IP 地址的网络部分。因此，具有子网掩码 `255.255.255.0` 的地址 `192.168.0.101` 的网络 ID 是 `192.168.0.0`。

对本地网络上的其他设备 (`192.168.0.102`，`192.168.0.103` 等等) 也是如此。

### CIDR 是什么，CIDR 表示法是什么？

**CIDR** 代表无类域间路由，用于 IPv4 以及最近的 IPv6 路由。

![Image](https://www.freecodecamp.org/news/content/images/2020/05/1920px-IP_Address_Match.svg.png) _来源: [无类域间路由][7]_

CIDR 包含几个主要概念。

第一个是可变长度子网掩码（VLSM），它基本上允许网络工程师在子网中创建子网。这些子网可以是不同大小的，因此可以减少未使用的 IP 地址。

CIDR 引入的第二个主要概念是 CIDR 表示法。

CIDR 表示法实际上只是子网掩码的简写，表示 IP 地址可用的位数。例如，`192.168.0.101/24` 中的 `/24` 相当于 IP 地址 `192.168.0.101` 和子网掩码 `255.255.255.0`。

### 如何计算 CIDR 表示法

要确定给定子网掩码的 CIDR 表示法，只需将子网掩码转换为二进制，然后数出其中的 1 或“开”位数。例如：

| 类型 | 十进制 | 二进制 |
| --- | --- | --- |
| 子网掩码 | 255.255.255.0 | 11111111.11111111.11111111.00000000 |

由于有三个八位字节的 1，因此有 24 个“开”位，这意味着 CIDR 表示法是 `/24`。

你可以用任意一种方式书写，但我相信你会同意 `/24` 比 `255.255.255.0` 更容易书写。

这通常与 IP 地址一起进行的，所以让我们来看一下具有 IP 地址的相同子网掩码：

| 类型 | 十进制 | 二进制 |
| --- | --- | --- |
| IP 地址 | 192.168.0.101 | 11000000.10101000.00000000.01100101 |
| 子网掩码 | 255.255.255.0 | 11111111.11111111.11111111.00000000 |

子网掩码的前三个八位字节都是“开”位，因此意味着 IP 地址的相同三个八位字节都是网络位。

让我们更详细地看看最后一个第四个八位字节：

| 类型 | 十进制 | 二进制 |
| --- | --- | --- |
| IP 地址 | 101 | 01100101 |
| 子网掩码 | 0 | 00000000 |

在这种情况下，因为子网掩码的这个八位字节的所有位都是“关”的，我们可以确定 IP 地址中这个八位字节的所有对应位都是主机的一部分。

当你书写 CIDR 表示法时，通常使用网络 ID。因此，带有子网掩码 `255.255.255.0` 的 IP 地址 `192.168.0.101` 的 CIDR 表示法是 `192.168.0.0/24`。

要查看更多如何计算给定 IP 地址和子网掩码的 CIDR 表示法和网络 ID 的示例，请查看此视频：

<iframe width="560" height="315" src="https://www.youtube.com/embed/XQ3T14SIlV4" style="aspect-ratio: 16 / 9; width: 100%; height: auto;" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen="" loading="lazy"></iframe>

## 类 IP 地址

现在我们已经讨论了一些子网和 CIDR 的基本示例，让我们放大看看所谓的类 IP 地址。

在开发子网之前，所有 IP 地址都属于特定的类：

![Image](https://www.freecodecamp.org/news/content/images/2021/03/subnetting.png) _Source: [Subnetting for dummies][8]_

注意还有 D 类和 E 类 IP 地址，但我们稍后会更详细地介绍这些。

类 IP 地址为网络工程师提供了一种为不同组织提供一系列有效 IP 地址的方法。

这种方法有很多问题，最终导致了子网的产生。但在我们深入了解这些问题之前，让我们仔细看看不同的类。

### A 类 IP 地址

对于 A 类 IP 地址，第一个八位字节（8 位 / 1 字节）表示网络 ID，剩下的三个八位字节（24 位 / 3 字节）是主机 ID。

A 类 IP 地址的范围是 `1.0.0.0` 到 `127.255.255.255`，默认掩码是 `255.0.0.0`（或 CIDR 中的 `/8`）。

这意味着 A 类寻址可以有 128（27）个网络和每个网络 16,777,214（224-2）个可用地址。

还要注意在 A 类范围内 `127.0.0.0` 到 `127.255.255.255` 的范围保留给主机回环地址（参见 [RFC5735][9]）。

### B 类 IP 地址

对于 B 类 IP 地址，前两个八位字节（16 位 / 2 字节）表示网络 ID，剩下的两个八位字节（16 位 / 2 字节）是主机 ID。

B 类 IP 地址的范围是 `128.0.0.0` 到 `191.255.255.255`，默认子网掩码是 `255.255.0.0`（或 CIDR 中的 `/16`）。

B 类寻址可以有 16,384 (214) 个网络地址和每个网络 65,534 (216) 个可用地址。

### C 类 IP 地址

对于 C 类 IP 地址，前三个八位字节（24 位 / 3 字节）表示网络 ID，最后一个八位字节（8 位 / 1 字节）是主机 ID。

C 类 IP 地址的范围是 `192.0.0.0` 到 `223.255.255.255`，默认子网掩码是 `255.255.255.0`（或 CIDR 中的 `/24`）。

C 类对应 2,097,152 (221) 个网络和每个网络 254 (28-2) 个可用地址。

### D 类和 E 类 IP 地址

最后两类是 D 类和 E 类。

D 类 IP 地址保留用于多播。它们的范围是 `224.0.0.0` 到 `239.255.255.255`。

E 类 IP 地址是实验性的，超过 `240.0.0.0` 的任何地址都属于 E 类。

### 类 IP 地址的问题

类 IP 地址的主要问题是它并不高效，并且可能导致大量 IP 地址浪费。

但是，如果你往上看，你会发现一个B类网络可以支持多达65,534个可用地址。即使每个员工都有多个具有唯一地址的设备，这也远远超出了你们组织的需求。

而且你的组织完全不可能回落到C类网络——可用的IP地址根本不够。

因此，虽然在IPv4地址广泛使用的时期使用的是类IP地址，但很快就清楚需要一个更好的系统，以确保我们不会用完大约42亿个可用地址。

自从1993年CIDR取代它们以来，就不再使用类IP地址，主要是为了理解早期的互联网架构以及为什么子网是重要的。

## 我希望这张备忘单对你有帮助

如果你觉得有帮助，请与朋友分享，让更多人受益。

此外，随时可以在 [Twitter][10] 上联系我们，告诉我你的想法。

---

![Kristofer Koishigawa](https://cdn.hashnode.com/res/hashnode/image/upload/v1710857138258/qSuNPwWGp.jpeg)

阅读[更多文章][11]。

---

如果你读到这里，请向作者表示感谢，让他们知道你在乎。说声谢谢

免费学习编程。freeCodeCamp的开源课程已经帮助超过40,000人获得了开发者的工作。[现在开始][12]

[1]: https://tools.ietf.org/html/rfc3021
[2]: https://www.freecodecamp.org/news/computer-networks-and-how-to-actually-understand-them-c1401908172d/
[3]: https://en.wikipedia.org/wiki/IPv4
[4]: https://whatismyipaddress.com/ipv4-shortage
[5]: https://support.huawei.com/enterprise/en/doc/EDOC1100145159
[6]: https://www.popularmechanics.com/technology/a32729384/how-to-find-ip-address/
[7]: https://en.wikipedia.org/wiki/Classless_Inter-Domain_Routing
[8]: https://community.spiceworks.com/networking/articles/2489-subnetting-for-dummies
[9]: https://tools.ietf.org/html/rfc5735
[10]: https://twitter.com/kriskoishigawa
[11]: /news/author/scissorsneedfoodtoo/
[12]: https://www.freecodecamp.org/learn/

