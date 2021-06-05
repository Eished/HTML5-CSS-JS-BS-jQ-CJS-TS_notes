# 极客学院HTML5+CSS+JS+Bootstrap+jQuery+CreateJS+TypeScript+实战系列视频

## 1. HTML5 开发前准备

## 2. HTML5 基础

### 2.1 HTML5特性简介

#### 2.1.1 什么是HTML5

> HTML5 是 W3C 与 WHATWG 合作的结果,WHATWG 指 Web Hypertext Application Technology Working Group。
>
> WHATWG 致力于 web 表单和应用程序，而 W3C 专注于 XHTML 2.0。在 2006 年，双方决定进行合作，来创建一个新版本的 HTML。
>
> HTML5 中的一些有趣的新特性：

1. 用于绘画的canvas标签
2. 用于媒体回放的video和audio标签
3. 对本地离线储存的更好支持
4. 新的特殊内容元素
   - 如：`article`、`footer`、`header`、`nav`、`section`
5. 新的表单控件
   - 如：`calendar`、`date`、`time`、`email`、`url`、`search`
6. 浏览器的支持
   - Safari、Chrome、FireFox以及Opera包括IE9基本支持了HTML5

#### 2.1.2 HTML5集成开发环境

​	使用 Intellij IDEA 进行开发：www.jetbrains.com

#### 2.1.3 HTML基础讲解

1. 声明：`<!DOCTYPE html>`

   1. `<!DOCTYPE html> ` 用途：HTML 有很多版本，明白页面使用的确切 HTML 版本，浏览器才能正确显示

2. HTML 基础标签：

   1. `head`: 

      ```HTML
      <head>
          <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">
          <title>HTML基础</title>
        </head>
      ```

   2. `body`: 放其它标签内容

   3. `<h1>...<h6>`： 标题

   4. `<p>`： 段落

   5. `<a href=" ">`：超链接

   6. `<img src=" " alt=" ">`：图像

### 2.2 HTML5元素、属性和格式化

#### 2.2.1 HTML 元素

1. 元素：开始标签到结束标签的所有代码

   | 开始标签       | 元素内容            | 结束标签 |
   | -------------- | ------------------- | -------- |
   | `<p>`          | this is my web page | `</P>`   |
   | `<br/>` 空元素 |                     |          |

2. HTML 元素语法：

   - 元素内容是在开始标签与结束标签之间的内容
   - 空元素在开始标签中进行关闭
   - 大多数HTML元素可拥有属性

3. 嵌套的HTML元素

   - 大多数HTML元素可以嵌套使用

#### 2.2.2 HTML 属性

1. 标签可以拥有属性为元素提供更多的信息
2. 属性以键值对的形式出现
   - 如：`href="www.xxx.com"`
3. 常用标签属性：
   - `<h1>`: `align` 对齐方式
   - `<body>`: `bgcolor` 背景颜色，`background` 是设置背景图片
   - `<a>`: `target` 规定在何处打开链接，新窗口：`_blank` 默认：`_self`
4. 通用属性：
   - `class`：规定元素的类名
   - `id`：规定元素的唯一 ID
   - `style`：规定元素的样式
   - `title`：规定元素的额外信息

#### 2.2.3 HTML 格式化

- | 标签       | 描述     |
  | ---------- | -------- |
  | `<b>`      | 粗体文本 |
  | `<big>`    | 大号字   |
  | `<em>`     | 着重文字 |
  | `<i>`      | 斜体字   |
  | `<small>`  | 小号字   |
  | `<strong>` | 加重语气 |
  | `<sub>`    | 下标字   |
  | `<sup>`    | 上标字   |
  | `<ins>`    | 插入字   |
  | `<del>`    | 删除字   |

  

### 2.3 HTML5样式、链接和表格

#### 2.3.1 HTML5 样式

1. 标签：

   - `<style>`: 样式定义
   - `<link>`: 资源引用

2. 属性：

   - `rel="stylesheet"` : 外部样式表
   - `type="text/css"` : 引入文档的类型
   - `margin-left` : 边距

3. 三种样式插入方式：

   1. 外部样式表：`<link rel="stylesheet" href="style.css">`

      ```css
      /* style.css */
      h1 {color: red}
      ```

      

   2. 内部样式表：

      ```HTML
      <head>
        <style>
          body {background-color:burlywood;}
        </style>
      </head>
      ```

      

   3. 内联样式表：`<p style="background-color: cornsilk;">asf</p>`

#### 2.3.2 HTML5 链接

1.  链接数据：
   - 文本链接
   - 图片链接
2. 属性：
   - `href`：指向另一个文档
   - `name`：创建文档内的链接，实现文档内跳转
     - `<a href="tips">点击跳转</a>`
     -  `<a name="tips">跳转位置</a>`
3. `img` 标签属性：
   - `alt` ：替换文本属性( 图像不显示时 )
   - `width`：宽
   - `height`：高

#### 2.3.3 HTML5 表格

1. HTML 表格

   | 标签         | 描述                 |
   | :----------- | :------------------- |
   | `<table>`    | 定义表格             |
   | `<caption>`  | 定义表格标题         |
   | `<th>`       | 定义表格的表头       |
   | `<tr>`       | 定义表格的行         |
   | `<td>`       | 定义表格单元         |
   | `<colgroup>` | 定义表格列的组       |
   | `<col>`      | 定义用于表格列的属性 |
   | `<theah>`    | 定义表格的页眉       |
   | `<tbody>`    | 定义表格的主体       |
   | `<tfoot>`    | 定义表格的页脚       |

2. 属性：

   - `border` 边框
   - `colspan` 单元格跨列

   - `cellpadding` 单元格内边距
   - `cellspacing` 单元格间距

