###1. Markdown文件简明语法
如果你熟悉markdown语法，请跳过这段。

作为一个代码工作者，难免要碰到写文档的事情。写文档的时候难免要在文档中插入代码。可是Word也好，有道云笔记也好，都存在一个缺点：代码无法高亮。用Word的格式去一个个刷吧，太费时间了。直到我这个孤陋寡闻的人发现了markdown。好了，就是它了，太好学，太简单，太强大，太符合要求了。

markdown的设计思想就是要你少用鼠标，你会发现，你使用markdown写文档，会专注于内容本身，而不是排版。

> 备注：有道云笔记4.9版本以后已经开始支持markdown格式，在此对有道云笔记的开发者表示感谢。

有多简单呢？我这里只作一个简单介绍，如果要看相信的介绍，请自己Google或百度。

####1. 段落和标题大纲
标题大纲（类似于HTML的H1, H2, …）

简单得很，一级标题用# 标题, 二级标题用## 标题，三级标题用### 标题，以此类推。

段落（类似HTML的<\p>）标签
    连续的2个回车表示一个段落。就这么简单

####2. 无序列表和有序列表
无序列表每个每个列表项用*开头

有序列表每个列表项用1., 2., ……这样的开头

tab表示缩进一个层级，可以实现列表的嵌套。

####3. 强调和斜体
*我是斜体*这样就是表示一个斜体: 我是斜体

**我是粗体**这样就表示一个粗体：我是粗体

####4. 表示引用和行内代码
>开头，表示引用的文件
用两个’`’把字符包起来，就是现实一个行内代码。类似HTML的<code></code>的效果。
####5. 转义
\ 表示转义。

####6. 横线
---表示一个横线，也就是HTML里的<\hr />标签

####7. 表示链接
[链接的内容](http://www.foo.com/bar)

####8. 表示图片
![微博的Logo](http://img.t.sinajs.cn/.../WB_logo.png)

这里显示的是微博的Logo:

![微博Logo](http://img.t.sinajs.cn/t6/style/images/global_nav/WB_logo.png)


####9. 表示表格
>|表头1|表头2|...|表头N|
>
>|--|--|...|--|
>
>|内容1|内容2|...|内容N|

|  表头1	  | 表头2	    |  表头N    |
| --- | --- | --- |
| 内容1    |   内容2  |   内容N  |


####10. 代码高亮
终于说到代码高亮了，这个更加简单了，看好了，就是这样
> ``` 语言[java/python/php/bash/html/javascript/…]
> 你的代码　
> ```
就是这样简单。
如：
``` java
  public class HelloWorld{
    public static void main(String[] args){
      System.out.println("Hellow World");
    }
  }
```

###2. 安装Atom
Atom是github出品的一个优秀的编辑器，支持C、C++、Java、HTML、SQL、Python、PHP等超过20种的编程语言。用Atom来编写Markdown，算是一种“杀鸡用牛刀”。我试用过使用Sublime Text，微软的Visual Studio Code和Atom三个软件编写markdown，结果是Atom最舒服，没有之一。
![](https://img-blog.csdn.net/20160517232609868)


[官网下载Atom](https://atom.io/)，一路 Next 大法完成安装。

###3. Atom编写Markdown文件
编写就按markdown的规矩来写。Ctrl + Shift + M 可以召唤出markdown预览界面，再按一次可以取消预览。

###4. 导出PDF文件
Atom 有个插件markdown-pdf可以导出markdown为pdf文件，便于交流。为什么推荐这个插件呢？理由如下：
1. 免费的。很多在线的markdown编辑器导出PDF文件的功能只对会员开放，就是要钱。这个无可厚非，可是不给试用几次我怎么才能知道导出的效果呢？
2. 导出的文件的代码也是高亮的。VS Code有md2pdf这个插件，可惜导出的pdf的代码不高亮。

4.1. 安装markdown-pdf

    1.点击 File -> Settings -> Install

![](https://img-blog.csdn.net/20160517233047448)


    2.输入 markdown-pdf 并按 回车键
![](https://img-blog.csdn.net/20160517233407684)

    3.点击 Install

    4.重启Atom

4.2. 导出PDF

![](https://img-blog.csdn.net/20160517233437742)
