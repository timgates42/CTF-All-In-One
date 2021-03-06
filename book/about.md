# 关于本书

## 作者简介

杨超，毕业于西安电子科技大学，L-Team成员。目前就职于中国汽研北京分院，从事车联网安全研究和工具开发。曾在海康威视、斗象科技工作过。活跃在开源社区，关注我的GitHub（firmianay）。

## 作者序

时间回到2017年7月，随着信息安全的发展，CTF竞赛也开始引人关注，这种有趣的竞赛模式对技术切磋和快速学习十分有效。在西电信安协会（XDSEC）学长的带领下，我已经接触了较长的一段时间。由于网上还没有比较完善和系统的资料，本着开源之精神，以分享他人提高自己为目的，我在GitHub上创建了一个叫做“CTF-All-In-One”的项目，并给了自己第1个star。在随后的时间里，这个项目日渐完善，吸引和帮助了不少初学者，到今天已经收获了超过2100个star，在此我将它们献给所有为技术分享与进步作出贡献的CTF出题人和项目贡献者们。

收到刘皎老师的约稿邀请是在2018年10月，那时我刚上大四，我说可以试试看，就惊喜又惶恐地接受了这项挑战。然后就是定目录，交样章，在2019年1月签订了约稿合同。没想到写作的道路竟如此艰难，每一章、每一节、每一个例子甚至每一个词都要斟酌，就生怕误人子弟。学业和工作的事情很多，最初参与的两个朋友相继离开，我本人也多次想要放弃，直到2020年7月才完成初稿。经过几轮艰苦的校稿，终于在2020年10月签订了出版合同。两年时间仿佛一晃就这样过去了。

写作的过程基本就是一个现学现卖的过程，我一边学习新知识，一边在框架体系里进行整理。这条路上有太多的分叉和无数的坑，我尽量把自己的经验写进书里，让读者可以快速获得其中的关键技术，避免重复劳动。所以与其称之为一本书，倒不如说是一个经过校对、完善，最终得到出版的知识库。在这个过程中，我也发现了写作对我来说是一种有效的训练方式，是一种附加的价值，通过对自己的知识和想法进行梳理，从而大大有益于我的工作。

我知道自己的限度，这本书是我写的第一本也很可能是最后一本。安全很有趣，我很高兴当初选择了它，很荣幸有机会分享出来，希望读者读到这本书时，也会为自己的选择而感到高兴。我们将此书命名为《CTF竞赛权威指南(Pwn篇)》，是给未来留出了空间，期待有更多人参与进来，拿出Web篇、Reverse篇、Crypto篇等更好的作品，让这个系列更配得上“权威”二字。

作为一本面向初学者的书，读者中一定不乏中学生群体，全国中学生网络安全竞赛每年都在我的母校西安电子科技大学进行，今年已是第三届，颇具规模。欢迎各位报考网络与信息安全学院，这里真的是一个很棒的地方。

最后，感谢我的大学室友刘晋，他早期的帮助让这个项目得以成型。感谢腾讯的吴石老师，他的推荐让这个成型的项目得以转换成书。感谢电子工业出版社的刘皎老师，她认真细致的工作使本书得以高质量地呈现给读者。感谢eee战队谢天忆、朱梦凡、马会心和刘耕铭的审核。感谢我的学弟槐和koocola，贡献了本书第11章的初稿。感谢湖北警官学院的谈楚瑜和MXYLR，以及其他来自GitHub的朋友的鼓励和支持。感谢我的父母给了我选择和发展的自由，让我在人生道路上没有后顾之忧。以及感谢那位不愿透露姓名的朋友，遇见你曾是青春最美好的事。感谢你们！

杨超
2020年11月于北京

## 内容简介

本书专注于Linux二进制安全。全书包含12章，从二进制底层开始，结合源码详细分析了常见的二进制安全漏洞、缓解机制以及漏洞利用方法，并辅以分析工具和环境搭建的讲解。
本书在素材的选择上较为连续、完整，每个知识点均配以经典例题，并花费了大量篇幅深入讲解，以最大程度地还原分析思路和解题过程。读者完全可以依据本书自主、系统性地学习，达到举一反三的效果。
本书主要面向CTF初学者，也适合对CTF感兴趣的人群学习。

## 本书结构

**第1章 CTF简介**：介绍CTF竞赛模式、安全领域会议和学习经验。

**第2章 二进制文件**：介绍ELF文件格式、动静态编译和程序加载过程。

**第3章 汇编基础**：介绍必要的x86/x64汇编基础知识。

**第4章 Linux安全机制**：介绍必要的Linux基础知识，以及Pwn题中最常见的安全机制（Stack Canaries、No-eXecute、ASLR、PIE、FORTIFY_SOURCE、RELRO）。

**第5章 分析环境搭建**：介绍虚拟机、Docker环境的搭建和Pwn题的部署。

**第6章 分析工具**：介绍IDA Pro、Radare2、GDB以及其他常用工具的使用方法。

**第7章 漏洞利用开发**：介绍shellcode的基本原理，以及如何用Pwntools和zio库编写漏洞利用脚本。

**第8章 整数安全**：介绍计算机中整数的存储方式，以及溢出、回绕、截断等安全问题。

**第9章 格式化字符串**：介绍格式化字符串漏洞的原理和利用方法。

**第10章 栈溢出与ROP**：介绍栈溢出漏洞、返回导向编程的基本原理，以及BROP、SROP、ret2dl-resolve等多种利用方法。

**第11章 堆利用**：介绍glibc对内存堆块的管理方式，以及unlink、off-by-one、堆块重叠等多种利用方法。

**第12章 pwn技巧**：介绍Pwn题中常见的利用技巧和值得关注的安全问题。