3. > 实例：
   >
   > [没有边框的表格](https://www.runoob.com/try/try.php?filename=tryhtml_tables3)
   > 本例演示一个没有边框的表格。
   >
   > [表格中的表头(Heading)](https://www.runoob.com/try/try.php?filename=tryhtml_table_headers)
   > 本例演示如何显示表格表头。
   >
   > [带有标题的表格](https://www.runoob.com/try/try.php?filename=tryhtml_tables2)
   > 本例演示一个带标题 (caption) 的表格
   >
   > [跨行或跨列的表格单元格](https://www.runoob.com/try/try.php?filename=tryhtml_table_span)
   > 本例演示如何定义跨行或跨列的表格单元格。
   >
   > [表格内的标签](https://www.runoob.com/try/try.php?filename=tryhtml_table_elements)
   > 本例演示如何显示在不同的元素内显示元素。
   >
   > [单元格边距(Cell padding)](https://www.runoob.com/try/try.php?filename=tryhtml_table_cellpadding)
   > 本例演示如何使用 Cell padding 来创建单元格内容与其边框之间的空白。
   >
   > [单元格间距(Cell spacing)](https://www.runoob.com/try/try.php?filename=tryhtml_table_cellspacing)
   > 本例演示如何使用 Cell spacing 增加单元格之间的距离。
   >
   > [漂亮的表格](https://c.runoob.com/codedemo/3187)

### 2.4 HTML5列表、块和布局-块

#### 2.4.1 HTML 列表

| 标签   | 描述             |
| :----- | :--------------- |
| `<ol>` | 有序列表         |
| `<ul>` | 无序列表         |
| `<li>` | 列表项           |
| `<dl>` | 列表             |
| `<dt>` | 自定义列表项目   |
| `<dd>` | 自定列表项的描述 |

1. 无序列表
   - 使用标签：`<ul>`  `<li>`
   - 属性 `type= "disc(实心) \ circle(空心) \ square(方块)"`
2. 有序列表
   - 使用标签：`<ol>`  `<li>`
   - 属性`type= "A(大写字母) \ a(小写字母) \ l \ i "` 默认数字
   - 属性`start="10"` 从10开始
3. 嵌套列表
   - 使用标签：`<ul>`  `<ol>`  `<li>`
4. 自定义列表
   - 使用标签：`<dl>`  `<dt>`  `<dd>`

#### 2.4.2 HTML 块元素

1. 块元素：
   - 块元素显示时，通常会以新行开始
   - 如：`<h1>`、 `<p>`、`<ul>`
2. 内联元素：
   - 内联元素通常不会以新行开始
   - 如：`<b>`、`<a>`、`<img>`
3. `<div>` 元素：
   - `<div>` 元素也被称为块元素，是组合 HTML 的主要容器
4. `<span>` 元素：
   - `<span>`是内联元素，可作为文本的容器

#### 2.4.3 HTML 布局-块

1. 使用 `<div>` 元素布局
2. 使用 `<table>` 元素布局

### 2.5 HTML5表单提交和PHP环境搭建

#### 2.5.1 HTML 表单

1. 表单常用于获取不同类型的用户输入

2. 常用表单标签：

   | 标签         | 描述                                         |
   | :----------- | :------------------------------------------- |
   | `<form>`     | 定义供用户输入的表单                         |
   | `<input>`    | 定义输入域                                   |
   | `<textarea>` | 定义文本域 (一个多行的输入控件)              |
   | `<label>`    | 定义了 `<input>` 元素的标签，一般为输入标题  |
   | `<fieldset>` | 定义了一组相关的表单元素，并使用外框包含起来 |
   | `<legend>`   | 定义了 `<fieldset>` 元素的标题               |
   | `<select>`   | 定义了下拉选项列表                           |
   | `<optgroup>` | 定义选项组                                   |
   | `<option>`   | 定义下拉列表中的选项                         |
   | `<button>`   | 定义一个点击按钮                             |

3. `input` 的常用属性：

   - `text`（文本） `password`（密码） `radio`（单选 指定相同 `name` 实现） 
   - `checkbox`（复选） `submit`（提交） `reset`（重置）

4. `label`：当用户选择该标签时，浏览器就会自动将焦点转到和标签相关的表单控件上。

2.5.2 PHP 环境搭建（跳过）

- 使用 `node.js`

2.5.3 表单与 PHP 交互（跳过）

- 使用 `node.js` 进行交互

### 2.6 HTML5框架、背景和实体

#### 2.6.1 HTML  框架

1. 框架标签 `frame` ：框架对于页面的实际有着很大的作用

2. 框架集标签 `<framest>`：已过时

   - 框架集标签定义如何将窗口分割为框架
   - 每一个 `frameset` 定义一系列行或列
   - `rows/cols` 的值规定了每行或列占据屏幕的面积

3. 常用标签：

   - `noresize`：固定框架大小
   - `cols`：行
   - `rows`：列

4. 内联框架 `iframe`：仍在使用

   ```HTML
   <iframe src="2.6.1.框架b.html" frameborder="0" width="800px" height="800px" style="background-color: darkgray;"></iframe>
   <-- a 标签 target 的使用：_parent _top-->
   <a href="http://www.baidu.com" target="_self" style="color: rgb(0, 0, 0);">_self</a>
     <a href="http://www.baidu.com" target="_blank" style="color: rgb(0, 0, 0);">_blank</a>
     <a href="http://www.baidu.com" target="_parent" style="color: rgb(0, 0, 0);">_parent</a>
     <a href="http://www.baidu.com" target="_top" style="color: rgb(0, 0, 0);">_top</a>
   ```

#### 2.6.2 HTML 背景

1. 背景标签：`background` 图片、颜色等
2. 颜色：十六进制或RGB值表示

#### 2.6.3 HTML 实体

1. 实体：HTML 中预留字符串必须被替换成字符实体（转义）
   - 如：`< > &`

2.7 XHTML的使用规范（跳过）

### 2.7 HTML 速查列表

```HTML
HTML 基本文档
<!DOCTYPE html>
<html>
<head>
<title>文档标题</title>
</head>
<body>
可见文本...
</body>
</html>
基本标签（Basic Tags）
<h1>最大的标题</h1>
<h2> . . . </h2>
<h3> . . . </h3>
<h4> . . . </h4>
<h5> . . . </h5>
<h6>最小的标题</h6>
 
<p>这是一个段落。</p>
<br> （换行）
<hr> （水平线）
<!-- 这是注释 -->
文本格式化（Formatting）
<b>粗体文本</b>
<code>计算机代码</code>
<em>强调文本</em>
<i>斜体文本</i>
<kbd>键盘输入</kbd> 
<pre>预格式化文本</pre>
<small>更小的文本</small>
<strong>重要的文本</strong>
 
<abbr> （缩写）
<address> （联系信息）
<bdo> （文字方向）
<blockquote> （从另一个源引用的部分）
<cite> （工作的名称）
<del> （删除的文本）
<ins> （插入的文本）
<sub> （下标文本）
<sup> （上标文本）
链接（Links）
普通的链接：<a href="http://www.example.com/">链接文本</a>
图像链接： <a href="http://www.example.com/"><img src="URL" alt="替换文本"></a>
邮件链接： <a href="mailto:webmaster@example.com">发送e-mail</a>
书签：
<a id="tips">提示部分</a>
<a href="#tips">跳到提示部分</a>
图片（Images）
<img src="URL" alt="替换文本" height="42" width="42">
样式/区块（Styles/Sections）
<style type="text/css">
h1 {color:red;}
p {color:blue;}
</style>
<div>文档中的块级元素</div>
<span>文档中的内联元素</span>
无序列表
<ul>
    <li>项目</li>
    <li>项目</li>
</ul>
有序列表
<ol>
    <li>第一项</li>
    <li>第二项</li>
</ol>
定义列表
<dl>
  <dt>项目 1</dt>
    <dd>描述项目 1</dd>
  <dt>项目 2</dt>
    <dd>描述项目 2</dd>
</dl>
表格（Tables）
<table border="1">
  <tr>
    <th>表格标题</th>
    <th>表格标题</th>
  </tr>
  <tr>
    <td>表格数据</td>
    <td>表格数据</td>
  </tr>
</table>
框架（Iframe）
<iframe src="demo_iframe.htm"></iframe>
表单（Forms）
<form action="demo_form.php" method="post/get">
<input type="text" name="email" size="40" maxlength="50">
<input type="password">
<input type="checkbox" checked="checked">
<input type="radio" checked="checked">
<input type="submit" value="Send">
<input type="reset">
<input type="hidden">
<select>
<option>苹果</option>
<option selected="selected">香蕉</option>
<option>樱桃</option>
</select>
<textarea name="comment" rows="60" cols="20"></textarea>
 
</form>
实体（Entities）
&lt; 等同于 <
&gt; 等同于 >
&#169; 等同于 ©
```



## 3. CSS3 基础

### 3.1 CSS入门基础知识

#### 3.1.1 CSS 背景

1. 背景：

   - CSS 允许纯色背景，也允许复杂图像背景

   | Property                                                     | 描述                                         |
   | :----------------------------------------------------------- | :------------------------------------------- |
   | [background](https://www.runoob.com/cssref/css3-pr-background.html) | 简写属性，作用是将背景属性设置在一个声明中。 |
   | [background-attachment](https://www.runoob.com/cssref/pr-background-attachment.html) | 背景图像是否固定或者随着页面的其余部分滚动。 |
   | [background-color](https://www.runoob.com/cssref/pr-background-color.html) | 设置元素的背景颜色。                         |
   | [background-image](https://www.runoob.com/cssref/pr-background-image.html) | 把图像设置为背景。                           |
   | [background-position](https://www.runoob.com/cssref/pr-background-position.html) | 设置背景图像的起始位置。                     |
   | [background-repeat](https://www.runoob.com/cssref/pr-background-repeat.html) | 设置背景图像是否及如何重复。                 |

#### 3.1.1 CSS 文本

1. CSS 文本属性

   | 属性                                                         | 描述                     |
   | :----------------------------------------------------------- | :----------------------- |
   | [color](https://www.runoob.com/cssref/pr-text-color.html)    | 设置文本颜色             |
   | [direction](https://www.runoob.com/cssref/pr-text-direction.html) | 设置文本方向。           |
   | [letter-spacing](https://www.runoob.com/cssref/pr-text-letter-spacing.html) | 设置字符间距             |
   | [line-height](https://www.runoob.com/cssref/pr-dim-line-height.html) | 设置行高                 |
   | [text-align](https://www.runoob.com/cssref/pr-text-text-align.html) | 对齐元素中的文本         |
   | [text-decoration](https://www.runoob.com/cssref/pr-text-text-decoration.html) | 向文本添加修饰           |
   | [text-indent](https://www.runoob.com/cssref/pr-text-text-indent.html) | 缩进元素中文本的首行     |
   | [text-shadow](https://www.runoob.com/cssref/css3-pr-text-shadow.html) | 设置文本阴影             |
   | [text-transform](https://www.runoob.com/cssref/pr-text-text-transform.html) | 控制元素中的字母         |
   | [unicode-bidi](https://www.runoob.com/cssref/pr-text-unicode-bidi.html) | 设置或返回文本是否被重写 |
   | [vertical-align](https://www.runoob.com/cssref/pr-pos-vertical-align.html) | 设置元素的垂直对齐       |
   | [white-space](https://www.runoob.com/cssref/pr-text-white-space.html) | 设置元素中空白的处理方式 |
   | [word-spacing](https://www.runoob.com/cssref/pr-text-word-spacing.html) | 设置字间距               |

2. text-align 属性

   | 值      | 描述                                       |
   | :------ | :----------------------------------------- |
   | left    | 把文本排列到左边。默认值：由浏览器决定。   |
   | right   | 把文本排列到右边。                         |
   | center  | 把文本排列到中间。                         |
   | justify | 实现两端对齐文本效果。                     |
   | inherit | 规定应该从父元素继承 text-align 属性的值。 |

3. text-transform 属性：

   | 值         | 描述                                           |
   | :--------- | :--------------------------------------------- |
   | none       | 默认。定义带有小写字母和大写字母的标准的文本。 |
   | capitalize | 文本中的每个单词以大写字母开头。               |
   | uppercase  | 定义仅有大写字母。                             |
   | lowercase  | 定义无大写字母，仅有小写字母。                 |
   | inherit    | 规定应该从父元素继承 text-transform 属性的值。 |

4. CSS3 文本效果：

   - text-shadow：向文本添加阴影 `text-shadow: *h-shadow v-shadow blur color*;`
   - word-wrap：规定文本的换行规则 `word-wrap: normal|break-word;`

#### 3.1.1 CSS 字体

1. 在CSS中，有两种类型的字体系列名称：

   - **通用字体系列** - 拥有相似外观的字体系统组合（如 "Serif" 或 "Monospace"）
   - **特定字体系列** - 一个特定的字体系列（如 "Times" 或 "Courier"）

   | Generic family | 字体系列                   | 说明                                        |
   | :------------- | :------------------------- | :------------------------------------------ |
   | Serif          | Times New Roman Georgia    | Serif字体中字符在行的末端拥有额外的装饰     |
   | Sans-serif     | Arial Verdana              | "Sans"是指无 - 这些字体在末端没有额外的装饰 |
   | Monospace      | Courier New Lucida Console | 所有的等宽字符具有相同的宽度                |

2. 字体

   | Property                                                     | 描述                                 |
   | :----------------------------------------------------------- | :----------------------------------- |
   | [font](https://www.runoob.com/cssref/pr-font-font.html)      | 在一个声明中设置所有的字体属性       |
   | [font-family](https://www.runoob.com/cssref/pr-font-font-family.html) | 指定文本的字体系列                   |
   | [font-size](https://www.runoob.com/cssref/pr-font-font-size.html) | 指定文本的字体大小                   |
   | [font-style](https://www.runoob.com/cssref/pr-font-font-style.html) | 指定文本的字体样式                   |
   | [font-variant](https://www.runoob.com/cssref/pr-font-font-variant.html) | 以小型大写字体或者正常字体显示文本。 |
   | [font-weight](https://www.runoob.com/cssref/pr-font-weight.html) | 指定字体的粗细。                     |

3. CSS3 ：@font-face { src: url() } 引入字体

#### 3.1.1 CSS 链接

1. 链接的样式，可以用任何CSS属性（如颜色，字体，背景等）。

   特别的链接，可以有不同的样式，这取决于他们是什么状态。

   这四个链接状态是：

   - a:link - 正常，未访问过的链接
   - a:visited - 用户已访问过的链接
   - a:hover - 当用户鼠标放在链接上时
   - a:active - 链接被点击的那一刻

2. 当设置为若干链路状态的样式，也有一些顺序规则：

   - a:hover 必须跟在 a:link 和 a:visited后面
   - a:active 必须跟在 a:hover后面

3. text-decoration 属性去掉下划线

4. background-color

#### 3.1.1 CSS 列表

1. 列表：可放置和改变标志，或使用图片作为列表项标志

   | 属性                                                         | 描述                                               |
   | :----------------------------------------------------------- | :------------------------------------------------- |
   | [list-style](https://www.runoob.com/cssref/pr-list-style.html) | 简写属性。用于把所有用于列表的属性设置于一个声明中 |
   | [list-style-image](https://www.runoob.com/cssref/pr-list-style-image.html) | 将图象设置为列表项标志。                           |
   | [list-style-position](https://www.runoob.com/cssref/pr-list-style-position.html) | 设置列表中列表项标志的位置。                       |
   | [list-style-type](https://www.runoob.com/cssref/pr-list-style-type.html) | 设置列表项标志的类型。                             |

#### 3.1.1 CSS 表格

1. CSS 表格：改善表格外观
2. 表格边框：指定CSS表格边框，使用border属性。
3. 折叠边框：border-collapse 属性设置表格的边框是否被折叠成一个单一的边框或隔开
4. 表格宽高：Width和height属性定义表格的宽度和高度。
5. 表格文本对齐：text-align属性设置水平对齐方式，向左，右，或中心
6. 表格内边距：如果在表的内容中控制空格之间的边框，应使用td和th元素的填充属性padding
7. 表格颜色： background-color

#### 3.1.1 CSS 轮廓

1. 轮廓（outline）是绘制于元素周围的一条线，位于边框边缘的外围，可起到突出元素的作用。

   轮廓（outline）属性指定元素轮廓的样式、颜色和宽度。

2. 所有属性：

   | 属性                                                         | 说明                           | 值                                                           | CSS  |
   | :----------------------------------------------------------- | :----------------------------- | :----------------------------------------------------------- | :--- |
   | [outline](https://www.runoob.com/cssref/pr-outline.html)     | 在一个声明中设置所有的轮廓属性 | *outline-color outline-style outline-width *inherit          | 2    |
   | [outline-color](https://www.runoob.com/cssref/pr-outline-color.html) | 设置轮廓的颜色                 | *color-name hex-number rgb-number *invert inherit            | 2    |
   | [outline-style](https://www.runoob.com/cssref/pr-outline-style.html) | 设置轮廓的样式                 | none dotted dashed solid double groove ridge inset outset inherit | 2    |
   | [outline-width](https://www.runoob.com/cssref/pr-outline-width.html) | 设置轮廓的宽度                 | thin medium thick *length *inherit                           | 2    |

### 3.2 CSS基本样式讲解

#### 3.2.1 CSS 介绍

1. CSS 概述：
   - CSS 指层叠样式表
   - CSS 样式表极大的提高了工作效率

#### 3.2.2 CSS 基础语法

1. `'selector' { 'property': 'value'}`
   - 例：`h1 {color: red; font-size: 14px;}`
   - 属性如果大于一个，属性之间用分号隔开；
   - 如果值大于一个，则要加上引号：
     - 例：`p { font-family: "sans serif" }`

#### 3.2.3 CSS 高级语法

1. 选择器分组：

   `h1, h2, h3, h4, h5, h6 { color: red}`

2. 继承：` body { color: green} `

   - 子元素会继承父元素的样式

#### 3.2.1 CSS 派生选择器

1. 根据元素在其位置的父子关系来定义样式

#### 3.2.1 CSS id选择器

1. id 选择器：
   - id 选择器可以为标有唯一 id 的HTML元素指定样式
   - id 选择器以 # 来定义
2. id 选择器和派生选择器：
   - 目前常用 id 选择器建立派生选择器
   - 例：` #id li { color: blue} `

#### 3.2.1 CSS 类选择器

1. 类选择器（class）：类选择器以 `.` 显示
2. `class` 也可以用作派生选择器

#### 3.2.1 CSS 属性选择器

1. 属性选择器：对带有指定属性的HTML元素设置样式

   - 例：

     ```
     下面的例子是把包含标题（title）的所有元素变为蓝色：
     [title]
     {
         color:blue;
     }
     ```

2. 属性和值选择器

   - 例：

     ```css
     [title=runoob]
     {
         border:5px solid green;
     }
     /* 属性和值的选择器 - 多值 */
     [title~=hello] { color:blue; }
     ```

     > ## CSS 属性选择器 *=, |=, ^=, $=, ~= 的区别
     >
     > **先上总结:**
     >
     > **"value 是完整单词"** 类型的比较符号: **~=**, **|=**
     >
     > **"拼接字符串**" 类型的比较符号: ***=**, **^=**, **$=**
     >
     > 
     >
     > **1.attribute 属性中包含 value:**　
     >
     > [attribute~=value] 属性中包含独立的单词为 value，例如：
     >
     > ```
     > [title~=flower]  -->  <img src="/i/eg_tulip.jpg" title="tulip flower" />
     > ```
     >
     > [attribute*=value] 属性中做字符串拆分，只要能拆出来 value 这个词就行，例如：
     >
     > ```
     > [title*=flower]   -->  <img src="/i/eg_tulip.jpg" title="ffffflowerrrrrr" />
     > ```
     >
     > **2.attribute 属性以 value 开头:**
     >
     > [attribute|=value] 属性中必须是完整且唯一的单词，或者以 **-** 分隔开：，例如：
     >
     > ```
     > [lang|=en]     -->  <p lang="en">  <p lang="en-us">
     > ```
     >
     > [
     >
     > attribute^=value] 属性的前几个字母是 value 就可以，例如：
     >
     > ```
     > [lang^=en]    -->  <p lang="ennn">
     > ```
     >
     > **3.attribute 属性以 value 结尾:**
     >
     > ```
     > [attribute$=value] 属性的后几个字母是 value 就可以，例如：
     > a[src$=".pdf"]
     > ```

### 3.3 CSS盒子模型

#### 3.3.1 CSS 盒子模型概述

1. 盒子模型的内容范围包括：
   - margin、border、padding、content 部分组成

#### 3.3.2 CSS 内边距

1. 内边距：padding: 上 右 下 左

   ## padding（填充）

   当元素的 padding（填充）内边距被清除时，所释放的区域将会受到元素背景颜色的填充。

   单独使用 padding 属性可以改变上下左右的填充。

   ![img](readme.assets/VlwVi.png)

   | 属性                                                         | 说明                                       |
   | :----------------------------------------------------------- | :----------------------------------------- |
   | [padding](https://www.runoob.com/cssref/pr-padding.html)     | 使用简写属性设置在一个声明中的所有填充属性 |
   | [padding-bottom](https://www.runoob.com/cssref/pr-padding-bottom.html) | 设置元素的底部填充                         |
   | [padding-left](https://www.runoob.com/cssref/pr-padding-left.html) | 设置元素的左部填充                         |
   | [padding-right](https://www.runoob.com/cssref/pr-padding-right.html) | 设置元素的右部填充                         |
   | [padding-top](https://www.runoob.com/cssref/pr-padding-top.html) | 设置元素的顶部填充                         |

#### 3.3.3 CSS 边框

1. 边框的样式：border-style

   - none: 默认无边框

     dotted: 定义一个点线边框

     dashed: 定义一个虚线边框

     solid: 定义实线边框

     double: 定义两个边框。 两个边框的宽度和 border-width 的值相同

     groove: 定义3D沟槽边框。效果取决于边框的颜色值

     ridge: 定义3D脊边框。效果取决于边框的颜色值

     inset:定义一个3D的嵌入边框。效果取决于边框的颜色值

     outset: 定义一个3D突出边框。 效果取决于边框的颜色值

   - border-style属性可以有1-4个值：

     - border-style:dotted solid double dashed;
       - 上边框是 dotted
       - 右边框是 solid
       - 底边框是 double
       - 左边框是 dashed
     - border-style:dotted solid double;
       - 上边框是 dotted
       - 左、右边框是 solid
       - 底边框是 double
     - border-style:dotted solid;
       - 上、底边框是 dotted
       - 右、左边框是 solid
     - border-style:dotted;
       - 四面边框是 dotted

     上面的例子用了border-style。然而，它也可以和border-width 、 border-color一起使用

   - > border-style：属性1，属性2，属性3，属性4
     >
     > 上->右->下->左
     >
     > border-style：属性1，属性2，属性3
     >
     > 上->左右->下
     >
     > border-style：属性1，属性2
     >
     > 上下->左右
     >
     > border-style：属性1
     >
     > 上下左右属性相同

   | 属性                                                         | 描述                                                         |
   | :----------------------------------------------------------- | :----------------------------------------------------------- |
   | [border](https://www.runoob.com/cssref/pr-border.html)       | 简写属性，用于把针对四个边的属性设置在一个声明。             |
   | [border-style](https://www.runoob.com/cssref/pr-border-style.html) | 用于设置元素所有边框的样式，或者单独地为各边设置边框样式。   |
   | [border-width](https://www.runoob.com/cssref/pr-border-width.html) | 简写属性，用于为元素的所有边框设置宽度，或者单独地为各边边框设置宽度。 |
   | [border-color](https://www.runoob.com/cssref/pr-border-color.html) | 简写属性，设置元素的所有边框中可见部分的颜色，或为 4 个边分别设置颜色。 |
   | [border-bottom](https://www.runoob.com/cssref/pr-border-bottom.html) | 简写属性，用于把下边框的所有属性设置到一个声明中。           |
   | [border-bottom-color](https://www.runoob.com/cssref/pr-border-bottom-color.html) | 设置元素的下边框的颜色。                                     |
   | [border-bottom-style](https://www.runoob.com/cssref/pr-border-bottom-style.html) | 设置元素的下边框的样式。                                     |
   | [border-bottom-width](https://www.runoob.com/cssref/pr-border-bottom-width.html) | 设置元素的下边框的宽度。                                     |
   | [border-left](https://www.runoob.com/cssref/pr-border-left.html) | 简写属性，用于把左边框的所有属性设置到一个声明中。           |
   | [border-left-color](https://www.runoob.com/cssref/pr-border-left-color.html) | 设置元素的左边框的颜色。                                     |
   | [border-left-style](https://www.runoob.com/cssref/pr-border-left-style.html) | 设置元素的左边框的样式。                                     |
   | [border-left-width](https://www.runoob.com/cssref/pr-border-left-width.html) | 设置元素的左边框的宽度。                                     |
   | [border-right](https://www.runoob.com/cssref/pr-border-right.html) | 简写属性，用于把右边框的所有属性设置到一个声明中。           |
   | [border-right-color](https://www.runoob.com/cssref/pr-border-right-color.html) | 设置元素的右边框的颜色。                                     |
   | [border-right-style](https://www.runoob.com/cssref/pr-border-right-style.html) | 设置元素的右边框的样式。                                     |
   | [border-right-width](https://www.runoob.com/cssref/pr-border-right-width.html) | 设置元素的右边框的宽度。                                     |
   | [border-top](https://www.runoob.com/cssref/pr-border-top.html) | 简写属性，用于把上边框的所有属性设置到一个声明中。           |
   | [border-top-color](https://www.runoob.com/cssref/pr-border-top-color.html) | 设置元素的上边框的颜色。                                     |
   | [border-top-style](https://www.runoob.com/cssref/pr-border-top-style.html) | 设置元素的上边框的样式。                                     |
   | [border-top-width](https://www.runoob.com/cssref/pr-border-top-width.html) | 设置元素的上边框的宽度。                                     |

2. CSS3 边框：

   - border-radius：圆角边框
   - box-shadow：边框阴影
   - border-image：边框图片
     - border-radius:10px;width: 50px;border: solid 2px yellow;

#### 3.3.4 CSS 外边距

1. 围绕在内容边框的区域，默认透明，接收任意长度单位

2. margin属性可以有一到四个值。

   - margin:25px 50px 75px 100px;
     - 上边距为25px
     - 右边距为50px
     - 下边距为75px
     - 左边距为100px
   - margin:25px 50px 75px;
     - 上边距为25px
     - 左右边距为50px
     - 下边距为75px
   - margin:25px 50px;
     - 上下边距为25px
     - 左右边距为50px
   - margin:25px;
     - 所有的4个边距都是25px

   | 属性                                                         | 描述                                       |
   | :----------------------------------------------------------- | :----------------------------------------- |
   | [margin](https://www.runoob.com/cssref/pr-margin.html)       | 简写属性。在一个声明中设置所有外边距属性。 |
   | [margin-bottom](https://www.runoob.com/cssref/pr-margin-bottom.html) | 设置元素的下外边距。                       |
   | [margin-left](https://www.runoob.com/cssref/pr-margin-left.html) | 设置元素的左外边距。                       |
   | [margin-right](https://www.runoob.com/cssref/pr-margin-right.html) | 设置元素的右外边距。                       |
   | [margin-top](https://www.runoob.com/cssref/pr-margin-top.html) | 设置元素的上外边距。                       |

#### 3.3.5 CSS 外边距合并

1. 外边距合并：是一个边距叠加的概念
2. **相交 margin 值会合并：以大的值为准**

#### 3.3.6 CSS 盒子模型应用

1. 极客学院官网

###  3.4 CSS定位

#### 3.4.1 定位

1. CSS 定位：改变元素在页面上的位置

2. CSS 定位机制：

   - 普通流(static)：元素按照其在HTML中的位置顺序决定排布过程
   - 浮动(relative/absolute)
   - 绝对布局(fixed)

3. position 属性的五个值：

   - static : 偏移无效，z-index 无效
   - relative ：相对偏移，保留位置，z-index 有效
   - fixed ：固定定位，固定在可视区位置
   - absolute ：绝对定位，不保留位置脱离文档流，相对于父元素或文档定位，z-index 有效
   - sticky

4. "CSS" 列中的数字表示哪个CSS(CSS1 或者CSS2)版本定义了该属性。

   | 属性                                                         | 说明                                                         | 值                                                           | CSS  |
   | :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- | :--- |
   | [bottom](https://www.runoob.com/cssref/pr-pos-bottom.html)   | 定义了定位元素下外边距边界与其包含块下边界之间的偏移。       | auto *length % *inherit                                      | 2    |
   | [clip](https://www.runoob.com/cssref/pr-pos-clip.html)       | 剪辑一个绝对定位的元素                                       | *shape *auto inherit                                         | 2    |
   | [cursor](https://www.runoob.com/cssref/pr-class-cursor.html) | 显示光标移动到指定的类型                                     | *url* auto crosshair default pointer move e-resize ne-resize nw-resize n-resize se-resize sw-resize s-resize w-resize text wait help | 2    |
   | [left](https://www.runoob.com/cssref/pr-pos-left.html)       | 定义了定位元素左外边距边界与其包含块左边界之间的偏移。       | auto *length % *inherit                                      | 2    |
   | [overflow](https://www.runoob.com/cssref/pr-pos-overflow.html) | 设置当元素的内容溢出其区域时发生的事情。                     | auto hidden scroll visible inherit                           | 2    |
   | [overflow-y](https://www.runoob.com/css/cssref/css3-pr-overflow-y.html) | 指定如何处理顶部/底部边缘的内容溢出元素的内容区域            | auto hidden scroll visible no-display no-content             | 2    |
   | [overflow-x](https://www.runoob.com/css/cssref//cssref/css3-pr-overflow-x.html) | 指定如何处理右边/左边边缘的内容溢出元素的内容区域            | auto hidden scroll visible no-display no-content             | 2    |
   | [position](https://www.runoob.com/cssref/pr-class-position.html) | 指定元素的定位类型                                           | absolute fixed relative static inherit                       | 2    |
   | [right](https://www.runoob.com/cssref/pr-pos-right.html)     | 定义了定位元素右外边距边界与其包含块右边界之间的偏移。       | auto *length % *inherit                                      | 2    |
   | [top](https://www.runoob.com/cssref/pr-pos-top.html)         | 定义了一个定位元素的上外边距边界与其包含块上边界之间的偏移。 | auto *length % *inherit                                      | 2    |
   | [z-index](https://www.runoob.com/cssref/pr-pos-z-index.html) | 设置元素的堆叠顺序                                           | *number *auto inherit                                        | 2    |

#### 3.4.2 浮动

1. 浮动：同级文档流浮动，在父容器内，占有位置

   - float 属性可用的值
     - left：元素向左浮动
     - right：元素向右浮动
     - none：不浮动
     - inherit：从父元素继承

2. clear 属性：

   - 清楚浮动属性（包括继承的浮动）
   - `.text_line { clear:both; }`

   | 属性                                                       | 描述                               | 值                           | CSS  |
   | :--------------------------------------------------------- | :--------------------------------- | :--------------------------- | :--- |
   | [clear](https://www.runoob.com/cssref/pr-class-clear.html) | 指定不允许元素周围有浮动元素。     | left right both none inherit | 1    |
   | [float](https://www.runoob.com/cssref/pr-class-float.html) | 指定一个盒子（元素）是否可以浮动。 | left right none inherit      | 1    |

###  3.5 CSS选择器

#### 3.5.1 元素选择器

1. 最常见、最基本的选择器
   - 例：`h1 {}`

#### 3.5.2 选择器分组

1. 标签之间使用`,`分隔， `h1,h2,h3,a,p { color: red}`
2. 通配符：`* {}`

#### 3.5.3 类选择器详解

1. 类选择器允许以一种独立于文档元素的方式来指定样式
   - `.class {}`
2. 结合元素选择器
   - `a.class {}`
3. 多类选择器
   - `.class1 {}`
   - ` .class2 .class3 {}`
   - 拥有`class1~3`所有属性：`<p class="class1 class2 class3"> text </P>`

#### 3.5.4 ID 选择器详解

1. ID 选择器类似于类选择器
   - 例：#id {}
2. ID选择器与类选择器区别：
   1. ID选择器是唯一的，类可以重复多个
   2. 不能多个ID选择器结合使用
   3. 使用 JS 时一般用 ID
   4. ID 选择器先找到结构再找到内容再渲染，类选择器先渲染再找结构再找内容

#### 3.5.5 属性选择器详解

1.  3.2.1章节已详细说明

2. 多值选择器：

   ```css
   [title=runoob]
   {
       border:5px solid green;
   }
   /* 属性和值的选择器 - 多值 */
   [title~=hello] { color:blue; }
   ```

#### 3.5.6 后代选择器

1. 后代选择器：
   - 可以选择某元素后代的元素，可以跨子代
   - 例：`p strong { color: blue}`

#### 3.5.7 子元素选择器

1. 只能选择某元素的子元素
   - 例：`h1>strong { color: blue}`

#### 3.5.8 相邻兄弟选择器

1. 选择同一个父元素下的后一个相邻元素
   - 例：`h1+p{ color:bllue}`

### 3.6 CSS常用操作

#### 3.6.1 对齐操作

1. 水平对齐 `margin` 

   - 水平居中对齐一个元素(如 `<div>`), 可以使用 `margin: auto`
     - **注意:** 如果没有设置 **width** 属性(或者设置 100%)，居中对齐将不起作用。

2. 垂直居中对齐 `padding`

   - 水平和垂直都居中，可以使用 `padding` 和 `text-align: center`:

3. 左右对齐 `position` 

   - `position: absolute;` 属性来对齐元素，手动
   - 垂直居中 `transform: translate(-50%, -50%);` 

4. 左右对齐 `float` 

   - 对 `<body>` 元素的外边距和内边距进行预定义，可以避免在不同的浏览器中出现可见的差异。
   - 在父元素上添加 `overflow: auto;` 来解决子元素溢出的问题:

5. 文本对齐 `text-align` 

   - 如果仅仅是为了文本在元素内居中对齐，可以使用 `text-align: center;`

   - 垂直居中 `line-height`

     > 设置容器上下 padding 相同实现垂直居中和使用 line-height=height 实现垂直居中仅对单行文本有效，当文本行数超过单行时：
     >
     > -  1）**padding**：文本仍然处于容器垂直居中的位置，但是容器的 height 会随着文本行数的增加而增大；
     > -  2）**line-height=height**：容器的 height 不变，line-height 是文本的行间距，文本会溢出容器显示；
     >
     > 多行文本可使用 **vertical-align: middle;** 来实现元素的垂直居中，但是如果子元素的内容体积大于父元素的内容体积时，仍然会溢出，后面需要使用文字溢出处理来解决。

#### 3.6.2 尺寸操作

1. 属性

   | 属性                                                         | 描述                 |
   | :----------------------------------------------------------- | :------------------- |
   | [height](https://www.runoob.com/cssref/pr-dim-height.html)   | 设置元素的高度。     |
   | [line-height](https://www.runoob.com/cssref/pr-dim-line-height.html) | 设置行高。           |
   | [max-height](https://www.runoob.com/cssref/pr-dim-max-height.html) | 设置元素的最大高度。 |
   | [max-width](https://www.runoob.com/cssref/pr-dim-max-width.html) | 设置元素的最大宽度。 |
   | [min-height](https://www.runoob.com/cssref/pr-dim-min-height.html) | 设置元素的最小高度。 |
   | [min-width](https://www.runoob.com/cssref/pr-dim-min-width.html) | 设置元素的最小宽度。 |
   | [width](https://www.runoob.com/cssref/pr-dim-width.html)     | 设置元素的宽度。     |

#### 3.6.3 分类操作

1. 属性

   | 属性       | 描述                                   |
   | ---------- | -------------------------------------- |
   | clear      | 设置一个元素的侧面受否允许浮动其它元素 |
   | cursor     | 当前鼠标指向某元素之上时现实的指针类型 |
   | display    | 是否及如何显示元素                     |
   | float      | 元素再哪个方向浮动                     |
   | position   | 元素放置到静态、绝对、相对、固定的位置 |
   | visibility | 设置元素是否可见                       |

#### 3.6.4 导航栏

1. 垂直导航栏
   1. 去掉 `li` 点：`list-style-type:none`
   2. 去掉 `a` 下划线：`text-decoration:none`
   3. `li` 显示在一行：`display: inline`
2. 水平导航栏
3. 导航栏效果

#### 3.6.5 图片操作

1. 使用CSS创建图片廊

   ` <img src="./demo3.jpg" alt="图片文本描述" width="300" height="200">`

2. 图片透明度

   ```css
   img
   {
     opacity:0.4;
     filter:alpha(opacity=40); /*  IE8 及其更早版本 */
   }
   img:hover
   {
     opacity:1.0;
     filter:alpha(opacity=100); /* IE8 及其更早版本 */
   }
   ```

###  3.7 CSS动画—页面特效

#### 3.7.1 2D/3D 转换

1. 通过CSS3转换，我们能够对元素进行移动、缩放、转动、拉长或拉伸

   - 转换：使元素改变形状、尺寸和位置的一种效果
   - 可以使用 2D/3D 来转换元素

2. 2D 转换方法：

   - `translate()`：根据左(X轴)和顶部(Y轴)位置给定的参数，从当前元素位置移动

     - ```CSS
       div
       {
       transform: translate(50px,100px);
       -ms-transform: translate(50px,100px); /* IE 9 */
       -webkit-transform: translate(50px,100px); /* Safari and Chrome */
       }
       ```

   - `rotate()`：在一个给定度数顺时针旋转的元素。负值是允许的，这样是元素逆时针旋转。

     - ```CSS
       div
       {
       transform: rotate(30deg);
       -ms-transform: rotate(30deg); /* IE 9 */
       -webkit-transform: rotate(30deg); /* Safari and Chrome */
       }
       ```

   - `scale()`：该元素增加或减少的大小，取决于宽度（X轴）和高度（Y轴）的参数

     - ```CSS
       -ms-transform:scale(2,3); /* IE 9 */
       -webkit-transform: scale(2,3); /* Safari */
       transform: scale(2,3); /* 标准语法 */
       ```

   - `skew()`：`transform:skew(angle, angle);`

     - ```CSS
       div
       {
       transform: skew(30deg,20deg);
       -ms-transform: skew(30deg,20deg); /* IE 9 */
       -webkit-transform: skew(30deg,20deg); /* Safari and Chrome */
       }
       ```

     > - 包含两个参数值，分别表示X轴和Y轴倾斜的角度，如果第二个参数为空，则默认为0，参数为负表示向相反方向倾斜。
     >   - skewX(angle);表示只在X轴(水平方向)倾斜。
     >   - skewY(angle);表示只在Y轴(垂直方向)倾斜。

   - `matrix()`：

     - ```CSS
     div
       {
       transform:matrix(0.866,0.5,-0.5,0.866,0,0);
       -ms-transform:matrix(0.866,0.5,-0.5,0.866,0,0); /* IE 9 */
       -webkit-transform:matrix(0.866,0.5,-0.5,0.866,0,0); /* Safari and Chrome */
       }
       ```
     
     > - matrix()方法和2D变换方法合并成一个。
     >
     >   matrix 方法有六个参数，包含旋转，缩放，移动（平移）和倾斜功能。

3. 新的转换属性：

   | Property                                                     | 描述                   | CSS  |
   | :----------------------------------------------------------- | :--------------------- | :--- |
   | [transform](https://www.runoob.com/cssref/css3-pr-transform.html) | 适用于2D或3D转换的元素 | 3    |
   | [transform-origin](https://www.runoob.com/cssref/css3-pr-transform-origin.html) | 允许您更改转化元素位置 | 3    |

4. 2D 转换方法：

   | 函数                            | 描述                                     |
   | :------------------------------ | :--------------------------------------- |
   | matrix(*n*,*n*,*n*,*n*,*n*,*n*) | 定义 2D 转换，使用六个值的矩阵。         |
   | translate(*x*,*y*)              | 定义 2D 转换，沿着 X 和 Y 轴移动元素。   |
   | translateX(*n*)                 | 定义 2D 转换，沿着 X 轴移动元素。        |
   | translateY(*n*)                 | 定义 2D 转换，沿着 Y 轴移动元素。        |
   | scale(*x*,*y*)                  | 定义 2D 缩放转换，改变元素的宽度和高度。 |
   | scaleX(*n*)                     | 定义 2D 缩放转换，改变元素的宽度。       |
   | scaleY(*n*)                     | 定义 2D 缩放转换，改变元素的高度。       |
   | rotate(*angle*)                 | 定义 2D 旋转，在参数中规定角度。         |
   | skew(*x-angle*,*y-angle*)       | 定义 2D 倾斜转换，沿着 X 和 Y 轴。       |
   | skewX(*angle*)                  | 定义 2D 倾斜转换，沿着 X 轴。            |
   | skewY(*angle*)                  | 定义 2D 倾斜转换，沿着 Y 轴。            |

5. 3D 转换方法：

   - `rotateX()` ：围绕其在一个给定度数X轴旋转的元素
   - `rotateY()` ：围绕其在一个给定度数Y轴旋转的元素

6. 表格中的数字表示支持该属性的第一个浏览器版本号。

   紧跟在 -webkit-, -ms- 或 -moz- 前的数字为支持该前缀属性的第一个浏览器版本号。

   | 属性                                  | chrome             | IE   | FireFox         | Safari       | Opera              |
   | :------------------------------------ | :----------------- | ---- | --------------- | ------------ | ------------------ |
   | transform                             | 36.0 12.0 -webkit- | 10.0 | 16.0 10.0 -moz- | 4.0 -webkit- | 23.0 15.0 -webkit- |
   | transform-origin (three-value syntax) | 36.0 12.0 -webkit- | 10.0 | 16.0 10.0 -moz- | 4.0 -webkit- | 23.0 15.0 -webkit- |
   | transform-style                       | 36.0 12.0 -webkit- | 11.0 | 16.0 10.0 -moz- | 4.0 -webkit- | 23.0 15.0 -webkit- |
   | perspective                           | 36.0 12.0 -webkit- | 10.0 | 16.0 10.0 -moz- | 4.0 -webkit- | 23.0 15.0 -webkit- |
   | perspective-origin                    | 36.0 12.0 -webkit- | 10.0 | 16.0 10.0 -moz- | 4.0 -webkit- | 23.0 15.0 -webkit- |
   | backface-visibility                   | 36.0 12.0 -webkit- | 10.0 | 16.0 10.0 -moz- | 4.0 -webkit- | 23.0 15.0 -webkit- |

7. 下表列出了所有的转换属性：

   | 属性                                                         | 描述                                 | CSS  |
   | :----------------------------------------------------------- | :----------------------------------- | :--- |
   | [transform](https://www.runoob.com/cssref/css3-pr-transform.html) | 向元素应用 2D 或 3D 转换。           | 3    |
   | [transform-origin](https://www.runoob.com/cssref/css3-pr-transform-origin.html) | 允许你改变被转换元素的位置。         | 3    |
   | [transform-style](https://www.runoob.com/cssref/css3-pr-transform-style.html) | 规定被嵌套元素如何在 3D 空间中显示。 | 3    |
   | [perspective](https://www.runoob.com/cssref/css3-pr-perspective.html) | 规定 3D 元素的透视效果。             | 3    |
   | [perspective-origin](https://www.runoob.com/cssref/css3-pr-perspective-origin.html) | 规定 3D 元素的底部位置。             | 3    |
   | [backface-visibility](https://www.runoob.com/cssref/css3-pr-backface-visibility.html) | 定义元素在不面对屏幕时是否可见。     | 3    |

8. 3D 转换方法：

   | 函数                                                         | 描述                                      |
   | :----------------------------------------------------------- | :---------------------------------------- |
   | matrix3d(*n*,*n*,*n*,*n*,*n*,*n*, *n*,*n*,*n*,*n*,*n*,*n*,*n*,*n*,*n*,*n*) | 定义 3D 转换，使用 16 个值的 4x4 矩阵。   |
   | translate3d(*x*,*y*,*z*)                                     | 定义 3D 转化。                            |
   | translateX(*x*)                                              | 定义 3D 转化，仅使用用于 X 轴的值。       |
   | translateY(*y*)                                              | 定义 3D 转化，仅使用用于 Y 轴的值。       |
   | translateZ(*z*)                                              | 定义 3D 转化，仅使用用于 Z 轴的值。       |
   | scale3d(*x*,*y*,*z*)                                         | 定义 3D 缩放转换。                        |
   | scaleX(*x*)                                                  | 定义 3D 缩放转换，通过给定一个 X 轴的值。 |
   | scaleY(*y*)                                                  | 定义 3D 缩放转换，通过给定一个 Y 轴的值。 |
   | scaleZ(*z*)                                                  | 定义 3D 缩放转换，通过给定一个 Z 轴的值。 |
   | rotate3d(*x*,*y*,*z*,*angle*)                                | 定义 3D 旋转。                            |
   | rotateX(*angle*)                                             | 定义沿 X 轴的 3D 旋转。                   |
   | rotateY(*angle*)                                             | 定义沿 Y 轴的 3D 旋转。                   |
   | rotateZ(*angle*)                                             | 定义沿 Z 轴的 3D 旋转。                   |
   | perspective(*n*)                                             | 定义 3D 转换元素的透视视图。              |

#### 3.7.2 过渡

1. 通过使用 CSS3，可以给元素添加一些效果

2. CSS3 过渡是元素从一种样式转换成另一种样式

   - 动画效果的 CSS
   - 动画执行的时间

3. 下表列出了所有的过渡属性:

   | 属性                                                         | 描述                                         | CSS  |
   | :----------------------------------------------------------- | :------------------------------------------- | :--- |
   | [transition](https://www.runoob.com/cssref/css3-pr-transition.html) | 简写属性，用于在一个属性中设置四个过渡属性。 | 3    |
   | [transition-property](https://www.runoob.com/cssref/css3-pr-transition-property.html) | 规定应用过渡的 CSS 属性的名称。              | 3    |
   | [transition-duration](https://www.runoob.com/cssref/css3-pr-transition-duration.html) | 定义过渡效果花费的时间。默认是 0。           | 3    |
   | [transition-timing-function](https://www.runoob.com/cssref/css3-pr-transition-timing-function.html) | 规定过渡效果的时间曲线。默认是 "ease"。      | 3    |
   | [transition-delay](https://www.runoob.com/cssref/css3-pr-transition-delay.html) | 规定过渡效果何时开始。默认是 0。             | 3    |

4. 代码：

   ```HTML
   <!DOCTYPE html>
   <html>
   <head>
   <meta charset="utf-8"> 
   <title>菜鸟教程(runoob.com)</title>
   <style> 
   div {
       width: 100px;
       height: 100px;
       background: red;
       -webkit-transition: width 2s, height 2s, -webkit-transform 2s; /* For Safari 3.1 to 6.0 */
       transition: width 1s, height 1s, transform 1s;
   }
   
   div:hover {
       width: 200px;
       height: 200px;
       -webkit-transform: rotate(360deg); /* Chrome, Safari, Opera */
       transform: rotate(360deg);
   }
   </style>
   </head>
   <body>
   <p><b>注意：</b>该实例无法在 Internet Explorer 9 及更早 IE 版本上工作。</p>
   
   <div>鼠标移动到 div 元素上，查看过渡效果。</div>
   </body>
   </html>
   ```

5. 表格中的数字表示支持该属性的第一个浏览器版本号。

   紧跟在 -webkit-, -ms- 或 -moz- 前的数字为支持该前缀属性的第一个浏览器版本号。

   | 属性                       |                   |      |                |                  |               |
   | :------------------------- | ----------------- | ---- | -------------- | ---------------- | ------------- |
   | transition                 | 26.0 4.0 -webkit- | 10.0 | 16.0 4.0 -moz- | 6.1 3.1 -webkit- | 12.1 10.5 -o- |
   | transition-delay           | 26.0 4.0 -webkit- | 10.0 | 16.0 4.0 -moz- | 6.1 3.1 -webkit- | 12.1 10.5 -o- |
   | transition-duration        | 26.0 4.0 -webkit- | 10.0 | 16.0 4.0 -moz- | 6.1 3.1 -webkit- | 12.1 10.5 -o- |
   | transition-property        | 26.0 4.0 -webkit- | 10.0 | 16.0 4.0 -moz- | 6.1 3.1 -webkit- | 12.1 10.5 -o- |
   | transition-timing-function | 26.0 4.0 -webkit- | 10.0 | 16.0 4.0 -moz- | 6.1 3.1 -webkit- | 12.1 10.5 -o- |

#### 3.7.3 动画

1. 通过 CSS3 创建动画

2. CSS3 的动画需要遵循 @keyframes 规则

   - 规定动画的时长
   - 规定动画的名称

3. 下面的表格列出了 @keyframes 规则和所有动画属性：

   | 属性                                                         | 描述                                                         | CSS  |
   | :----------------------------------------------------------- | :----------------------------------------------------------- | :--- |
   | [@keyframes](https://www.runoob.com/cssref/css3-pr-animation-keyframes.html) | 规定动画。                                                   | 3    |
   | [animation](https://www.runoob.com/cssref/css3-pr-animation.html) | 所有动画属性的简写属性，除了 animation-play-state 属性。     | 3    |
   | [animation-name](https://www.runoob.com/cssref/css3-pr-animation-name.html) | 规定 @keyframes 动画的名称。                                 | 3    |
   | [animation-duration](https://www.runoob.com/cssref/css3-pr-animation-duration.html) | 规定动画完成一个周期所花费的秒或毫秒。默认是 0。             | 3    |
   | [animation-timing-function](https://www.runoob.com/cssref/css3-pr-animation-timing-function.html) | 规定动画的速度曲线。默认是 "ease"。                          | 3    |
   | [animation-fill-mode](https://www.runoob.com/cssref/css3-pr-animation-fill-mode.html) | 规定当动画不播放时（当动画完成时，或当动画有一个延迟未开始播放时），要应用到元素的样式。 | 3    |
   | [animation-delay](https://www.runoob.com/cssref/css3-pr-animation-delay.html) | 规定动画何时开始。默认是 0。                                 | 3    |
   | [animation-iteration-count](https://www.runoob.com/cssref/css3-pr-animation-iteration-count.html) | 规定动画被播放的次数。默认是 1。                             | 3    |
   | [animation-direction](https://www.runoob.com/cssref/css3-pr-animation-direction.html) | 规定动画是否在下一周期逆向地播放。默认是 "normal"。          | 3    |
   | [animation-play-state](https://www.runoob.com/cssref/css3-pr-animation-play-state.html) | 规定动画是否正在运行或暂停。默认是 "running"。               | 3    |

4. 代码：

   ```HTML
   <!DOCTYPE html>
   <html>
   <head>
   <meta charset="utf-8"> 
   <title>菜鸟教程(runoob.com)</title>
   <style> 
   div
   {
   	width:100px;
   	height:100px;
   	background:red;
   	position:relative;
   	animation-name:myfirst;
   	animation-duration:5s;
   	animation-timing-function:linear;
   	animation-delay:2s;
   	animation-iteration-count:infinite;
   	animation-direction:alternate;
   	animation-play-state:running;
   	/* Safari and Chrome: */
   	-webkit-animation-name:myfirst;
   	-webkit-animation-duration:5s;
   	-webkit-animation-timing-function:linear;
   	-webkit-animation-delay:2s;
   	-webkit-animation-iteration-count:infinite;
   	-webkit-animation-direction:alternate;
   	-webkit-animation-play-state:running;
   }
   
   @keyframes myfirst
   {
   	0%   {background:red; left:0px; top:0px;}
   	25%  {background:yellow; left:200px; top:0px;}
   	50%  {background:blue; left:200px; top:200px;}
   	75%  {background:green; left:0px; top:200px;}
   	100% {background:red; left:0px; top:0px;}
   }
   
   @-webkit-keyframes myfirst /* Safari and Chrome */
   {
   	0%   {background:red; left:0px; top:0px;}
   	25%  {background:yellow; left:200px; top:0px;}
   	50%  {background:blue; left:200px; top:200px;}
   	75%  {background:green; left:0px; top:200px;}
   	100% {background:red; left:0px; top:0px;}
   }
   </style>
   </head>
   <body>
   
   <p><b>注意:</b> 该实例在 Internet Explorer 9 及更早 IE 版本是无效的。</p>
   
   <div></div>
   
   </body>
   </html>
   ```

#### 3.7.4 多列

1. 在 CSS3 中，可以创建多列来对文本或者区域进行布局

2. 下表列出了所有 CSS3 的多列属性：

   | 属性                                                         | 描述                                     |
   | :----------------------------------------------------------- | :--------------------------------------- |
   | [column-count](https://www.runoob.com/cssref/css3-pr-column-count.html) | 指定元素应该被分割的列数。               |
   | [column-fill](https://www.runoob.com/cssref/css3-pr-column-fill.html) | 指定如何填充列                           |
   | [column-gap](https://www.runoob.com/cssref/css3-pr-column-gap.html) | 指定列与列之间的间隙                     |
   | [column-rule](https://www.runoob.com/cssref/css3-pr-column-rule.html) | 所有 column-rule-* 属性的简写            |
   | [column-rule-color](https://www.runoob.com/cssref/css3-pr-column-rule-color.html) | 指定两列间边框的颜色                     |
   | [column-rule-style](https://www.runoob.com/cssref/css3-pr-column-rule-style.html) | 指定两列间边框的样式                     |
   | [column-rule-width](https://www.runoob.com/cssref/css3-pr-column-rule-width.html) | 指定两列间边框的厚度                     |
   | [column-span](https://www.runoob.com/cssref/css3-pr-column-span.html) | 指定元素要跨越多少列                     |
   | [column-width](https://www.runoob.com/cssref/css3-pr-column-width.html) | 指定列的宽度                             |
   | [columns](https://www.runoob.com/cssref/css3-pr-columns.html) | 设置 column-width 和 column-count 的简写 |

#### 3.7.5 瀑布流效果

1. 用多列实现

###  3.8 HTML与CSS简单页面效果实例

1. 简单布局

## 4. JavaScript 基础（跳过）

### 4.1 JavaScript基础教程
### 4.2 JavaScript语法详解
### 4.3 JavaScript函数
### 4.4 JavaScript异常处理和事件处理

#### 4.4.1 捕获异常，自定义输出异常

```JS
// 捕获异常，自定义输出异常
function demo() {
	try {
		alert(str)
	}catch (err) {
		alert(err)
	}
}
```

#### 4.4.1 事件处理

- 下面是一些常见的HTML事件的列表:

  | 事件        | 描述                         |
  | :---------- | :--------------------------- |
  | onchange    | HTML 元素改变                |
  | onclick     | 用户点击 HTML 元素           |
  | onmouseover | 用户在一个HTML元素上移动鼠标 |
  | onmouseout  | 用户从一个HTML元素上移开鼠标 |
  | onkeydown   | 用户按下键盘按键             |
  | onload      | 浏览器已完成页面的加载       |

### 4.5 JavaScript DOM对象

### 4.6 JavaScript事件详解
### 4.7 JavaScript内置对象
### 4.8 JavaScript DOM对象控制HTML元素详解
### 4.9 JavaScript浏览器对象
### 4.10 JavaScript面向对象详解
### 4.12 Javascript瀑布流

## 5. HTML5 新特性基础

### 5.1 HTML5音频视频

#### 5.1.1 音频播放

1. Audio 音频：HTML5 提供了音频播放标准
2. control 控制器：提供添加播放、暂停和音量控件
3. 标签：
   - `<audio>`：定义声音
   - `<source>`：规定多媒体资源，可以是多个

#### 5.1.2 编解码工具

1. FFmpeg
2. 官方网址：www.ffmpeg.org
3. 使用命令行控制

#### 5.1.3 视频播放

1. Video 视频：HTML5 视频播放标准

2. control 控制器：提供添加播放、暂停和音量控件

3. 标签：

   - `<video>`：定义声音
   - `<source>`：规定多媒体资源，可以是多个

4. 属性：

   - width：宽
   - height：高

5. 代码：例子调用了两个方法：play() 和 pause()。它同时使用了两个属性：paused 和 width

   ```HTML
   <!DOCTYPE html> 
   <html> 
   <head> 
   <meta charset="utf-8"> 
   <title>菜鸟教程(runoob.com)</title> 
   </head>
   <body> 
   
   <div style="text-align:center"> 
     <button onclick="playPause()">播放/暂停</button> 
     <button onclick="makeBig()">放大</button>
     <button onclick="makeSmall()">缩小</button>
     <button onclick="makeNormal()">普通</button>
     <br> 
     <video id="video1" width="420">
       <source src="mov_bbb.mp4" type="video/mp4">
       <source src="mov_bbb.ogg" type="video/ogg">
       您的浏览器不支持 HTML5 video 标签。
     </video>
   </div> 
   
   <script> 
   var myVideo=document.getElementById("video1"); 
   
   function playPause()
   { 
   	if (myVideo.paused) 
   	  myVideo.play(); 
   	else 
   	  myVideo.pause(); 
   } 
   
   	function makeBig()
   { 
   	myVideo.width=560; 
   } 
   
   	function makeSmall()
   { 
   	myVideo.width=320; 
   } 
   
   	function makeNormal()
   { 
   	myVideo.width=420; 
   } 
   </script> 
   
   </body> 
   </html>
   ```

### 5.2 HTML5拖放

#### 5.2.1 拖放标签

1. 拖放（Drag 和 drop）是 HTML5 标准的组成部分。

2. 为了使元素可拖动，把 draggable 属性设置为 true

   - `<img draggable="true">`
   - `ev.preventDefault();` 阻止系统默认事件

3. 拖动：

   - ondragstart：调用了一个函数，drag(event)，规定了被拖动的数据
   - setData()：设置被拖动数据的数据类型和值
   - ondragover：事件规定在何处放置被拖动的数据
   - ondrop：放置被拖动数据时发生 drop 事件

4. 代码：

   ```HTML
   <!DOCTYPE html>
   <html>
   <head>
   <meta charset="utf-8"> 
   <title>菜鸟教程(runoob.com)</title>
   <style type="text/css">
   #div1, #div2
   {float:left; width:100px; height:35px; margin:10px;padding:10px;border:1px solid #aaaaaa;}
   </style>
   <script>
   function allowDrop(ev)
   {
   	ev.preventDefault();
   }
   
   function drag(ev)
   {
   	ev.dataTransfer.setData("Text",ev.target.id);
   }
   
   function drop(ev)
   {
   	ev.preventDefault();
   	var data=ev.dataTransfer.getData("Text");
   	ev.target.appendChild(document.getElementById(data));
   }
   </script>
   </head>
   <body>
   
   <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)">
   	<img src="img_w3slogo.gif" draggable="true" ondragstart="drag(event)" id="drag1" width="88" height="31"></div>
   <div id="div2" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
   
   </body>
   </html>
   ```

#### 5.2.2 拖放文件

1. 代码：

   ```HTML
   
   ```

### 5.3 HTML5Canvas标签

#### 5.3.1 创建Canvas标签

1. Canvas 标签：
   - HTML5 `<canvas>` 元素用于图形的绘制，通过脚本（JS）来完成
   - `<canvas>` 标签只是容器，必须使用脚本来绘制图形
   - 有多种方式使用 Canvas 绘制路径、盒子、圆、字符以及添加图像

#### 5.3.1 绘制图形

1. `<canvas>` 标签只是容器，必须使用 JavaScript 来绘制图形

2. 代码：

   ```
   
   ```

   

#### 5.3.1 绘制图片

### 5.4 HTML5 Canvas应用

#### 5.4.1 Canvas应用

### 5.5 SVG

#### 5.5.1 什么是SVG

1. SVG 指可伸缩矢量图形（Scalable Vector Graphics）
2. SVG 用来定义用于网络的基于矢量的图形
3. SVG 使用 XML 格式定义图形
4. SVG 图像在放大 

### 5.6 Web储存
### 5.7 HTML5 应用缓存与Web Workers
### 5.8 服务器推送事件

## 6. 响应式布局

### 6.1 响应式布局基础
### 6.2 响应式布局之Bootstrap

## 7. JQurey 基础

### 7.1 jQuery简介及语法
### 7.2 jQuery选择器和事件
### 7.3 jQuery效果之隐藏与显示、淡入淡出、滑动、回调
### 7.4 jQuery HTML之捕获、设置、元素添加、元素删除
### 7.5 jQuery CSS操作及jQuery的盒子模型
### 7.6 jQuery之元素的遍历与元素的过滤
### 7.7 jQuery AJAX之异步访问和加载片段
### 7.8 jQuery的扩展与noConflict
### 7.9 jQuery UI下载与使用
### 7.10 jQuery瀑布流

## 8. JQuery UI 基础

### 8.1 jQuery UI下载与使用
### 8.2 jQuery UI Interactions
### 8.3 jQuery UI Widgets(1)
### 8.4 jQuery UI Widgets(2)
### 8.5 jQuery UI Effects

## 9. JQurey Mobile 基础

### 9.1 了解jQuery Mobile
### 9.2 jQuery Mobile Widgets(1)
### 9.3 jQuery Mobile Widgets(2)
### 9.4 jQuery Mobile 事件

## 10. CreateJS 基础

### 10.1 CreateJS介绍

### 10.2 CreateJS基础

### 10.3 CreateJS控件

### 10.4 CreateJS-TweenJS

### 10.5 Createjs与flash生成js文件交互

## 11. TypeScript 基础

### 11.1 TypeScript环境搭建
### 11.2 TypeScript基本数据类型
### 11.3 TypeScript接口(Interfaces)
### 11.4 TypeScript函数
### 11.5 TypeScript类(Classes)

## 12. 实战开发教程

### 12.1 围住神经猫-HTML5实战游戏开发教程

### 12.2 看你有多色-HTML5实战游戏开发教程

### 12.3 冰桶挑战-HTML5-实战游戏开发教程

### 12.4 打企鹅-HTML5游戏实战开发

### 12.5 javascript语音识别库-julius

### 12.6 极客学院页面布局实现

### 12.7 极客学院播放视频页面布局

### 12.8 极客学院路径图页面布局实现

### 12.9 标签切换效果

### 12.10 回到顶部功能实现

### 12.11 图片与标签配合制作页面

### 12.12 导航栏

### 12.13 Tooltip

### 12.14 幽灵按钮

### 12.15 列表切换

### 12.16 侧边栏固定

### 12.17 照片墙

### 12.18.微信内网页开发工具包(微信JS-SDK)

