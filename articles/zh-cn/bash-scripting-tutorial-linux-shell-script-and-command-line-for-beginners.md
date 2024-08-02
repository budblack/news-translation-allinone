---
title: Bash 脚本教程 – 初学者的 Linux Shell 脚本和命令行指南
date: 2024-08-02T08:22:53.260Z
author: Zaira Hira
authorURL: https://www.freecodecamp.org/news/author/zaira/
originalURL: https://www.freecodecamp.org/news/bash-scripting-tutorial-linux-shell-script-and-command-line-for-beginners/
translator: ""
reviewer: ""
---

在 Linux 中，流程自动化在很大程度上依赖于 shell 脚本。这涉及到创建一个包含一系列命令的文件，这些命令可以一起执行。

<!-- more -->

在本文中，我们将从 bash 脚本编写的基础知识开始，包括变量、命令、输入/输出和调试。我们还会沿途看到每个示例。

让我们开始吧。🚀

## 目录

1.  [前提条件][1]
2.  [简介][2]

-   [Bash 脚本的定义][3]
-   [Bash 脚本的优点][4]
-   [Bash Shell 和命令行界面的概述][5]

3.  [如何开始 Bash 脚本编写][6]

-   [如何从命令行运行 Bash 命令][7]
-   [如何创建和执行 Bash 脚本][8]

4.  [Bash 脚本基础知识][9]

-   [Bash 脚本中的注释][10]
-   [Bash 中的变量和数据类型][11]
-   [Bash 脚本中的输入和输出][12]
-   [基本的 Bash 命令（echo、read 等）][13]
-   [条件语句（if/else）][14]

5.  [Bash 中的循环和分支][15]

-   [while 循环][16]
-   [for 循环][17]
-   [case 语句][18]

6.  [如何使用 cron 调度脚本][19]
7.  [如何调试和排除 Bash 脚本的故障][20]
8.  [结论][21]

-   [学习更多关于 Bash 脚本的资源][22]

## 前提条件

为了跟随本教程的进度，你应具备以下条件：

-  具有访问命令行的运行中的 Linux 版本。

如果你没有安装 Linux 或者你是初学者，你可以很容易通过 [Replit][23] 访问 Linux 命令行。Replit 是一个基于浏览器的 IDE，你可以在几分钟内访问 bash shell。

你也可以通过 WSL（Windows Subsystem for Linux）在你的 Windows 系统上安装 Linux。[这里][24] 有一个相关教程。

## 简介

### Bash 脚本的定义

Bash 脚本是一个包含一系列命令的文件，这些命令由 bash 程序逐行执行。它允许你通过命令行执行一系列操作，如导航到特定目录、创建文件夹和启动进程。

通过将这些命令保存在脚本中，你可以多次重复相同的操作，并通过运行脚本执行它们。

### Bash 脚本的优点

Bash 脚本是一种强大且灵活的工具，可以用于自动化系统管理任务、管理系统资源以及在 Unix/Linux 系统中执行其他例行任务。Shell 脚本的一些优点包括：

-   **自动化**：Shell 脚本允许你自动化重复性任务和过程，节省时间并减少手动执行时可能出现的错误。
-   **可移植性**：Shell 脚本可以在各种平台和操作系统上运行，包括 Unix、Linux、macOS，甚至通过使用模拟器或虚拟机在 Windows 上运行。
-   **灵活性**：Shell 脚本高度可定制，可以轻松修改以满足特定需求。它们还可以与其他编程语言或实用程序结合，创建更强大的脚本。
-   **易访问性**：Shell 脚本易于编写，不需要任何特殊工具或软件。它们可以使用任何文本编辑器进行编辑，并且大多数操作系统都有内置的 shell 解释器。
-   **集成**：Shell 脚本可以与其他工具和应用程序集成，如数据库、Web 服务器和云服务，从而实现更复杂的自动化和系统管理任务。
-   **调试**：Shell 脚本易于调试，大多数 shell 都内置调试和错误报告工具，可以帮助快速识别和修复问题。

### Bash Shell 和命令行界面的概述

"Shell" 和 "bash" 这两个术语可以互换使用。但两者之间有细微的区别。

"Shell" 这个术语是指提供命令行界面以与操作系统交互的程序。Bash（Bourne-Again SHell）是最常用的 Unix/Linux shell 之一，并且是许多 Linux 发行版中的默认 shell。

