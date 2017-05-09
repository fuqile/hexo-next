---
title: Markdown语法 完整版
tags: [Markdown]
categories: Markdown
---
本文参考兔清风的博客，并新增一些语法，原文地址 <http://blog.leanote.com/post/freewalk/Markdown-%E8%AF%AD%E6%B3%95%E6%89%8B%E5%86%8C#title>

准备自己练练手，同时也在此做个记录，方便以后查阅。
## 1. 斜体和粗体

**代码**

```
1. *斜体* 或 _斜体_
2. **粗体**
3. ***加粗斜体***
4. ~~删除线~~
```
**显示效果**

1. *斜体* 或 _斜体_
2. **粗体**
3. ***加粗斜体***
4. ~~删除线~~

## 2. 分级标题

**代码**

```
1. # 一级标题
2. ## 二级标题
3. ### 三级标题
4. #### 四级标题
5. ##### 五级标题
6. ###### 六级标题
```

**显示效果**

1. # 一级标题
2. ## 二级标题
3. ### 三级标题
4. #### 四级标题
5. ##### 五级标题
6. ###### 六级标题

## 3. 超链接

&emsp;&emsp;**Markdown** 支持两种形式的链接语法：行内式和参考式两种，一般行内式使用比较多 

### 3.1 行内式

**语法说明**

+ []里写链接文字，()里写链接地址，()中的“”中可以为链接指定title属性，title属性可加可不加。title属性的效果是鼠标悬停在链接上会出现指定的title文字。`[链接文字](链接地址 “链接标题”)`这样的形式。链接地址与链接标题中间有一个空格。

**代码**

```
1. 欢迎来到[githing的博客](http://blog.githing.com)
2. 欢迎来到[githing的博客](http://blog.githing.com "githing的博客")
```
**显示效果**

1. 欢迎来到[githing的博客](http://blog.githing.com)
2. 欢迎来到[githing的博客](http://blog.githing.com "githing的博客")

### 3.2 参考式

&emsp;&emsp;参考式超链接一般用在学术论文上面，或者另一种情况，如果某一个链接在文章中多处使用，那么使用引用的方式创建链接将非常好，它可以让你对链接进行统一的管理。

**语法说明**

&emsp;&emsp;参考式链接分为两部分，文中的写法`[链接文字][链接标记]`，在文本的任意位置添加`[链接标记]:链接地址 “链接标题”`，链接地址与链接标题前有一个空格。

&emsp;&emsp;如果链接文字本身可以做为链接标记，也可以写成`[链接文字][]`

&emsp;&emsp;`[链接文字]：链接地址`的形式，见代码最后一行。

**代码**

```
1. 我经常去的几个网站[Google][1]、[githing][2]以及[自己的博客][3]
2. [githing的博客][3]是个不错的[网站][]。

[1]:http://www.google.com "Google"
[2]:http://githing.com "githing"
[3]:http://blog.githing.com "githing的博客"
[网站]:http://githing.com
```
**显示效果**

1. 我经常去的几个网站[Google][1]、[githing][2]以及[自己的博客][3]
2. [githing的博客][3]是个不错的[网站][]。

[1]:http://www.google.com "Google"
[2]:http://githing.com "githing"
[3]:http://blog.githing.com "githing的博客"
[网站]:http://githing.com

### 3.3 自动链接

**语法说明**

&emsp;&emsp;**Markdown** 支持以比较简短的自动链接形式来处理网址和电子邮件信箱，只要是用<>包起来，Markdown就会自动把它转成链接。一般网址的链接文字就和链接地址一样，例如：

**代码**

```
1. 这是我的网址<http://githing.com>
2. 这是我的邮箱<rdystwnts@126.com>
```
**显示效果**

1. 这是我的网站<http://githing.com>
2. 这是我的邮箱<rdystwnts@126.com>


