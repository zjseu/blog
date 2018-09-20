---
title: Markdown教程
date: 2018-09-16 22:59:40
tags: Markdown
---

最近打算整一个博客，记录一些工作中学习的知识、生活上偶尔的随笔。之前一直都是在有道云笔记上记录学习或是工作中遇到的问题，但是发现这样不太方便和其他同学进行交流，因此萌生了创建个人博客的想法。

开始搭建之前，Google了很多前辈搭建博客的方式，比较之下，最终采用的是[**Github+Hexo**方式搭建博客](#todo)。在使用Hexo的过程中，发现$ hexo new [layout] *title*生成的是.md格式的文件，这个文件就是由Markdown语言编写的。工欲善其事，必先利其器，为了便于之后博客的编写，个人博客的第一篇文章就献给了Markdown了。

[Markdown](https://zh.wikipedia.org/zh-hans/Markdown)在维基百科上的定义是“一种轻量级标记语言，允许人们使用易于读写的**纯文本**格式编写文档，然后转换成有效的HTML文档”。通过简单的标记语法，使得普通文本内容具有一定的格式。

* *斜体*

  文本编辑中，少不了对一些特殊单词进行“倾斜”的操作。在Markdown中，可以使用(*)包裹需要“斜体”的内容。除此以外，还可以使用(_)。

* **加粗**

  除了斜体以外，加粗同样是常见的操作。Markdown语法中，使用(**)修饰加粗的内容。

* **_加粗斜体_**

  可以利用(_)与(*)的搭配，使一块文本同时具有斜体与加粗的效果。

* # 一级标题

  Markdown中一共有6个层级的标题，标题通过(#)定义，几级标题就用几个(#)表示。例如###表示三级标题。

  ## 二级标题

  ### 三级标题

  #### 四级标题

  ##### 五级标题

  ###### 六级标题

* 超链接

  Markdown有两种超链接的方式。

  * [内联链接](#InlineLink)，将超链接绑定到一块文本上。例如[Markdown教程](http://www.markdowntutorial.com)，当点击有超链接的文本时，就会跳转到绑定的链接上。采用的方式是在[]中括号之后紧跟()小括号，中括号中的内容就是文本，小括号中的内容就是需要绑定的链接。

  * [引用链接][reference link]，引用链接是链接到文本中的其他地方。例如[跳转到Baidu][reference link]，采用的方式是在[]中括号之后紧跟[]中括号，第一个中括号中是文本，第二个中括号就是链接的地址（其指向一个外部链接）。引用链接的优势是指向同一个链接的多处文本可以复用链接地址，如果有修改，也只需要修改一处即可。

    [reference link]: http://www.baidu.com

* 图片

  在Markdown中插入图片的语法与创建超链接的类似。在图片中，也有类似超链接的两种插入方式。插入图片的语法比超链接的多了一个**感叹号!**。语法为! + [] + ()或[]

  * ![内联图片](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1537114317327&di=dad1b2816b29ec481ced226b0860ce4b&imgtype=0&src=http%3A%2F%2Fimg.mp.itc.cn%2Fupload%2F20161104%2Fc8af1f32614a4c5bb039e409ce0ba0a4_th.jpeg)

  * ![引用图片][reference image]

    [reference image]: https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1537114391779&di=6e07d327ed31c7caaa6a378d87725d16&imgtype=0&src=http%3A%2F%2Fwww.talkimages.cn%2Fimages%2Fmedium%2F20133066%2Ftkf003_377874.jpg

* 大段引用

  > Markdown中标记大段引用的方式就是在一段话前利用**大于号>**进行标记。
  >
  > 多行标记就需要在每行开头用**>**标记（包括空行）

* 列表

  Markdown中列表也有两种表示：

  * 无序列表，无序列表以*符号前缀修饰，展示出来的结果就是这篇文章里的每个操作列一样。
  * 有序列表，有序列表以数字开头：
    1. 这是有序列表1
    2. 这是有序列表2

* 分隔线

  三个连续的-号表示细分隔线。

  ---

  三个连续的*号表示粗分隔线。

  ***

* 代码块

  Markdown代码块：

  ```Java
  public class Program {
      public static void main(String[] args) {
          System.out.println("this is a java code in markdown");
      }
  }
  ```

* 编辑器

  目前用的Markdown的编辑器是[Typora](https://typora.io/)，体验还不错，推荐一发。

以上都是一些基础的语法，Markdown的扩展后续再写。