Shell 或命令行界面看起来是这样的：

![image-135](https://www.freecodecamp.org/news/content/images/2023/03/image-135.png)

Shell 接收用户的命令并显示输出。

在上述输出中，`zaira@Zaira` 是 shell 提示符。当 shell 以交互方式使用时，在等待用户命令时会显示一个 `$`。

如果 shell 以 root（具有管理权的用户）身份运行，提示符会变为 `#`。超级用户 shell 提示符看起来是这样的：

```bash
[root@host ~]#
```

尽管 Bash 是一种类型的 shell，还有其他 shell 可用，如 Korn shell (ksh)、C shell (csh) 和 Z shell (zsh)。每种 shell 都有其自己的语法和功能集，但它们都有提供命令行界面以与操作系统交互的共同目的。



```bash
ps
```

这是我的输出结果：

![image-134](https://www.freecodecamp.org/news/content/images/2023/03/image-134.png)

检查 shell 类型。我使用的是 bash shell

总结一下，虽然“shell”是指任何提供命令行界面的程序的一个广泛术语，但“Bash”是一种特定类型的 shell，在 Unix/Linux 系统中广泛使用。

注意：在本教程中，我们将使用 "bash" shell。

## 如何开始使用 Bash 脚本编写

### 从命令行运行 Bash 命令

如前所述，shell 提示符看起来像这样：

```bash
[username@host ~]$
```

您可以在 `$` 符号后输入任何命令，并在终端上看到输出。

通常，命令遵循以下语法：

```
command [选项] 参数
```

让我们讨论一些基本的 bash 命令并查看它们的输出。确保跟着做哦 :)

- `date`：显示当前日期

```bash
zaira@Zaira:~/shell-tutorial$ date
Tue Mar 14 13:08:57 PKT 2023
```

- `pwd`：显示当前工作目录。

```bash
zaira@Zaira:~/shell-tutorial$ pwd
/home/zaira/shell-tutorial
```

- `ls`：列出当前目录的内容。

```bash
zaira@Zaira:~/shell-tutorial$ ls
check_plaindrome.sh  count_odd.sh  env  log  temp
```

- `echo`：打印一段文本或变量的值到终端。

```bash
zaira@Zaira:~/shell-tutorial$ echo "Hello bash"
Hello bash
```

您可以始终使用 `man` 命令查看命令手册。

例如，`ls` 的手册看起来像这样：

![image-138](https://www.freecodecamp.org/news/content/images/2023/03/image-138.png)

您可以使用 `man` 命令详细查看命令的选项

### 如何创建和执行 Bash 脚本

#### 脚本命名约定

按照惯例，bash 脚本以 `.sh` 结尾。然而，即使没有 `sh` 扩展名，bash 脚本也可以正常运行。

#### 添加 Shebang

Bash 脚本以 `shebang` 开头。Shebang 是 `bash #` 和 `bang !` 的组合，后跟 bash shell 路径。这是脚本的第一行。Shebang 告诉 shell 通过 bash shell 执行它。Shebang 仅仅是 bash 解释器的绝对路径。

以下是 shebang 语句的示例。

```bash
#!/bin/bash
```

您可以使用以下命令找到您的 bash shell 路径（可能与上述路径不同）：

```bash
which bash
```

#### 创建我们的第一个 bash 脚本

我们的第一个脚本提示用户输入路径。然后，它将列出路径的内容。

使用 `vi` 命令创建一个名为 `run_all.sh` 的文件。您可以使用任何您喜欢的编辑器。

```bash
vi run_all.sh
```

在文件中添加以下命令并保存：

```bash
#!/bin/bash
echo "今天是 " `date`

echo -e "\n请输入目录路径"
read the_path

echo -e "\n 你的路径包含以下文件和文件夹："
ls $the_path
```

打印用户提供的目录内容的脚本

让我们逐行仔细看看脚本。我将再次显示相同的脚本，但这次带有行号。

```bash
  1 #!/bin/bash
  2 echo "今天是 " `date`
  3
  4 echo -e "\n请输入目录路径"
  5 read the_path
  6
  7 echo -e "\n 你的路径包含以下文件和文件夹："
  8 ls $the_path
```

- 第 1 行：Shebang (`#!/bin/bash`) 指向 bash shell 路径。
- 第 2 行：`echo` 命令在终端显示当前日期和时间。注意 `date` 在反引号中。
- 第 4 行：我们希望用户输入一个有效的路径。
- 第 5 行：`read` 命令读取输入并将其存储在变量 `the_path` 中。
- 第 8 行：`ls` 命令使用存储路径的变量并显示当前的文件和文件夹。

#### 执行 bash 脚本

为了使脚本可执行，请使用以下命令为您的用户分配执行权限：

```bash
chmod u+x run_all.sh
```

这里，

- `chmod` 修改文件的所有权以供当前用户使用：`u`。
- `+x` 将执行权限添加到当前用户。这意味着作为所有者的用户现在可以运行该脚本。
- `run_all.sh` 是我们希望运行的文件。

您可以使用下列任何方法运行脚本：

- `sh run_all.sh`
- `bash run_all.sh`
- `./run_all.sh`

让我们看看它在运行中的样子 🚀

![run-script-bash-2](https://www.freecodecamp.org/news/content/images/2023/03/run-script-bash-2.gif)

## Bash 脚本基础

### Bash 脚本中的注释

Bash 脚本中的注释以 `#` 开头。这意味着任何以 `#` 开头的行都是注释，将被解释器忽略。

注释对于文档编写非常有帮助，并且是帮助他人理解代码的一个好习惯。

以下是注释的示例：

```bash
# 这是一个示例注释
# 这两行将被解释器忽略
```

### Bash 中的变量和数据类型

变量让您存储数据。您可以在脚本中使用变量读取、访问和操作数据。

Bash 中没有数据类型。在 Bash 中，变量能够存储数值、单个字符或字符串。

在 Bash 中，您可以通过以下方式使用和设置变量值：
```

```bash
country=Pakistan
```

2\.  根据从程序或命令获取的输出，使用命令替换赋值。请注意，$ 是访问现有变量值所需的。

```bash
same_country=$country
```

这会将 `country` 的值赋给新变量 `same_country`

要访问变量值，请在变量名称后附加 `$`。

```bash
zaira@Zaira:~$ country=Pakistan
zaira@Zaira:~$ echo $country
Pakistan
zaira@Zaira:~$ new_country=$country
zaira@Zaira:~$ echo $new_country
Pakistan
```

赋值和打印变量值

### 变量命名规范

在 Bash 脚本中，以下是变量命名规范：

1. 变量名称应以字母或下划线 (`_`) 开头。
2. 变量名称可以包含字母、数字和下划线 (`_`)。
3. 变量名称区分大小写。
4. 变量名称不应包含空格或特殊字符。
5. 使用能反映变量用途的描述性名称。
6. 避免使用保留关键字（如 `if`, `then`, `else`, `fi` 等）作为变量名称。

以下是一些合法变量名称的示例：

```bash
name
count
_var
myVar
MY_VAR
```

以下是一些非法变量名称的示例：

```bash
2ndvar (变量名称以数字开头)
my var (变量名称包含空格)
my-var (变量名称包含连字符)
```

遵循这些命名规范有助于使 Bash 脚本更具可读性和易于维护。

### Bash 脚本中的输入和输出

#### 收集输入

在本节中，我们将讨论一些为脚本提供输入的方法。

1. 读取用户输入并将其存储在变量中

我们可以使用 `read` 命令读取用户输入。

```bash
#!/bin/bash 

echo "What's your name?" 

read entered_name 

echo -e "\nWelcome to bash tutorial" $entered_name
```

![name-sh](https://www.freecodecamp.org/news/content/images/2023/03/name-sh.gif)

2\.  从文件读取

此代码从名为 `input.txt` 的文件中读取每一行并将其打印到终端。我们将在本文稍后学习 while 循环。

```bash
while read line
do
  echo $line
done < input.txt
```

3\.  命令行参数

在 bash 脚本或函数中，`$1` 表示传递的初始参数，`$2` 表示传递的第二个参数，以此类推。

此脚本将名字作为命令行参数并打印个性化问候语。

```bash
echo "Hello, $1!"
```

我们将 `Zaira` 作为参数提供给脚本。

```bash
#!/bin/bash
echo "Hello, $1!"
```

脚本代码：`greeting.sh`

**输出：**

![name-sh-1](https://www.freecodecamp.org/news/content/images/2023/03/name-sh-1.gif)

#### 显示输出

这里我们将讨论一些从脚本接收输出的方法。

1. 打印到终端：

```bash
echo "Hello, World!"
```

这会将文本 "Hello, World!" 打印到终端。

2\.  写入文件：

```bash
echo "This is some text." > output.txt
```

这会将文本 "This is some text." 写入名为 `output.txt` 的文件。请注意，`>` 操作符会覆盖文件内容（如果文件已存在）。

3\.  追加到文件：

```bash
echo "More text." >> output.txt
```

这会将文本 "More text." 追加到 `output.txt` 文件的末尾。

4\.  重定向输出：

```bash
ls > files.txt
```

这会列出当前目录中的文件并将输出写入名为 `files.txt` 的文件。您可以通过这种方式将任何命令的输出重定向到文件。

### 基本 Bash 命令（echo, read 等）

以下是一些最常用的 bash 命令列表：

1.  `cd`: 切换到不同目录。
2.  `ls`: 列出当前目录的内容。
3.  `mkdir`: 创建新目录。
4.  `touch`: 创建新文件。
5.  `rm`: 删除文件或目录。
6.  `cp`: 复制文件或目录。
7.  `mv`: 移动或重命名文件或目录。
8.  `echo`: 将文本打印到终端。
9.  `cat`: 连接并打印文件内容。
10.  `grep`: 在文件中搜索模式。
11.  `chmod`: 更改文件或目录的权限。
12.  `sudo`: 以管理权限运行命令。
13.  `df`: 显示可用磁盘空间。
14.  `history`: 显示先前执行的命令列表。
15.  `ps`: 显示有关正在运行的进程的信息。

### 条件语句（if/else）

产生布尔结果（真或假）的表达式称为条件。有多种方法来评估条件，包括 `if`、`if-else`、`if-elif-else` 和嵌套条件。

****语法****：

```bash
if [[ condition ]];
then
	statement
elif [[ condition ]]; then
	statement 
else
	do this by default
fi
```

Bash 条件语句的语法

我们可以使用逻辑运算符（如 AND `-a` 和 OR `-o`）进行更具意义的比较。

```bash
if [ $a -gt 60 -a $b -lt 100 ]
```

此语句检查两个条件是否都为真：a 大于 60 且 b 小于 100。

让我们看一个使用 `if`、`if-else` 和 `if-elif-else` 语句的 Bash 脚本示例，以确定用户输入的数字是正数、负数还是零：

```bash
#!/bin/bash

echo "Please enter a number: "
read num
```

Script to determine if a number is positive, negative, or zero

该脚本首先提示用户输入一个数字。然后，它使用一个 `if` 语句检查该数字是否大于 0。如果是的话，脚本输出该数字是正数。如果该数字不大于 0，脚本进入下一个语句，即 `if-elif` 语句。在这里，脚本检查该数字是否小于 0。如果是的话，脚本输出该数字是负数。最后，如果该数字既不大于 0 也不小于 0，脚本使用 `else` 语句输出该数字是零。

来看一下它的运行情况 🚀

![test-odd](https://www.freecodecamp.org/news/content/images/2023/03/test-odd.gif)

## 在 Bash 中的循环和分支

### While 循环

While 循环检查一个条件，并且在条件为 `true` 时持续循环。我们需要提供一个计数器语句来增加计数器以控制循环的执行。

在下面的例子中，`(( i += 1 ))` 是增加 `i` 值的计数器语句。该循环将恰好运行 10 次。

```bash
#!/bin/bash
i=1
while [[ $i -le 10 ]] ; do
   echo "$i"
  (( i += 1 ))
done
```

While 循环执行 10 次。

![image-187](https://www.freecodecamp.org/news/content/images/2023/03/image-187.png)

### For 循环

`for` 循环，就像 `while` 循环一样，允许你执行特定次数的语句。每个循环在语法和用法上有所不同。

在下面的例子中，该循环将迭代 5 次。

```bash
#!/bin/bash

for i in {1..5}
do
    echo $i
done
```

For 循环迭代 5 次。

![image-186](https://www.freecodecamp.org/news/content/images/2023/03/image-186.png)

### Case 语句

在 Bash 中，case 语句用于将给定值与一系列模式进行比较，并根据第一个匹配的模式执行一段代码。Bash 中 case 语句的语法如下：

```bash
case expression in
    pattern1)
        # code to execute if expression matches pattern1
        ;;
    pattern2)
        # code to execute if expression matches pattern2
        ;;
    pattern3)
        # code to execute if expression matches pattern3
        ;;
    *)
        # code to execute if none of the above patterns match expression
        ;;
