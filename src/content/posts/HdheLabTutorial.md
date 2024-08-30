---
title: HdHeLabTutorial
published: 2024-08-30
description: 'A tutorial for hdHe''s Lab'
image: ''
tags: []
category: '教程'
draft: false 
language: ''
---


`Author` : Maplef

`Email` : <maplefsnow@gmail.com>

`Date` : 2024.03

## 目录

<!-- TOC -->

- [hdHeLab Tutorial](#hdhelab-tutorial)
    - [目录](#%E7%9B%AE%E5%BD%95)
    - [前言](#%E5%89%8D%E8%A8%80)
    - [建议提前掌握的知识/技能](#%E5%BB%BA%E8%AE%AE%E6%8F%90%E5%89%8D%E6%8E%8C%E6%8F%A1%E7%9A%84%E7%9F%A5%E8%AF%86%E6%8A%80%E8%83%BD)
        - [简洁且高效地使用现代操作系统（Windows, Linux, ...）](#%E7%AE%80%E6%B4%81%E4%B8%94%E9%AB%98%E6%95%88%E5%9C%B0%E4%BD%BF%E7%94%A8%E7%8E%B0%E4%BB%A3%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9Fwindows-linux-)
            - [Linux](#linux)
            - [Windows](#windows)
        - [规范地管理项目和文件夹结构](#%E8%A7%84%E8%8C%83%E5%9C%B0%E7%AE%A1%E7%90%86%E9%A1%B9%E7%9B%AE%E5%92%8C%E6%96%87%E4%BB%B6%E5%A4%B9%E7%BB%93%E6%9E%84)
        - [会使用终端 Terminal 并理解环境变量 Environment Variables](#%E4%BC%9A%E4%BD%BF%E7%94%A8%E7%BB%88%E7%AB%AF-terminal-%E5%B9%B6%E7%90%86%E8%A7%A3%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F-environment-variables)
            - [Path](#path)
            - [其他变量](#%E5%85%B6%E4%BB%96%E5%8F%98%E9%87%8F)
        - [了解并掌握面向对象程序设计思想](#%E4%BA%86%E8%A7%A3%E5%B9%B6%E6%8E%8C%E6%8F%A1%E9%9D%A2%E5%90%91%E5%AF%B9%E8%B1%A1%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E6%80%9D%E6%83%B3)
        - [了解代码编辑器（Editor）和集成开发环境（IDE）及掌握其使用方法](#%E4%BA%86%E8%A7%A3%E4%BB%A3%E7%A0%81%E7%BC%96%E8%BE%91%E5%99%A8editor%E5%92%8C%E9%9B%86%E6%88%90%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83ide%E5%8F%8A%E6%8E%8C%E6%8F%A1%E5%85%B6%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95)
        - [简单了解程序编译过程和编译器](#%E7%AE%80%E5%8D%95%E4%BA%86%E8%A7%A3%E7%A8%8B%E5%BA%8F%E7%BC%96%E8%AF%91%E8%BF%87%E7%A8%8B%E5%92%8C%E7%BC%96%E8%AF%91%E5%99%A8)
            - [编译四阶段](#%E7%BC%96%E8%AF%91%E5%9B%9B%E9%98%B6%E6%AE%B5)
            - [编译器](#%E7%BC%96%E8%AF%91%E5%99%A8)
        - [使用 VPN 节点和代理软件访问国际网络](#%E4%BD%BF%E7%94%A8-vpn-%E8%8A%82%E7%82%B9%E5%92%8C%E4%BB%A3%E7%90%86%E8%BD%AF%E4%BB%B6%E8%AE%BF%E9%97%AE%E5%9B%BD%E9%99%85%E7%BD%91%E7%BB%9C)
            - [获取代理软件](#%E8%8E%B7%E5%8F%96%E4%BB%A3%E7%90%86%E8%BD%AF%E4%BB%B6)
            - [获取 VPN 节点](#%E8%8E%B7%E5%8F%96-vpn-%E8%8A%82%E7%82%B9)
        - [Git](#git)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [配置](#%E9%85%8D%E7%BD%AE)
            - [学习](#%E5%AD%A6%E4%B9%A0)
        - [流程图绘制](#%E6%B5%81%E7%A8%8B%E5%9B%BE%E7%BB%98%E5%88%B6)
            - [draw.io](#drawio)
            - [Microsoft Visio](#microsoft-visio)
        - [CMake](#cmake)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [学习](#%E5%AD%A6%E4%B9%A0)
    - [实验室常用软件和开发套件](#%E5%AE%9E%E9%AA%8C%E5%AE%A4%E5%B8%B8%E7%94%A8%E8%BD%AF%E4%BB%B6%E5%92%8C%E5%BC%80%E5%8F%91%E5%A5%97%E4%BB%B6)
        - [OpenCV - 机器视觉](#opencv---%E6%9C%BA%E5%99%A8%E8%A7%86%E8%A7%89)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [学习](#%E5%AD%A6%E4%B9%A0)
        - [Qt / LabView - GUI 操作界面设计](#qt--labview---gui-%E6%93%8D%E4%BD%9C%E7%95%8C%E9%9D%A2%E8%AE%BE%E8%AE%A1)
        - [NINational Instruments DAQmx - NI 数据采集卡](#ninational-instruments-daqmx---ni-%E6%95%B0%E6%8D%AE%E9%87%87%E9%9B%86%E5%8D%A1)
        - [Advantech Common Motion API - 研华运动控制卡](#advantech-common-motion-api---%E7%A0%94%E5%8D%8E%E8%BF%90%E5%8A%A8%E6%8E%A7%E5%88%B6%E5%8D%A1)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [学习](#%E5%AD%A6%E4%B9%A0)
        - [DaHeng Galaxy SDK - 大恒相机开发套件](#daheng-galaxy-sdk---%E5%A4%A7%E6%81%92%E7%9B%B8%E6%9C%BA%E5%BC%80%E5%8F%91%E5%A5%97%E4%BB%B6)
        - [HIKVision SDK - 海康威视相机开发套件](#hikvision-sdk---%E6%B5%B7%E5%BA%B7%E5%A8%81%E8%A7%86%E7%9B%B8%E6%9C%BA%E5%BC%80%E5%8F%91%E5%A5%97%E4%BB%B6)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [学习](#%E5%AD%A6%E4%B9%A0)
    - [开发环境配置](#%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE)
        - [Visial Studio Code](#visial-studio-code)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [配置](#%E9%85%8D%E7%BD%AE)
        - [Visual Studio](#visual-studio)
            - [安装](#%E5%AE%89%E8%A3%85)
            - [配置](#%E9%85%8D%E7%BD%AE)
    - [写在后面](#%E5%86%99%E5%9C%A8%E5%90%8E%E9%9D%A2)

<!-- /TOC -->

## 前言

我时常怀疑，写下这些东西的意义，究竟会有多少。我时常怀疑，非计科科班出身而要掌握这些技能，是否会有失偏颇。

我曾目睹一些惨象，比如用记事本在没有后缀名的文档里敲代码，比如需要恢复之前删掉的某个模块而不断 ctrl-Z，比如混乱的项目库管理让整个项目几乎无法维护……

许多看似常识一样的知识和技能，如果不去了解和学习或者甚至未曾听闻，便也会如“隔了一层可悲的厚障壁”，怎么也施展不开。除去研究方面的种种困难，我更不愿意看到的是由于低效和混乱的工作方式导致时间和精力被白白浪费。但这是一个水滴石穿的过程，只有具备一定的项目开发经验才会慢慢在实践中总结一套属于自己的工作流，慌不择路往往是一个开发者的必经之路。

我常常回想：“若是当时写某某的时候如何如何，便好了”，“若是当时知道有某某，就好了”。诸如此类的想法变成了一点又一点微小的遗憾，一点又一点微小的遗憾聚沙成塔，最终变得无法撼动。我不想看到后来者继续积累这种微小的遗憾。

我并非计科科班出身，只依靠一厢情愿在这条路上摸爬滚打，并不见得有什么资格在这里指指点点，姑妄言之，姑妄听之。若是读后可以产生一些有益的思考或启发，便也不枉实验室经年来对我的种种栽培。

我在深夜里回顾过往，敲下这些文字。那些曾经做过的努力和探索，或心有不甘，或潦草收尾，都构筑成坚实而悲伤的基，不堪回首，回首不堪。而如今我即将离开这里，时间要把一切都雪藏。这些文字或许只是我自己的一厢情愿，连我自己都不知道它们究竟何去何从。但倘若尚有一个人读过，倘若只有一个人读过也好，也算作是我曾经存在于斯的今生今世的证明。

> 不要温和地走进，那个良夜。

*<p style="text-align: center;">献给勇敢的人</p>*

## 建议提前掌握的知识/技能

笔者整理了进入实验室以及参与各种竞赛以来，自身或其他同学因基本能力的欠缺而导致的低效工作情况，大致列举了在正式开始启动一个项目前需要掌握的基本技能，以供参考。

### 简洁且高效地使用现代操作系统（Windows, Linux, ...）

#### Linux

如果读者是 Linux 发行版（如 Arch Linux、Ubuntu 等）的惯用者，笔者认为读者已经不必继续阅读本章节的剩余部分，可直接阅读 [实验室常用软件和开发套件](#%E5%AE%9E%E9%AA%8C%E5%AE%A4%E5%B8%B8%E7%94%A8%E8%BD%AF%E4%BB%B6%E5%92%8C%E5%BC%80%E5%8F%91%E5%A5%97%E4%BB%B6) 一章。

#### Windows

有许多个人电脑常用的系统管理方法可能并不适用于工控机/开发环境，由于 Windows 系统十分宏大和繁杂，每个人都有不同的理解，笔者在此给出一些建议，仅供参考。

- 开发环境应竭力遵循系统的整洁和最小化原则，不要安装不必要的大型应用软件，**特别是 360、电脑管家等所谓的安全软件**
- 确保开发套件、SDK、驱动、编译器等重要系统组件从**官方网站**下载，不要使用第三方下载站或分发页。若官网无法访问，参考 [使用 VPN 节点和代理软件访问国际网络](#%E4%BD%BF%E7%94%A8-vpn-%E8%8A%82%E7%82%B9%E5%92%8C%E4%BB%A3%E7%90%86%E8%BD%AF%E4%BB%B6%E8%AE%BF%E9%97%AE%E5%9B%BD%E9%99%85%E7%BD%91%E7%BB%9C) 一章
- 开发环境可能被多人使用，不要留下自己的个人信息（如浏览器记住密码等功能），信息安全很重要
- 尽量不要使用中文路径名，一律使用英文命名文件夹和源文件。路径名中严禁出现半角单引号(`'`)、半角双引号(`"`)或其他可能引起歧义的特殊字符。路径名中尽量不要带有空格，如确有需要可使用半角减号(`-`)或下划线(`_`)代替
- 合理管理硬盘空间，可对系统硬盘进行必要的分区加以区分。如可参考分为系统(system)、环境(env)、软件(software)、项目(projects)、文档(doc)五区
- 尽管系统回收站是最后的后悔药，删除每一个文件之前也都要三思

### 规范地管理项目和文件夹结构

规范、有序地管理项目结构有助于代码层次的理解和项目的扩展，可多阅读、参考别人的项目，学习文件夹命名方式、文件夹的组织等，最终形成个人的习惯。

下面是我个人使用的一个项目结构，可供参考：

```shell
.
├── CMakeLists.txt      -> cmake 文档
├── .git                -> git 本地存储库
├── .gitignore          -> git 忽略文件
├── include             -> 模块头文件
├── lib                 -> 模块静态链接库
├── module              -> 各模块面向对象封装
├── src                 -> 源代码
├── tasks               -> 多线程任务
├── tests               -> 测试脚本
├── utils               -> 工具类
└── .vscode             -> vscode 配置文件
```

### 会使用终端 (Terminal) 并理解环境变量 (Environment Variables)

Windows 自带的终端命令行主要是 `cmd.exe` 或 `powershell.exe`，可以直接通过 `Win + R` 快捷键调出运行后启动。但这两个终端过于老旧，笔者推荐 Windows 推出的全新终端 `Windows Terminal` 接管上述两个程序的功能。打开 Microsoft Store 搜索 “Windows Terminal” 即可下载并安装，安装完成后 `Win + R` 并键入 `wt` 即可快捷启动。

关于 Windows 命令行指令，可以自行搜索官方文档学习，常用的有 `cd`, `dir`, `cat`, `rm` 等。

一个默认的终端会读取系统中的环境变量，让运行特定程序变得简单。环境变量分为系统变量和用户变量，系统变量对所有用户生效，用户变量则只对当前登录的用户生效，下文不再区分。在 Windows 平台下，环境变量主要分为 `Path` 和其他变量。

#### Path

Path 环境变量的主要作用是能够让系统快速启动一个应用程序，其变量值是很多个文件夹路径。它的意思是告诉系统：当你想运行一个应用程序时，你可以在这些文件夹里查找。这样就能让系统快速启动这个应用程序。

一些经典应用：`git`, `python3`, `code`, `java`, `g++` 等。

#### 其他变量

其他变量是为了方便记录某些特定路径或系统信息，或打开某些特定文件，可以自行配置。

### 了解并掌握面向对象程序设计思想

笔者认为，对于开发者而言，学习并具有面向对象的程序设计思维非常重要。**面向对象是一种思维，并不局限于某种特定的语言**。学习面向对象的思想可以让代码编写能力更上一个台阶，并且对整个代码世界和现实世界都有更进一步的认识。

学习面向对象程序设计，学习封装、继承、多态等特性，可以提高代码的复用性，让整个工程井井有条，省去重复开发相似功能的时间。

推荐阅读菜鸟教程中关于 C++ 面向对象部分的介绍：[https://www.runoob.com/cplusplus/cpp-classes-objects.html](https://www.runoob.com/cplusplus/cpp-classes-objects.html)。其他文档或视频教程均可，可以自行搜索。

### 了解代码编辑器（Editor）和集成开发环境（IDE）及掌握其使用方法

### 简单了解程序编译过程和编译器

#### 编译四阶段

从代码源文件到最终能够执行的可执行文件，编译过程会经过以下的四个阶段：

- 预处理
- 编译
- 汇编
- 链接

具体细节可自行搜索学习，特别需要着重理解的是“**链接**”阶段，此阶段也是环境配置和程序报错的重灾区。

#### 编译器

常见的 C++ 编译器有以下几种：

- GCC (GNU Compiler Collection)：跨平台编译器
- MinGW (Minimalist GNU for Windows)：在Windows上开发和编译使用GNU工具链的应用程序，提供了一种轻量级的方式在 Windows 环境下进行开发
- MSVC (Microsoft Visual C++)：微软开发的一款 C++ 编译器和集成开发环境，是 Windows 平台上最常用的 C++ 开发工具之一

承担具体编译任务的主要是编译器中的 `gcc.exe`(C) 和 `g++.exe`(C++) 程序，集成开发环境或 cmake 脚本等底层调用的都是这些程序以完成编译操作。

有关 MinGW 的安装，可参考：[https://code.visualstudio.com/docs/cpp/config-mingw](https://code.visualstudio.com/docs/cpp/config-mingw)

### 使用 VPN 节点和代理软件访问国际网络

使用 VPN 节点，俗称“翻墙”，可以自由地访问国际网络和服务，如 [Google](https://google.com)、[Arxiv](https://arxiv.org/) 等。

#### 获取代理软件

笔者常用的代理软件为 Clash，但 Clash 官方内核仓库因不可抗力被迫删除，目前可在此镜像站下载 Clash For Windows 版本：[https://www.clash.la/releases/](https://www.clash.la/releases/)。

其他代理软件，如 [ShadowRocket](https://www.shadowrocket.vip/)、 [v2ray](https://www.v2ray.com/) 等亦可，可根据喜好自行探索。

#### 获取 VPN 节点

有许多个人或国际组织对中国大陆用户提供 VPN 节点服务，笔者常用的代理服务由 XSUS 提供，可在此进行购买：[https://xsus.wiki/](https://xsus.wiki/)。其他运营商亦可，自行探索。

简而言之，购买节点后会获得一串订阅链接，将此订阅链接粘贴至代理软件相应的配置项中即可拉取节点信息，选择节点并开启系统代理后即可自由访问国际网络。相关教程很多，可以自行搜索。

### Git

Git 官网：[https://git-scm.com/](https://git-scm.com/)

学会使用 Git 管理自己的项目，是笔者认为每个编写代码的人应该具备的基本素质。Git 提供了完善的版本管理机制，允许开发者以“提交(commit)”为单位对项目代码进行回溯，更有全球性的代码仓库 [GitHub](https://github.com/) 可作为远程(remote)服务器使用，大大降低了因本地硬件故障造成的项目丢失可能性。

#### 安装

在 Windows 下，官网下载 Git 的安装程序并按照提示安装即可。Git 的安装程序可配置项较多，全部使用默认设置一路 next 即可。

将 Git 的安装目录加入系统变量(PATH)中。

#### 配置

打开终端，对 Git 进行基本的配置。执行以下命令：

```bash
# 设置 git 全局代理，代理端口根据代理软件给出的端口设置，一般为 7890
git config --global https.proxy https://127.0.0.1:7890
git config --global http.proxy http://127.0.0.1:7890

# 设置 git 提交时使用的用户名和邮箱，否则无法进行提交
# 如果开发环境是公共的且所有人共用一个账户，不要填写自己的个人信息，填一个公用的即可（乱填也行）
git config user.name <your_name>
git config user.email <your_email>
```

#### 学习

推荐一个可视化学习 Git 的网站：[https://learngitbranching.js.org/?locale=zh_CN](https://learngitbranching.js.org/?locale=zh_CN)，这个网站基本囊括了 Git 使用的所有入门/初级知识，值得一学。

### 流程图绘制

#### draw.io

一个开源的绘图工具，网站：<https://draw.io/>

可以在线绘制，也有应用程序，是画流程图、甘特图等各类图表的好帮手，模板丰富。

#### Microsoft Visio

和微软 Office 家族御三家的操作逻辑相同，可以自行学习。

### CMake

> CMake是一个跨平台的安装（编译）工具，可以用简单的语句来描述所有平台的安装(编译过程)。他能够输出各种各样的makefile或者project文件，能测试编译器所支持的C++特性,类似UNIX下的automake。只是 CMake 的组态档取名为 CMakeLists.txt。Cmake 并不直接建构出最终的软件，而是产生标准的建构档（如 Unix 的 Makefile 或 Windows Visual C++ 的 projects/workspaces），然后再依一般的建构方式使用。
>
> ——百度百科

简而言之，CMake 可以看作是 Make 的上层封装，使开发者直接生成 Makefile，省去复杂的编写。用 CMake 进行项目的建构可以类比使用 VS 建构，但 CMake 更灵活轻量更易配置，且是跨平台的。

后文的 [开发环境配置](#%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE) 一章，笔者介绍的就是 VS Code + CMake 的环境配置方法。

#### 安装

CMake 官方下载：[https://cmake.org/download/](https://cmake.org/download/)

#### 学习

CMake 官方编写的 Tutorial 就是最好的 CMake 教程：[https://cmake.org/cmake/help/latest/guide/tutorial/index.html](https://cmake.org/cmake/help/latest/guide/tutorial/index.html)，值得一学。

## 实验室常用软件和开发套件

笔者整理了进入实验室以来所接触到的各种硬件软件的开发套件，并给予简要介绍和说明。

有关如何使用 VS(Visual Studio) 或 VS Code(Visual Studio Code) 进行相关软件环境和项目的配置，参见后文。

### OpenCV - 机器视觉

#### 安装

OpenCV 官方下载页：[https://opencv.org/releases/](https://opencv.org/releases/)

运行下载好的 exe 程序，选择解压路径即可完成安装。

有关如何将 OpenCV 集成至自己的项目中，参见 [开发环境配置](#%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83%E9%85%8D%E7%BD%AE) 一章。

#### 学习

关于 OpenCV 的学习，市面上有很多教程，可以自行搜索。

一些有用的资料：

- OpenCV 官方文档：[https://docs.opencv.org/4.9.0/index.html](https://docs.opencv.org/4.9.0/index.html)
- OpenCV Tutorial C++：[https://www.opencv-srf.com/p/introduction.html](https://www.opencv-srf.com/p/introduction.html)
- Learn OpenCV C++ and Python Examples：[https://github.com/spmallick/learnopencv](https://github.com/spmallick/learnopencv)

### Qt / LabView - GUI 操作界面设计

*由于笔者仅进行过 Qt 的开发，故本节内容只介绍 Qt。*

Qt Online Installer 下载：[https://www.qt.io/download-qt-installer-oss](https://www.qt.io/download-qt-installer-oss)

由于在线安装默认连接的官方下载源速度过于缓慢，需要手动指定国内中科大镜像源，所以不要通过双击此 exe 的方式进行下载。在下载目录打开终端，键入以下命令启动下载器：

```bash
# 由于版本可能不同，下载器文件名按照实际名字更改
.\qt-unified-windows-x64-4.7.0-online.exe --mirror https://mirrors.ustc.edu.cn/qtproject
```

按照下载器给出的提示进行安装，在指定安装路径界面选择 `Qt x.x for desktop development` 安装方式，之后全部以默认项安装即可。

Qt 自带了 minGW1120_64 编译器和 cmake，（也许）针对 Qt 进行了特别的优化，推荐在配置 Qt 环境时直接指定 Qt 自带的编译器和 cmake，无需额外安装。

- Qt 自带的 mingw 编译器位置：`../Qt/Tools/mingw1120_64/`
- Qt 自带的 cmake 位置：`../Qt/Tools/CMake_64/bin/`

### NI(National Instruments) DAQmx - NI 数据采集卡

### Advantech Common Motion API - 研华运动控制卡

#### 安装

Advantech Common Motion Driver 下载：[https://www.advantech.com.cn/zh-cn/support/details/driver?id=1-RNJ0CF](https://www.advantech.com.cn/zh-cn/support/details/driver?id=1-RNJ0CF)

下载后安装软件，软件安装完成后会自动安装驱动，保持默认设置即可。

研华官方提供的示例软件 Common Motion Utility 的路径为 `../Advantech/Common Motion/Utility/Common Motion Utility.exe`，可在此进行基本的板卡功能测试。

#### 学习

Common motion API manual：[https://www.advantech.com/en-us/support/details/software-api-manual?id=1-11TOQZZ](https://www.advantech.com/en-us/support/details/software-api-manual?id=1-11TOQZZ)

自行下载阅读并学习该开发手册。

### DaHeng Galaxy SDK - 大恒相机开发套件

### HIKVision SDK - 海康威视相机开发套件

#### 安装

官方相机客户端 MVS 下载：[https://www.hikrobotics.com/cn/machinevision/service/download?module=0](https://www.hikrobotics.com/cn/machinevision/service/download?module=0)

#### 学习

安装 MVS 后，在 `../MVS/Development/Documentations/` 目录下可找到文档和开发指南，可对照阅读学习。

## 开发环境配置

配置开发环境向来是让人头痛的事情，笔者深有体会。不同的系统版本、软件版本、集成开发环境版本下都会产生难以预期的奇怪报错，且通常由于问题的特殊性难以找到相应的教程，笔者对此心有戚戚。笔者在此撰写的教程总有一天会过时或失效，笔者希望读者在配置环境的过程中逐渐掌握一般方法和常见问题的解决方式，学会看报错信息和 log，在试错中不断学习和进步，以期能够自由地组装趁手的开发环境。

由于 Visual Studio 内置了 Windows Kit 和 MSVC 编译器等 Windows 平台下开发必需的组件，即使只使用 vscode 进行开发，也需要安装 Visual Studio 及其组件。

### Visial Studio Code

#### 安装

VS Code 官方下载：<https://code.visualstudio.com>

#### 配置



### Visual Studio

#### 安装

Visual Studio 官方下载：<https://visualstudio.microsoft.com>

遵循安装程序的指引进行安装，组件勾选 `使用 C++ 的桌面开发` 和 `通用 Windows 平台开发` 即可，右侧详细组件列表可继续自行选择需要组件进行添加。若 `Windows 10 Kit` 没有勾选，可选上。

更改安装位置到自己喜欢的位置，取消勾选 `安装后保留缓存`。一个可参考的配置如下：

(image not found)

#### 配置

## 写在后面

这里是写在后面。