---
title: LaTeX, HTML, Markdown 的区别
date: 2025-05-01 17:53 +/-TTTT 0000
categories: [计算机, Markdown]
tags: [静态网站, markdown, latex]     # TAG names should always be lowercase
---

本文介绍几种标记语言之间的区别。

## LaTex & Tex

LaTeX 是一种基于 TeX 的排版系统，适合高质量文档排版设计，特别**适合学术论文、书籍、技术文档等**需要复杂数学公式、图表和格式的排版。输出结果美观且专业。

> 这里有一个非常有意思的网站：[TeX — Beauty and Fun](https://docs.huihoo.com/homepage/shredderyin/tex_frame.html)    

下面为内容节选：   
>其实世界上只有一个TeX程序，它就叫做 "tex", 它是由 D. E. Knuth 设计并且实现的。   
TeX 不仅是一个排版程序，而且是一种程序语言。   
>
>LaTeX 就是用这种语言写成的一个“TeX 宏包”，它扩展了 TeX 的功能，
>**使我们很方便的逻辑的进行创作而不是专心于字体，缩进这些烦人的东西。**   

>TeX 还有其它的大型宏包，它们和 LaTeX 一起 都被叫做 "format"，现在还有一种常用的>format叫做 ConTeXt, 用 它能方便的作出漂亮的幻灯片，动态屏幕文档…… 
>我们通常用 TeX 都是在用 LaTeX, ConTeXt, 因为 TeX 的底层需要更多的知识才能了解，**一般人不需要自己设计自己的格式。**

>TeX 主要依靠 BibTeX 实现文献管理。作者可以从杂志，协会，网站等地方得到 BitTeX 文献数据库，然后在自己的文件里只需要写一个几个字母长的标识符，比如 "kn95"，**就可以自动在论文，书籍末尾加上已经引用的文献的参考文献条目。** 文献条目可以自动排序，也可以不排序。

>**作者们有了这些风格文件，可以一瞬间把已经写好的论文转化成投稿需要的格式。**真的是一瞬间，你试试在LaTeX 文档的 开头把 \documentclass{article} 改成 \documentclass[twocolomn]{IEEEtran}
运行 LaTeX，马上就得到一篇可以投到 IEEE transactions，并且满足他们所有的格式要求的文章。



> **这就是为什么经济学投稿文章的时候，有的杂志会要求LaTeX格式。**


Latex官网：[LaTeX](https://www.latex-project.org/)   
Latex官网下载：[LaTeX/Get](https://www.latex-project.org/get/)   
在线编译（**本人推荐**）：[Overleaf](https://www.overleaf.com/)   

本人推荐在线编辑，因为能少下一个软件是一个。本人用过Overleaf，能直接在线编译和预览，非常方便。Overleaf也是包括在LaTeX官网推荐的几款软件中的。



## HTML & Latex
HTML（HyperText Markup Language，超文本标记语言）是用于创建**网页**的标记语言，定义网页的结构和内容。支持超链接、图像、视频等多媒体。

**本人观点：** 
> **Latex 用来专业排版，输出PDF用来打印。**   
> **HTML 用来构建网页内容。动态或者静态网页。**

> Latex 通过直接引用设计好的格式来形成非常完美的排版，让内容创作和格式排版分开。   
> HTML 通过追加 CSS 文件来进行网页格式和样式的调整，通过追加 JavaScript 文件来进行网页动态的设计。

## Markdown & Latex
Markdown 是一种轻量级标记语言。特点是简单易读、易写，适合快速编写。   
优点是快速，非常快速的生成一个大致的结构，但是缺点是丧失了精美的排版，并且语法不是完全统一。   


比如下文，快速插入一行代码。

```
print(hello world)
```

Latex是纯学术风格，写paper写书用, 适合长篇、精致，比如数学公式、图片位置调整、表格样式调整。   
Markdown是程序员风格，写笔记贴代码片段用。更便利于代码的粘贴。


Markdown 官方指南： [Markdown Guide](https://www.markdownguide.org/)
官网提供了很多本地和线上编译器。参考：[MD: Document](https://www.markdownguide.org/getting-started/#documents)   

**本人观点：**
> **我认为 Markdown 是一种非常适合记笔记的语法。 强推！**   
> 你可以在任何地方用markdown语法书写快速笔记，然后只需要后期命名为`.md`后缀即可。   
> 但是我觉得直接用 VS Code 编译 Markdown 很好！因为能少下一个软件就少下一个。   



## Markdown & HTML
Markdown 的定义是“轻量级”标记语言，而HTML是“超”。   
HTML 偏重精确性，文档结构准确无误；Markdown 强调流畅性，标记简单且与渲染效果相似。

就工作原理而言，我们所写的Markdown 格式文本，也是最终转换为HTML 进而在网页上呈现。   


祝您愉快，以上
> 活得潦草一点，随心一点，谁不干错事儿呢
{: .prompt-tip }