esac
```

Case 语句语法

这里，“expression”是我们想要比较的值，“pattern1”，“pattern2”，“pattern3”等是我们想要进行比较的模式。

双分号 “;;” 将要为每个模式执行的代码块分隔开来。星号 “\*” 代表默认情况，当没有一个指定的模式匹配该表达式时执行。

让我们看一个例子。

```bash
fruit="apple"

case $fruit in
    "apple")
        echo "This is a red fruit."
        ;;
    "banana")
        echo "This is a yellow fruit."
        ;;
    "orange")
        echo "This is an orange fruit."
        ;;
    *)
        echo "Unknown fruit."
        ;;
esac
```

Case 语句示例

在这个例子中，由于“fruit”的值是“apple”，第一个模式匹配，并且执行 echo “This is a red fruit.” 的代码块。如果“fruit”的值是“banana”，第二个模式将匹配并执行 echo “This is a yellow fruit.” 的代码块，依此类推。如果“fruit”的值不匹配任何指定的模式，则执行默认情况，输出“Unknown fruit.”。

## 如何使用 cron 安排脚本

Cron 是 Unix-like 操作系统中用于作业调度的强大工具。通过配置 cron，你可以设置自动作业在每日、每周、每月或特定时间运行。cron 提供的自动化能力在 Linux 系统管理中起到了至关重要的作用。

以下是安排 crons 的语法：

```bash
# Cron job example
* * * * * sh /path/to/script.sh
```

这里，`*` 代表分别的分钟、小时、日、月、周几。

以下是一些安排 cron 作业的示例。

| 安排 | 描述 | 示例 |
| --- | --- | --- |
| `0 0 * * *` | 每天午夜运行一个脚本 | `0 0 * * * /path/to/script.sh` |
| `*/5 * * * *` | 每 5 分钟运行一个脚本 | `*/5 * * * * /path/to/script.sh` |
| `0 6 * * 1-5` | 从星期一到星期五每天早上 6 点运行一个脚本 | `0 6 * * 1-5 /path/to/script.sh` |
| `0 0 1-7 * *` | 每个月的前 7 天运行一个脚本 | `0 0 1-7 * * /path/to/script.sh` |
| `0 12 1 * *` | 每个月的第一天中午 12 点运行一个脚本 | `0 12 1 * * /path/to/script.sh` |

#### 使用 crontab

`crontab` 工具用于添加和编辑 cron 作业。

`crontab -l` 列出特定用户已经安排好的脚本。

你可以通过 `crontab -e` 添加和编辑 cron。

你可以在我的 [另一篇文章][25] 中阅读更多关于 cron 作业的内容。

## 如何调试和排除 Bash 脚本的故障

调试和排除故障是任何 Bash 脚本编写者的重要技能。虽然 Bash 脚本可以非常强大，但它们也容易出现错误和意外行为。在本节中，我们将讨论一些调试和排除 Bash 脚本故障的技巧和技术。

调试 Bash 脚本最有用的技巧之一是在脚本的开头设置 `set -x` 选项。这个选项启用了调试模式，使得 Bash 会在终端中打印它执行的每个命令，并以 `+` 符号作为前缀。这对于识别脚本中出现错误的位置非常有帮助。

```bash
#!/bin/bash

