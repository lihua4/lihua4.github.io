标准 Markdown
-------

**段落**

```
这个文档自身就是使用 Markdown 编写的。

Markdown 允许你通过编写易读、易写的富文本格式，然后很方便就可以转换成有效的 HTML。
```

**标题**

Setext-style:

```
标题 1
========

标题 2
--------
```

atx-style (尾部的 `#` 是可选的):

```
# 标题 1 #

## 标题 2 ##

###### 标题 6
```


**强调或突出**

```
*突出*   **强调**
_突出_   __强调__
```

**链接**

内联风格 (`title` 是可选的):

```
[我们的官方网站](https://play.google.com/store/apps/dev?id=7902058998609141477 "Title")
```

内联风格 (`title` 是可选的):

```
[Cool Navbar][id]。 之后，可以在文档的其他任意地方, 定义这个链接:

[id]: https://play.google.com/store/apps/details?id=com.melody.loveyun.tnavbar  "Title"
```
**LaTex数学公式**
```
内联公式，请将公式括在中$...$：
$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$
对于显示的公式，请使用$$...$$：
$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$
```
$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$
```
上标和下标，请使用^和_
例如:x_i^2， log2𝑥 使用:\log_2 x
```
$x_i^2$ ，$\log_2 x$
```
和与积分 \sum和\int;
下标是下限，而上标是上限，例如:\sum_1^n
```
$\sum_1^n$
```
分数有常用的三种制作方法,\frac ab ：产生𝑎/𝑏
对于更复杂的分子和分母，请使用{…}，写法： \frac{a+1}{b+1}
如果分子和分母很复杂，则您可能更喜欢\over，它会将所在的组拆分
{a+1\over b+1} 显示为： 𝑎+1/𝑏+1
```
$\frac ab$ ，$\frac{a+1}{b+1}$
```
数学字体
\mathcal {ABC…688} ，\mathbb {ABCDEFGHIJKLMN}，\mathbf {ABC…890} 等一系列字体
```
$\mathcal {ABC…688}$ ，$\mathbb {ABCDEFG}$ ，$\mathbf {ABC…250}$

[点击查看更多LaTex语法](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)


**Email**

```
开发者 email <developer.xuyun@gmail.com> 链接.
```

**图片**

内联风格 (`title` 是可选的):

```
![alt text](https://www.baidu.com/img/bd_logo1.png "百度")
```

引用风格 (`title` 是可选的):

```
![alt text][id]

[id]: https://s3.pstatp.com/aweme/resource/web/static/image/index/logo_efcda07.png "抖音"
```

**列表**

有序列表:

```
1. 列表项 1
2. 列表项 2
```

无序列表:

```
* 列表项 1
* 列表项 2

- 列表项 3
- 列表项 4
```

列表项缩进两个空格就可以创建一个嵌套的列表：

```
1. 列表项 1
  1. 嵌套的列表可以是有序的
  2. 格式和正常的有序、无序列表没有差异
2. 列表项 2
  * 嵌套的列表可以是无序的
    * 这个嵌套的列表项有4个空格的缩进，因为它的父列表项自身就带有2个空格的缩进
    * 还允许更多层的嵌套
3. 列表项 3
```

**引用**

```
> 段落前面添加大于号和空格，就能够形成引用段落。

> > 这是嵌套的引用。
```

**内联代码**

```
`内联代码` 使用反引号包含

你也可以像 `` `这样` `` 转义反引号
```

**代码块**

每行缩进4个空格或者1个 tab：

```
这是一个正常的段落。

    这是代码块。
```

**水平分割线**

三个或更多的星号或横杠：

```

---

* * *

******

- - - - 
```

**强制换行**

在行尾输入两个空格:

```
这句话
不会
换行

这句话
会
换行
```

GitHub Flavored Markdown
-------

**链接自动展示**

你可以直接输入链接地址，它可以直接识别这个链接。

```
https://play.google.com/store/apps/dev?id=7902058998609141477
```

**删除线**

通过两个波浪号将字符包含：

```
~~错误的文本~~
```

**围栏式代码块**

````
```
标准的 Markdown 通过每行开头的4个空格将文本转换成代码块，而 GFM 支持围栏式代码块。只要将代码用 ``` 包含起来即可，不需要4个空格的缩进
```
````

**表格**

这是个简单的表格:

```
First Header | Second Header | Third Header
------------ | ------------- | ------------
Content Cell | Content Cell  | Content Cell
Content Cell | Content Cell  | Content Cell
```

出于美观的考虑, 可以把两端都包围起来:

```
| First Header | Second Header | Third Header |
| ------------ | ------------- | ------------ |
| Content Cell | Content Cell  | Content Cell |
| Content Cell | Content Cell  | Content Cell |
```

通过在标题分割行添加冒号 `:` ,你可以定义表格单元的对其格式：向左靠齐，居中和向右靠齐：

```
First Header | Second Header | Third Header
:----------- | :-----------: | -----------:
Left         | Center        | Right
Left         | Center        | Right
```