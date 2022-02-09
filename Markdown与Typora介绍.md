# Markdown与Typora

转载自[最齐的Tpora使用教程](https://blog.csdn.net/qq_41261251/article/details/102817673)

---

版权声明：本文为CSDN博主「水木子_」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/qq_41261251/article/details/102817673

## 一、Markdown与[Typora](https://so.csdn.net/so/search?q=Typora&spm=1001.2101.3001.7020)介绍

### 1.1 Markdown介绍

```
Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。

Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。

Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。

Markdown 编写的文档后缀为 .md, .markdown。
```

### 1.2 Typora介绍与下载

Typora编辑器让人们能更简单地用Markdown语言书写文字，解决了使用传统的Markdown编辑器写文的痛点，并且界面简洁优美，实现了实时预览等功能。

Typora官网： https://typora.io/

windos版本下载地址：https://typora.io/#windows

请根据自己的电脑配置自行下载安装，过程简单，在此不多做介绍。

## 二、Markdown语法

### 2.1 标题

使用 **#** 可以表示标题，一级标题对应一个 **#** ，二级标题对应两个 **#** 号，最多至六级标题。在Typora中，**#** 后要紧接着一个空格才能表示标题，否则就是普通字符。

在Typora中，也可以使用快捷键Ctrl+1（2，3，4，5，6）表示相对应的标题。Ctrl+0表示段落。标题快捷键信息可在菜单栏中的段落选项下查看。

### 2.2 字体

用一对星号`*`括住的文本表示斜体文本，如：*要变斜体的文本*，斜体文本 ；
也可以用一对下划线`_`括住文本来表示斜体文本，如：_要变斜体的文本_，斜体文本 ；
也可以使用Typora的快捷键Ctrl+I来表示斜体文本。

用一对`**`括住的文本表示粗体文本，如：**要变粗体的文本**，粗体文本；
也可以用一对`__`括住的文本来表示粗体文本，如：__要变粗体的文本__，粗体文本；
也可以使用Typora的快捷键Ctrl+B来表示粗体文本。

用一对`***`括住的文本表示粗斜体文本，如：***要变粗斜体的文本***，粗斜体文本；
也可以用一对`___`括住的文本来表示粗斜体文本，如：___要变粗斜体的文本___

### 2.3 各种线

分割线，可以使用三个及以上的 + 号或 * 号或 - 来表示一条分割线；
由三个*号表示的分割线：

***

由三个+号表示的分割线：

+++

由三个-号表示的分割线：

---

删除线，可以使用一对`~~`括住的文本来表示删除文本，如：~~要加删除线的文本~~，删除文本；在Typora中，也可以使用快捷键Alt+Shift+5来加删除线，语法相同，删除线。
下划线，可以使用HTML的标签<u>和</u>表示增加下划线的文本，如：<u>要增加下划线的文本</u>，下划线；在Typora中，也可以使用快捷键Ctrl+U来增加下划线，语法也是相同的，下划线。

### 2.4 列表

#### 无序列表

可以使用`*`，`+`或`-`标记符号来表示无序列表项，记住要在标记符号后**添加一个空格**，语法显示如下：

```
* 第一项
* 第二项
+ 第一项
+ 第二项
- 第一项
- 第二项
```

结果如下：

* 第一项
* 第二项
+ 第一项
+ 第二项
- 第一项
- 第二项

#### 有序列表

可以使用**数字加上`.`再加上空格**来表示有序列表，语法如下：

```
1. 第一项
3. 第二项
10. 第三项
```

结果如下：

1. 第一项
2. 第二项
3. 第三项

从结果可以看出，数字并不重要。

**嵌套列表**

- 一
  - 1.1
    - 1.1.1
      - 1.1.1.2
        - 1.1.1.3
- 二
  - 2.1
    - 2.1.1
    - 1. 有序列表第一项
      2. 有序列表第二项

首先使用`*`、`+`或`-`进入列表，然后回车换行，会发现系统自动生成列表第二项，此时按下**Tab**键，列表第二项变为第一项的子列表。**按回车退出当前列表**。可以在无序列表中嵌套有序列表。 

1. 一
   1. 一、一
      1. 一、一、一
         1. 一、一、一、一
         2. 一、一、一、二
2. 二
   1. 二、一
   2. - 无序列表第一项
      - 无序列表第二项

也可以在有序列表中嵌套无序列表。

### 2.5 区块

当我们想要引用别人的文章内容时，可以将其放在区块内。

可以使用`>`加空格来表示区块。

> 这是区块
>
> 区块也可以嵌套
>
> > 二级区块
> >
> > > 三级区块

要退出区块，同样使用`Enter`键即可。

### 2.6 代码

如果是一行代码，可以使用段内代码块来表示，用一对 **`**（数字1旁边的符号）括住代码。

比如`printf("Hello World!")`

如果是代码段，那么可以使用**三个 ` 加Enter/空格+编程语言**来表示。如：

如果是代码段，那么可以使用**三个 ` 加Enter/空格+编程语言**来表示。如：

```c
# include <stdio.h>
void main(){
	printf("Hello world!\n");
}
1234
```

可以在代码块的右下角选择编程语言。

### 2.7 链接

链接的使用方式有两种语法，如下：

```
[链接文字](链接地址)
或
<链接地址>
123
```

我们可以使用链接打开网页，示例如下：

```
[百度](https://www.baidu.com/)
<https://www.baidu.com/>
12
```

显示效果如下：

[百度](https://www.baidu.com/)
https://www.baidu.com/

当鼠标移到相应的链接文字时，按住**Ctrl+鼠标左键**点击访问。

链接除了可以打开相应的网页外，还可以**打开本地文件**，使用方式类似，不过链接地址需要使用本地文件的地址，相对地址、绝对地址均可：

示例：

```
[打开LinkTest.md文档](./LinkTest.md)
[打开LinkTest.png照片](./img/LinkTest.png)
12
```

结果如下：

[打开LinkTest.md文档](https://blog.csdn.net/qq_41261251/article/details/LinkTest.md)

[打开LinkTest.png照片](https://blog.csdn.net/qq_41261251/article/details/img/LinkTest.png)

经测试可以打开相应的文件。但是不能使用`<要打开的文件地址>`来打开相应的文件，比如<./LinkTest.md>并没有表现为可链接状态。

补充知识：

一个小圆点`.`表示当前目录，故`./LinkTest.md`表示当前目录下的LinkTest.md文件，`./img/LinkTest.png`表示当前目录下的img文件下的LinkTest.png文件。

两个小圆点`..`表示上一级目录。

我们也可以使用链接来实现**页内跳转**，语法为：

```
[链接文字](#标题文字)
1
```

示例：

```
[跳转到第一章第一节](#1.1 Markdown介绍)
1
```

结果如下：

[跳转到第一章第一节](#1.1 Markdown介绍)

经测试，可以成功跳转。

### 2.8 图片

我们也可以在Markdown文档中插入图片，语法如下：

```
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
123
```

- 首先一个感叹号
- 然后中括号里面写属性文本
- 小括号里面写图片地址，后可接标题

示例语法：

```
![本地png图片PictureTest.png](./img/PictureTest.png)

![本地jpg图片](./img/PictureTest.jpg)

![网络图片](http://static.runoob.com/images/runoob-logo.png "菜鸟教程")
```

结果如下：

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-EqvQOozY-1572414627611)(img/PictureTest.png)]](https://img-blog.csdnimg.cn/20191108173048186.png)

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-SJe9oWf3-1572414627613)(img/PictureTest.jpg)]](https://img-blog.csdnimg.cn/20191108173059240.jpg)

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-o6fdyzYF-1572414627614)(img/runoob-logo.png "菜鸟教程")]](https://img-blog.csdnimg.cn/20191108173109242.png)

在Typora中，也可以直接使用`Ctrl+C`，`Ctrl+V`来直接进行复制粘贴图片，但是，由于Markdown是需要图片的地址的，所以需要简单设置一下Typora。

**点击文件 --> 偏好设置 --> 图像**，如下：

可以自行设置选择将图片复制到哪个文件夹。

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-cJcfQ4sd-1572414627616)(img/image-20191029190539469.png)]](https://img-blog.csdnimg.cn/20191108173127600.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzQxMjYxMjUx,size_16,color_FFFFFF,t_70)

这里选择复制到指定路径，然后在下面一栏中填写./img，表示将图片复制到你正在编辑的文档同一级的img文件夹下。在下面的选项中，勾选第一、二、三项。正因为勾选了第二项，所以当我们在插入网络图片时，Typora会自动帮我们将网络图片下载到指定的路径下，前面的"菜鸟教程"图片便是如此。

![[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传(img-tPqjvvPS-1572414627619)(img/image-20191029190813277.png)]](https://img-blog.csdnimg.cn/20191108173139695.png)

由于Markdown的特殊语法，故经常会出现图片加载失败的情况，很大的可能就是因为在指定的路径上找不到相应的图片，当然，有时候也是由于Typora的原因，重启Typora即可。

### 2.9 表格

Markdown 制作表格使用 `|` 来分隔不同的单元格，使用 `-` 来分隔表头和其他行。

语法如下：

```
|表头|表头|表头|
|---|---|----|
|单元格|单元格|单元格|
|单元格|单元格|单元格|
```

结果如下：

| 表头   | 表头   | 表头   |
| ------ | ------ | ------ |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |

我们可以设置对齐方式：

- `:-`表示左对齐
- `-:`表示右对齐
- `:-:`表示中间对齐

示例如下：

```
|左对齐|右对齐|中间对齐|
|:---|---:|:----:|
|单元格|单元格|单元格|
|单元格|单元格|单元格|
```

结果如下：

| 左对齐 | 右对齐 | 中间对齐 |
| ------ | ------ | -------- |
| 单元格 | 单元格 | 单元格   |
| 单元格 | 单元格 | 单元格   |

在Typora中，我们可以使用快捷键**Ctrl+T**来插入表格，并选择行列，当选中表格某一单元格时，可以在表格左上角手动设置对齐方式，右上角选择更多操作。

## 三、Typora与数学公式

在本章中，重点不在于介绍如何插入数学公式，而在于如何表示数学符号。

### 3.1 如何插入数学公式

在Typora中，有两种方法插入数学公式，语法为：

```
第一种方法：$数学公式$
第二种方法：
$$
数学公式
$$
```

第一种方法表示插入行内公式（内联公式），即可以将公式插入到一行中，比如$1+2=3$这样的公式。

第二种方法表示插入行间公式（外联公式），即可以将公式插入到行与行之间，单独占据一行或者数行的空间，并且居中放置。 
$$
1+2=3\\1+3=4
$$
如果要在行间公式内换行，在换行的位置使用`\\`。

接下来重点介绍如何表示数学符号。

3.2 上标下标
上下标可以使用^，_后跟相应的符号来实现。如：

上标  ：$a^1$ ， 下 标 ： $a_1$ 
如果作为上标、下标的符号不止一个，则需要用花括号{}将其括起来。如：

上标为12：$a^{12}$,下标为34：$a_{34}$
$$
f(x)=x^{x^x}\\e^{x^2}\\e^{x^2}
$$

### 3.3 根号

我们可以使用`\sqrt{}`来表示根号。如：
$$
\sqrt{2},\sqrt{5}
$$
我们也可以使用`\sqrt[]{}`来表示更具体的根号信息：

```
\sqrt[3]{4}，\sqrt[4]{10}
```

$$
\sqrt[3]{4}，\sqrt[4]{10}
$$

### 3.4 上下水平线

我们可以使用`\underline{}`,`\overline{}`来表示上下水平线，如：

```
$下水平线：\underline{a+b}$
$上水平线：\overline{a+b}$
```

结果为：

$下水平线：\underline{a+b}$
$上水平线：\overline{a+b}$

### 3.5 上下水平大括号

我们可以使用`\overbrace{}` 和 `\underbrace{}` 在表达式的上、下方给出一水平的大括号

```
$\overbrace{x_1+x_2+x_3}$
$\underbrace{x_1+x_2+x_3}$
```

$\overbrace{x_1+x_2+x_3}$
$\underbrace{x_1+x_2+x_3}$

当然，我们也可以在括号上添加说明，使用语法为`\overbrace{}^{}`和`\underbrace{}_{}`

```
$\overbrace{x_1+x_2+x_3}^{3个元素}$
$\underbrace{x_1+x_2+x_3}_{3个元素}$
```

$\overbrace{x_1+x_2+x_3}^{3个元素}$
$\underbrace{x_1+x_2+x_3}_{3个元素}$

### 3.6 向量符号

我们可以使用`\vec{}`来表示单个字母向量，其实也可以表示多个字母，但不美观，另两个命令`\overrightarrow{}` 和`\overleftarrow{}`在定义从A 到B 的向量时非常有用。如：

```
$\vec{a}$
$\vec{AB}$
$\vec{ABC}$
$\overrightarrow{AB}$
$\overleftarrow{AB}$
```

$\vec{a}$
$\vec{AB}$
$\vec{ABC}$
$\overrightarrow{AB}$
$\overleftarrow{AB}$

我们可以使用`\frac{}{}`来表示分数，如：

```
$\frac{1}{2}$
$\frac{\sqrt{3}}{4}$
```

$\frac{1}{2}$
$\frac{\sqrt{3}}{4}$

### 3.8 积分运算符

积分运算符用`\int` 来生成 ，用`\int_{}^{}`来表示积分上下界，如：

```
$\int$
$\int_{1}^{2}$
```

$\int$
$\int_{1}^{2}$

### 3.9 求和运算符

求和运算符可以使用`\sum`来生成，用`\sum_{}^{}`来表示求和上下界，如：

```
$\sum$
$\sum_{i=1}^{10}x_i$
```

$\sum$
$\sum_{i=1}^{10}x_i$

求和符号的上下标在内联公式里，表现为上面那样，当在外联公式里时，表现如下：
$$
$\sum_{i=1}^{10}x_i$
$$

### 3.10 连乘运算符

连乘运算符用`\prod{}`表示，同样地，上下标用`prod_{}^{}`表示，如：

```
$\prod$
$\prod_{i=1}^{10}x_i$
$$
\prod_{i=1}^{10}x_i
$$
```

$\prod$
$\prod_{i=1}^{10}x_i$
$$
\prod_{i=1}^{10}x_i
$$

### 3.11 特殊符号

#### 希腊字母

α`\alpha`，β `\beta`，γ `\gammaγ`，θ `\thetaθ`，ρ` \rho`，λ `\lambda`，μ `\mu`

Δ `\Delta`，π `\pi`，Ω `\Omega`

关系运算符

大于>，大于等于≥ 为`\geq`或`\ge`

小于<，小于等于≤ 为`\leq`或`\le`

等于=，不等于≠ `\neq`或`ne` 

加减乘除

加+ 减-

乘×为`\times` 除÷为`\div`

### 3.12 矩阵表示

我们可以使用以下格式来显示矩阵：

```
$$
\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6\\
\end{matrix}
$$
```

$$
\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6\\
\end{matrix}
$$

可是这并不是我们常见的矩阵啊，旁边的中括号呢？

别急，我们先把上面的公式说明一下：

- `\begin{matrix}`和`\end{matrix}`说明在它们之间的是矩阵
- `1 & 2 & 3\\`表示第一行的元素，其中用`&`来分割每一个元素，用`\\`来换行

```
$$
\left[\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6
\end{matrix}\right]
$$
```

$$
\left[\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6
\end{matrix}\right]
$$

其实我们仅仅在`\begin{matrix}`前面加了`\left[`，在`\end{matrix}`后面加了`\right]`，这样就能正确显示括号了，那我们可以将`[]`改为`||`吗，当然可以，就简单地把`\left[`，`\right]`改为`\left|`和`\right|`即可。

```
$$
\left|\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6
\end{matrix}\right|
$$
```

$$
\left|\begin{matrix}
1 & 2 & 3\\
4 & 5 & 6
\end{matrix}\right|
$$

### 3.13 方程组

```
$$
\begin{equation}
\left\{
             \begin{array}{lr}
             x=\dfrac{3\pi}{2}(1+2t)\cos(\dfrac{3\pi}{2}(1+2t)), &  \\
             y=s, & 0\leq s\leq L,|t|\leq1.\\
             z=\dfrac{3\pi}{2}(1+2t)\sin(\dfrac{3\pi}{2}(1+2t)), &  
             \end{array}
\right.
\end{equation}
$$
```

$$
\begin{equation}
\left\{
             \begin{array}{lr}
             x=\dfrac{3\pi}{2}(1+2t)\cos({\dfrac{3\pi}{2}(1+2t)}), &  \\
             y=s, & 0\leq s\leq L,|t|\leq1.\\
             z=\dfrac{3\pi}{2}(1+2t)\sin({\dfrac{3\pi}{2}(1+2t)}), &  
             \end{array}
\right.
\end{equation}
$$

现在我们一一来解释：

- `begin{equation}`与`\end{euqation}`表示它们之间的为方程组。

- `\left\{`和`\right`.表示在方程组的左边加上`{`，在右边加上`.`，因为{在外联公式中有特殊的意义，因此需要在其前面加上转义字符\。

- `\begin{array}`和`\end{array}`表示它们之间的是数组，其实这也可以用来表示矩阵。

- `{lr}`表示有两列，第一列的值靠左排列，用`l`表示，第二列的值靠右排列，用`r`表示，如果是中间对齐则为`c`。

- 然后下面三行是方程式，用`&`分割，用`\\`换行。

### 3.14 分段函数

其实分段函数与方程组类似，示例如下：

```
$$
y=
\begin{equation}
	\left\{
		\begin{array}{lr}
		x-1 & x \leq 0
		x+1 & x>0
		\end{array}
	\right. 
\end{equation}
$$

```

$$
y=
\begin{equation}
	\left\{
		\begin{array}{lr}
		x-1 & x \leq 0
		x+1 & x>0
		\end{array}
	\right. 
\end{equation}
$$

就是在`\begin{equation}`前加`y=`即可。

## 四、Typora与HTML

### 4.1 改变字体颜色及大小

我们可以使用`<font> </font>`标签来改变字体的颜色及大小，如：

```
<font size=3 color="red">字体颜色为红色，大小为3</font>

<font size=4 color="blue">字体颜色为蓝色，大小为4</font>

<font size=6 color="violet">字体颜色为紫罗兰，大小为6</font>
```

<font size=3 color="red">字体颜色为红色，大小为3</font>

<font size=4 color="blue">字体颜色为蓝色，大小为4</font>

<font size=6 color="violet">字体颜色为紫罗兰，大小为6</font>

属性`size`表示字体大小，`color`表示颜色。

### 4.2 改变对齐方式

我们可以改变字体的对齐方式，用标签`<p> </p>`加上属性`align`，如：

```
<p align="left">左对齐</p>
<p align="center">中间对齐</p>
<p align="right">右对齐</p>
```

<p align="left">左对齐</p>
<p align="center">中间对齐</p>
<p align="right">右对齐</p>

我们可以通过标签`<img src=url />`来插入图片，如：

```
<img src="img/1.jpg" />
```

<img src = "Markdown%E4%B8%8ETypora%E4%BB%8B%E7%BB%8D.assets/20191108173413620.jpg"/>

我们可以改变`<img>`标签的属性，来改变图片的大小。

```
<img src="img/1.jpg" width=100 height=100/>
```

<img src = "Markdown%E4%B8%8ETypora%E4%BB%8B%E7%BB%8D.assets/20191108173413620.jpg" width=100 height=100/>

也可以改变图片的位置，如：

```<img src="img/1.jpg" width=30 height=30 style="float:left"/>图片在左边```
```<img src="img/1.jpg" width=30 height=30 style="float:right"/>图片在右边```
<img src = "Markdown%E4%B8%8ETypora%E4%BB%8B%E7%BB%8D.assets/20191108173413620.jpg" style = "float:left"/>

<img src = "Markdown%E4%B8%8ETypora%E4%BB%8B%E7%BB%8D.assets/20191108173413620.jpg" style = "float:right"/>

## 五、扩展用法

### 5.1 插入emoji表情

我们可以使用`:emoji:`的语法来插入表情，比如：

:happy:的语法为`:happy:`

🦀的语法为`:crab:`

🐴的语法为`:horse:`

### 5.2 插入目录

当我们为使用标题将文分章节后，可以在输入`[toc]`命令的地方自动根据标题生成目录。

### 5.3 导出

选择文件 --> 导出，可以选择导出的文件格式，有pdf,html,word等格式。

### 5.4 文本高亮

在Typora中，可以用一对`==`将要高亮的文本括起来，如：

```==要高亮的文本== ```

```==背景会用黄色填充==```

==要高亮的文本==
==背景会用黄色填充==

这个功能可在偏好设置 --> Markdown扩展语法中设置。

### 5.5 上下标

在Typora中，可以用一对`~`将下标括起来，如：`H~2~O`表示H2O

同样，我们也可以用一对`^`将上标括起来，如：`X^2^`表示X2

上下标可在偏好设置 --> Markdown扩展语法中设置。

### 六、参考资料

[1] 菜鸟Markdown教程：https://www.runoob.com/markdown/md-tutorial.html

[2] 更多数学符号表达式：http://mohu.org/info/symbols/symbols.htm

[3] Latex 方程组表示： https://blog.csdn.net/lemolemac/article/details/9057471

[4] 菜鸟HTML教程：https://www.runoob.com/html/html-tutorial.html