set -x

# 您的脚本放在这里
```

### 检查退出码

当 Bash 遇到错误时，它会设置一个退出码来指示错误的性质。您可以使用 `$?` 变量检查最近命令的退出码。值为 `0` 表示成功，而任何其他值表示错误。

```bash
#!/bin/bash

# 您的脚本放在这里

if [ $? -ne 0 ]; then
    echo "发生错误。"
fi
```

### 使用 `echo` 语句

另一个调试 Bash 脚本的有用技巧是在代码中插入 `echo` 语句。这可以帮助您识别错误发生的位置以及变量传递的值是什么。

```bash
#!/bin/bash

# 您的脚本放在这里

echo "变量 x 的值是: $x"

# 更多代码放在这里
```

### 使用 `set -e` 选项

如果您希望在脚本中的任何命令失败时立即退出脚本，您可以使用 `set -e` 选项。这个选项会使 Bash 在脚本中的任何命令失败时退出并带有错误，这样可以更容易地识别和修复脚本中的错误。

```bash
#!/bin/bash

set -e

# 您的脚本放在这里
```

### 通过验证日志来排查定时任务

我们可以使用日志文件来排查定时任务。日志会记录所有的计划任务。您可以在日志中检查并验证特定任务是否按预期运行。

对于 Ubuntu/Debian，您可以在这里找到 `cron` 日志：

```bash
/var/log/syslog
```

其他发行版的位置各不相同。

一个 cron 任务日志文件可能看起来像这样：

```bash
2022-03-11 00:00:01 Task started
2022-03-11 00:00:02 Running script /path/to/script.sh
2022-03-11 00:00:03 Script completed successfully
2022-03-11 00:05:01 Task started
2022-03-11 00:05:02 Running script /path/to/script.sh
2022-03-11 00:05:03 Error: unable to connect to database
2022-03-11 00:05:03 Script exited with error code 1
2022-03-11 00:10:01 Task started
2022-03-11 00:10:02 Running script /path/to/script.sh
2022-03-11 00:10:03 Script completed successfully
```

Cron 日志

## 结论

在本文中，我们首先介绍了如何访问终端，然后运行了一些基本的 bash 命令。我们还学习了什么是 bash shell。我们简要地了解了使用循环和条件语句分支代码。最后，我们讨论了使用 cron 来自动化脚本，并介绍了一些故障排除技巧。

### 学习更多关于 Bash 脚本的资源

如果您想深入了解 bash 脚本的世界，我建议您看看 freeCodeCamp 上这门 6 小时的 Linux 课程。

<iframe width="356" height="200" src="https://www.youtube.com/embed/sWbUDq4S6Y8?feature=oembed" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen="" title="Introduction to Linux – Full Course for Beginners" name="fitvid0"></iframe>

在本教程中，您学到了最喜欢的内容是什么？您还可以在这些[平台][27]上与我联系。📧�

下次教程再见，祝您编码愉快 😁

横幅图片致谢：[Freepik][28]

---

![Zaira Hira](https://www.freecodecamp.org/news/content/images/size/w60/2024/07/Untitled-design--8-.png)

我是一名 DevOps 顾问和 FreeCodeCamp 的作者。我的目标是为技术人员提供简洁明了的内容！

---

如果您看完了这篇文章，请向作者表示感谢，展示您的关心。说声谢谢

免费学习编码。freeCodeCamp 的开源课程已经帮助了超过 40,000 人找到开发者工作。[开始学习][29]

[1]: #pre-requisites
[2]: #introduction
[3]: #definition-of-bash-scripting
[4]: #advantages-of-bash-scripting
[5]: #overview-of-bash-shell-and-command-line-interface
[6]: #how-to-get-started-with-bash-scripting
[7]: #how-to-run-bash-commands-from-the-command-line
[8]: #how-to-create-and-execute-bash-scripts
[9]: #bash-scripting-basics
[10]: #comments-in-bash-scripting
[11]: #variables-and-data-types-in-bash
[12]: #input-and-output-in-bash-scripts
[13]: #basic-bash-commands-echo-read-etc-
[14]: #conditional-statements-if-else-
[15]: #looping-and-branching-in-bash
[16]: #while-loop
[17]: #for-loop
[18]: #case-statements
[19]: #how-to-schedule-scripts-using-cron
[20]: #how-to-debug-and-troubleshoot-bash-scripts
[21]: #conclusion
[22]: #resources-for-learning-more-about-bash-scripting
[23]: https://replit.com/~
[24]: https://www.freecodecamp.org/news/how-to-install-wsl2-windows-subsystem-for-linux-2-on-windows-10/
[25]: https://www.freecodecamp.org/news/cron-jobs-in-linux/
[26]: https://www.freecodecamp.org/news/p/01e109a1-569f-45d1-b5db-c35259b5da7f/zaira_.bio.link
[27]: https://zaira_.bio.link/
[28]: https://www.freepik.com/free-vector/hand-drawn-flat-design-devops-illustration_25726540.htm#query=programmer%20linux&position=4&from_view=search&track=ais
[29]: https://www.freecodecamp.org/learn/

