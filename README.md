#  Markdown基础


- **Markdown和扩展Markdown简洁的语法**
- **代码块高亮**
- **图片链接和图片上传**
- ***LaTex\*数学公式**
- **导入导出Markdown文件**
- **丰富的快捷键**

------

## 快捷键

- 加粗 `Ctrl + B`
- 斜体 `Ctrl + I`
- 引用 `Ctrl + Q`
- 插入链接 `Ctrl + L`
- 插入代码 `Ctrl + K`
- 插入图片 `Ctrl + G`
- 提升标题 `Ctrl + H`
- 有序列表 `Ctrl + O`
- 无序列表 `Ctrl + U`
- 横线 `Ctrl + R`
- 撤销 `Ctrl + Z`
- 重做 `Ctrl + Y`

## Markdown及扩展

> Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档，然后转换成格式丰富的HTML页面。 —— [[ 维基百科 \]](https://zh.wikipedia.org/wiki/Markdown)



[使用简单的符号标识不同的标题，将某些文字标记为**粗体**或者*斜体*，创建一个](https://zh.wikipedia.org/wiki/Markdown)[链接](http://www.csdn.net/)等，详细语法参考帮助？。

### 表格

**Markdown　Extra**　表格语法：

| 项目     | 价格  |
| -------- | ----- |
| Computer | $1600 |
| Phone    | $12   |
| Pipe     | $1    |

可以使用冒号来定义对齐方式：

| 项目     | 价格    | 数量 |
| -------- | ------- | ---- |
| Computer | 1600 元 | 5    |
| Phone    | 12 元   | 12   |
| Pipe     | 1 元    | 234  |

### 定义列表

**Markdown　Extra**　定义列表语法： 

项目1

: 定义 A

项目2

: 定义 B

项目3

: 定义 C

: 定义 D

```
> 定义D内容
```

### 代码块

代码块语法遵循标准markdown代码，例如：

```
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None
class SomeClass:
    pass
>>> message = '''interpreter
... prompt'''
```

## 自定义字体颜色(github中看不到颜色):

Hello

## 删除线

~~Hello~~

\###脚注 生成一个脚注[^footnote]. [^footnote]: 这里是 **脚注** 的 *内容*.

### 目录

用 `[TOC]`来生成目录：

[TOC]

### 数学公式

使用MathJax渲染*LaTex* 数学公式，详见[math.stackexchange.com](http://math.stackexchange.com/).

- 行内公式，数学公式为：$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$。

- 块级公式：

  $ x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$

更多LaTex语法请参考   

[LaTeX技巧10：LaTeX数学公式输入初级入门_](http://blog.sina.com.cn/s/blog_5e16f1770100fs38.html 'LaTeX技巧10：LaTeX数学公式输入初级入门_LaTeX_Fun_新浪博客,LaTeX_Fun,')

[LaTeX 第五课：数学公式排版 ](https://zhuanlan.zhihu.com/p/24502400 '本文同时发布于微信公众号：两个少年的奇幻漂流（ID：Amazing_Adventure）本期的主要内容是数学公式的排版，包含以下内容：行内公式与行间公式数学结构的输入数学符号的输入多行公式排版数学公式的排版是 LaTeX 的…')

### UML 图:

可以渲染序列图：

```
张三->李四: 嘿，小四儿, 写博客了没
Note right of 李四: 李四愣了一下，说：
李四-->张三: 忙得吐血，哪有时间写。
```

或者流程图：

```
st=>start: 开始
e=>end: 结束
op=>operation: 我的操作
cond=>condition: 确认？

st->op->cond
cond(yes)->e
cond(no)->op
```

- 关于 **序列图** 语法，参考 [Markdown 进阶技能：用代码画时序图 ](https://zhuanlan.zhihu.com/p/70261692 '这篇文章将为大家介绍如何以写代码的方式画时序图（也叫顺序图），同时也会介绍一些时序图基础知识。相比于使用画图工具拖拽画图，用代码画图有什么好处？首先，这种方式非常轻便，无需安装复杂的画图应用。Typora…').
- 关于 **流程图** 语法，参考[MarkDown不能画流程图？其实很简单 ](https://zhuanlan.zhihu.com/p/28468233 '前言MarkDown的简便性让人越来越喜欢。虽然MarkDown也不是万能的，有些排版等MarkDown做起来也不是那么完美，尤其是涉及图片操作。在日常的文档生产中，难免要用到一些流程图，一般用亿图图示等流程图软件画好了导…').
