designAppBarLayoutCollapsingToolbarLayout### windows下: 常用快捷键
- ctrl + shift + p 打开搜索,即命令面板
- ctrl + shift + m 预览当前的md文件
- 打开命令面板，输入命令命令Settings View:Open，也可以输入svo，打开设置面板。
- 区块引用 Blockquotes

  标记区块引用是使用 ">" 的引用方式

- 列表

  Markdown 支持有序列表和无序列表。
  无序列表使用星号、加号或是减号作为列表标记：
  有序列表则使用数字接着一个英文句点：

- 代码区块
language-markdown
  要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以，例如，下面的输入：

 ``` java
 <android.support.design.widget.AppBarLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            app:layout_behavior="android.support.design.widget.AppBarLayout$Behavior"
            android:id="@+id/appbar">
```

- 链接：Markdown 支持两种形式的链接语法： 行内式和参考式两种形式

  不管是哪一种，链接文字都是用 [方括号] 来标记。

  1. 要建立一个行内式的链接，只要在方块括号后面紧接着圆括号并插入网址链接即可:
    [markdown基本语法](https://www.jianshu.com/p/f3fd881548ad)

     如果你是要链接到同样主机的资源，你可以使用相对路径：
    [本地图片](C:/Users/akulaku/Desktop/ic_adjust_limit_top_bg.png)
  2. 参考式的链接是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记，接着，在文件的任意处，你可以把这个标记的链接内容定义出来：

      - [1] :https://www.jianshu.com/p/f3fd881548ad
      - [markdown基本语法] :https://www.jianshu.com/p/f3fd881548ad

- 强调

  > Markdown 使用星号（*）和底线（_）作为标记强调字词的符号，被 * 或 _ 包围的字词会被转成用 \<em> 标签包围，用两个 * 或 _ 包起来的话，则会被转成 \<strong>,例如：
  > - *single asterisks*
  > - _single underscores_
  > - **double asterisks**
  > - __double underscores__

- 图片

  本地图片上传
  1. [登录] :http://yotuku.cn/
  2. 上传图片，点击markdown，粘贴到markdown文档即可

### atom的插件必备
- markdown-preview-plus插件

  Atom自带的Markdown预览插件markdown-preview功能比较简单，markdown-preview-plus对其做了功能扩展和增强：
  - 支持预览实时渲染。(Ctrl + Shift + M)
  - 支持Latex公式。(Ctrl + Shift + X)

- markdown-scroll-sync 同步滚动插件
- markdown-table-editor 表格生成插件markdown-preview

| name | age |
| ---- | --- |
| 哈哈 | 10  |

- markdown-themeable-pdf、pdf-view ：pdf导出插件

  Shift+Ctrl+E将markdown文件导出成为pdf

- markdown-image-paste
  > 贴图工具，这个是非常好用的功能，如果你输入的图片非常多，markdown可能是你的噩梦，但是这个工具可以减少一些复杂的操作，但具体的要看你的熟练程度，本人写博客一般都不会写特别长，但是喜欢用图片，一幅图胜过一百句话。
  - 使用截图工具将图片复制到系统剪切板。
  - 在Markdown新起一行输入文件名。
  - Ctrl + V 会自动把图片保存到Markdown文件相同目录下(因此要求Markdown文件应该先保存)，并命名为刚输入的文件名，同时在刚才输入文件名行处生成img标签。
- LaTeX 是写数学公式的法宝
- 换行：可以在前一行的末尾加入至少两个空格
  然后换行写其它的文字或者添加换行符<br/>
- markdown语法：http://xianbai.me/learn-md/article/syntax/paragraphs-and-line-breaks.html
