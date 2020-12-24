# Think Python

>第二版，基于 Python3


>原作者 Allen B. Downey


>翻译 [CycleUser](http://blog.cycleuser.org)


+   [在线阅读](https://think-py.apachecn.org)
+   [在线阅读（Gitee）](https://apachecn.gitee.io/think-py-2e-zh/)

## 译者的话
这是一本很经典的 Python 入门教材，也是一本很适合初学者的编程入门书籍。网上有过一些翻译，不过我觉得都还是自己动手来尝试一下，这样更有利于深入了解和体验，所以就再造轮子了。

## 作者的话
这是 Think Python 这本书的第二版，本次使用的是 Python3，与 Python2 有很多不同，这些不同之处会有标注。如果你用 Python2 的话，还是建议你去阅读[上一个版本](http://www.greenteapress.com/thinkpython/index.html)。

读者可以到[亚马逊](http://amzn.to/Owtmjy)购买本书；或者下载 Think Python 2e [PDF 格式的电子版.](http://www.greenteapress.com/thinkpython2/thinkpython2.pdf)；也可以在线阅读 Think Python 2e [HTML 网页版本](http://www.greenteapress.com/thinkpython2/html/index.html)（推荐这个，都是文字格式，更方便）.


样例代码以及其他问题的解决可以到[这里](http://www.greenteapress.com/thinkpython2/code)找(具体样例的链接在书中就有)。

## 简要介绍
Think Python 这本书是面向初学者介绍 Python 编程。

首先介绍的是一些编程的基本内容，给出概念和解释，然后循序渐进地深入讲解每个概念。

复杂的部分，比如递归以及面向对象编程，这些都分成一个个小块，以多个章节的方式来逐步介绍。

## 第二版的更新

*	开始用 Python3：书里面所有样例都用 Python3 来实现，参考代码也都做了升级，用 Python2 或者 3 都能运行。

*	去掉了一些比较难的内容：基于读者反馈，我们认识到大家存在某些困难，所以就调整或者去掉了一些难点。

*	浏览器内能 Python 编程了：初学者遇到的第一个困难就是安装 Python。另外有的读者可能不想去直接就安装 Python，我们就提供了一个用浏览器来运行 Python 的简介：使用 PythonAnywhere，一个免费的在线 Python 编程环境。（译者注：中国用户以考虑试试 fenby.com，也有类似的实现，还有视频的介绍。）

*	引入了更多的 Python 特性：单独加了一章来介绍一些第一版中没有提及的 Python 功能，比如列表解析和附加的数据结构。


这本书是一本自由的书，遵循[创作共用署名-非商业性使用-第三版协议](http://creativecommons.org/licenses/by-nc/3.0/)，这意味着你可以自由地复制、分发和修改他，只要你有所贡献，并且不用于商业目的，就可以。

如果你有一些评论、修正或者建议，可以发邮件给 feedback@thinkpython.com。

其他由 Allen Downey 编写的自-和谐-由书籍都可以在[Green Tea Press](http://greenteapress.com/)找到.

## 英文原版下载

*	编译好的 PDF 版本在这里下载：[PDF](http://www.greenteapress.com/thinkpython2/thinkpython2.pdf)。

*	LaTeX 代码在 GitHub 这里可以下载：[this GitHub repository](https://github.com/AllenDowney/ThinkPython2).


## 过往历史

第一版在[这里](http://www.greenteapress.com/thinkpython)，是由剑桥大学出版社出版的，标题是 Python for Software Design. 可以到亚马逊去买到。
本书的原始版本由 Green Tea Press 出版，标题为 How to Think Like a Computer Scientist: Learning with Python. 这个版本可以从[Lulu.com](http://lulu.com)这个网站找到。其他由 Allen Downey 编写的自由书籍都可以在 Green Tea Press 找到.

# 前言

## 本书的奇幻历史


在 1999 年 1 月的时候呢，我正准备教一门 Java 的入门编程课。我当时已经教过三次了，受挫感很强。班上挂科率特别高，而且即使那些没挂科的学生编程的整体水平也特别低。

当时有很多问题，首先我就发现教材不太好用。那些教材都特别大部头，有很多关于 Java 的细节，特别琐碎又并不重要，而且也没有足够的关于如何编程的高层次指导（译者注：就是缺乏战略性指导，没有告诉学生编程的心法）。这些教材总有一些『陷阱门效应』：开头他们都却是挺简单，然后逐步提升，接着突然在某个地方，比如第五章，出现很坑很复杂的陷阱。学生们要突然一下子应对太多新东西，甚至措手不及，而我作为教师就得花费整个后半个学期来一点点给学生们补上。

开课的两周之前，我最终决定要写个自己的教科书。目标如下：

*	简短。让学生读 10 页就够比让他们读 50 页效果好得多。

*	降低词汇难度。我尽量把术语用量降到最低，并且在首次使用的时候对每一个都进行定义。

*	循序渐进。为了避免『陷阱门效应』，我专门把这些最为复杂的部分抽离成一个个专题，并且都切分成小规模的部分，一步步来进行。

*	专注于编程，而不是编程语言。我只保留了关于 Java 的最小规模内容，没有涉及更多的细节。


我还需要个标题，就突发奇想，选了个标题叫做『如何像计算机科学家一样思考』。

我的第一版教材很粗糙，不过用起来效果还不错。学生真能看得进去，并且理解了我在课上所讲的那些难点和有趣的专题，最重要的是，他们能够根据这本教材来实践。

之后我就以 GNU 自由文档协议来发布了这本书，这一协议允许所有人去复制、修改以及分发这本书。

接下来的事情很有趣了。Jeff Elkner，维吉尼亚的一位高中教师，他很欣赏我这本书，把这本书从 Java 翻译成了 Python 的版本。他发给我一份『译稿』，然后我开启了阅读『自己的书』来学习 Python 的奇妙经历。于是在 2001 年，我通过 Green Tea Press 出版了本书的第一个 Python 版本。

在 2003 年，我开始在奥林商学院教学，并且第一次开始教 Python 了。这和 Java 的对比很鲜明。学生们省力多了，学得也更多了，在有趣的项目上也更努力，整体上都觉得这一学习过程很有乐趣。从那以后，我就继续维护这本书，修正错误，改进样例、附加资料以及练习题。

结果就产生了现在这本书，现在标题简化了很多——Think Python。

主要的改变如下：

*	在每一章的末尾，我加了关于 debug 的部分。这些内容提供了关于 debug 的一些整体策略，比如如何找到和避免 bug，还有就是关于 Python 一些陷阱进行了提醒。


*	我加了更多的练习，从简单的理解方面的测试，到一些比较充足的项目。大多数练习都有解决方案的样本链接。


*	我还添加了一些案例研究，包含练习、解决方案和讨论的更大规模的样例。


*	此外我还扩展了关于程序开发规划和基本设计模式的讨论。


*	关于 debug 和算法分析，还额外加了一些附录。

	

这本 Think Python 的第二版有如下的新内容：


*	本书内的所有参考代码都升级到 Python3 了。


*	我增加了一部分内容，以及一些关于 web 方面的细节，这是为了帮助初学者能够在浏览器中开始尝试 Python，这样即便你不想安装 Python 也没问题了。


*	在第四章的第一节，我把我自己的一个原来叫做 Swampy 的小乌龟图形包转换撑了一个更标准的 Python 模块，名字叫做 turtle，更好安装，功能也比之前强大了。


*	我还添加了新的一章，叫做『彩蛋』，介绍了一些 Python 的额外功能，严格来说，这些功能并不算必备的，但有时候蛮好用的。


我希望大家能享受学习这本书的过程，也希望这本书能帮助大家学习编程，并且让大家学会像计算机科学家一样思考，哪怕有一点点也好。

    本书英文版原作者：Allen B. Downey（艾伦 唐尼）

                Olin College 奥林商学院

## 致谢

非常感谢 Jeff Elkner，是他把我的 Java 教材翻译成了 Python，才引起了这一项目的开始，并且也把 Python 语言介绍给我，它已经是我最喜欢的编程语言了。
也要感谢 Chris Meyers，他对『如何像计算机科学家一样思考』的一些章节有贡献。
感谢自由软件基金会，是他们提出了 GNU 自由文档协议，在这一协议的帮助下，我和 Jeff 以及 Chris 的合作成为了可能，当然也要感谢我现在使用的知识共享协议。
感谢 Lulu 的编辑们，他们出版了『如何像计算机科学家一样思考』。
感谢 O’Reilly 公司的编辑们，他们出版了这本『Think Python』。

最后还要感谢所有曾对本书早期版本做出过贡献的同学们，以及其他参与改错和提出建议的朋友们（列表如下）。

### 贡献列表

有几百名读者，他们目光敏锐又思维迅捷，在过去的这些年里提供了各种建议，发现了各种错误。他们贡献和热情都是对本项目的巨大帮助。

如果大家有任何意见建议，请发邮件到 feedback@thinkpython2.com 联系我们。如果基于反馈做出了修改，我会将你添加到贡献列表（当然你不想被添加也可以的）。

希望你能至少把出错句子的一部分提供出来，这都让我更容易去搜索。页码和章节编号也可以，但不太容易找。多谢了！

（译者注：以下贡献列表省略不在此处提供，有兴趣的朋友可以去看英文原版。）



## 下载

### Docker

```
docker pull apachecn0/think-py-2e-zh
docker run -tid -p <port>:80 apachecn0/think-py-2e-zh
# 访问 http://localhost:{port} 查看文档
```

### PYPI

```
pip install think-py-2e-zh
think-py-2e-zh <port>
# 访问 http://localhost:{port} 查看文档
```

### NPM

```
npm install -g think-py-2e-zh
think-py-2e-zh <port>
# 访问 http://localhost:{port} 查看文档
```
