# HTML5与CSS3实现动态网页

## 步骤1: 初识HTML5
	本阶段内容主要涵盖H5新增、删除标签、标签属性变化以及HTML5布局知识。
	通过本阶段学习，大家可以运用HTML5标签轻松实现网页音乐播放器和视频播放器，熟练运用HTML5的语义化标签进行静态网页的开发。
- HTML5 ≈ HTML + CSS + JS + API

- #### 学前准备：

  ​	了解HTML基本知识
  ​	具备CSS基础
  ​	熟练使用JavaScript

- #### 移动互联网 HTML5 的优势

  - 跨平台
    - HTML5 是唯一通吃PC、Mac、iPhone、Android等主流平台的语言
  - 快速迭代
    - 互联网产品大多免费、且有网络效应，后来者抢夺用户难度非常大
  - 减低成本
    - HTML5 开发比原生APP开发成本低一半
  - 导流入口多
    - HTML5 应用导流非常容易

- #### Web 改变趋势

  - Native APP → WebApp → Hybrid App
  - PC → 移动 → 智慧互联

- #### 学习目标

  - 掌握新标签以及新属性的功能特点，并熟练应用
  - 了解HTML5的前景及学习展望
  - 明确未来的学习目标和深入学习的方向
  - 为移动前端打好基础



### 第1课 HTML5标签变化

		HTML5标签变化
		HTML5文档类型如何定义，有哪些标签，以及如何使用，从整体认识HTML5
		DTD、新增的标签、删除的标签、重定义标签
- HTML `<!DOCTYPE>` 标签

  - 定义和用法：

    - 版本声明，在文档的第一行

  - 不是 HTML 标签

  - 常用声明：

    > ### HTML 4.01 Strict
    >
    > 该 DTD 包含所有 HTML 元素和属性，但不包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。
    >
    > ```
    > <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
    > ```
    >
    > ### HTML 4.01 Transitional
    >
    > 该 DTD 包含所有 HTML 元素和属性，包括展示性的和弃用的元素（比如 font）。不允许框架集（Framesets）。
    >
    > ```
    > <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" 
    > "http://www.w3.org/TR/html4/loose.dtd">
    > ```
    >
    > ### HTML 4.01 Frameset
    >
    > 该 DTD 等同于 HTML 4.01 Transitional，但允许框架集内容。
    >
    > ```
    > <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" 
    > "http://www.w3.org/TR/html4/frameset.dtd">
    > ```

- 文档类型定义（DTD)

  - DTD：定义合法的 XML 文档构建模块，它使用一系列合法元素来定义文档结构
  - HTML 中的 DTD：规定了标记语言的规则，浏览器才能正确的显示内容
  - HTML5 中的 DTD：HTML5 不基于 SGML，所以不需要引用 DTD
  - HTML 元素和文档类型：www.w3school.com.cn/tags/html_ref_dtd.asp



#### 新增的标签

##### 结构标签

- 块状元素，有意义的 div

| 标签           | 描述                           |
| -------------- | ------------------------------ |
| `<header>`     | 定义了一个页面或一个头部区域   |
| `<nav>`        | 定义导航栏链接                 |
| `<section>`    | 定义一个区域                   |
| `<aside>`      | 定义页面内容部分的侧边栏       |
| `<hgroup>`     | 定义文件中一个区块的相关信息   |
| `<figure>`     | 定义一组媒体内容以及他们的标题 |
| `<figcaption>` | 定义 figure 元素的标题         |
| `<footer>`     | 定义一个页面或一个区域的底部   |
| `<article>`    | 定义一篇文章                   |
| `<dialog>`     | 定义一个会话框，类似微信       |

- 标签嵌套级别：header / section / footer > aside / article / figure / hgroup / nav > div / figcaption

##### 多媒体标签

- 三类媒体标签

| 标签       | 描述                                    |
| ---------- | --------------------------------------- |
| `<video>`  | 定义一个视频                            |
| `<audio>`  | 定义音频内容                            |
| `<source>` | 定义媒体资源                            |
| `<canvas>` | 定义画布                                |
| `<embed>`  | 定义外部的可交互的内容或插件，如：flash |

- 默认属性：`controls="controls" width="200px" autoplay="autoplay" loop="-1"`
- 标签的意义：多媒体标签的出现意味着富媒体的发展以及支持不使用插件的情况下操作媒体文件，极大的提高可用户体验

##### Web 应用标签

- ##### 状态标签：

  | 标签         | 描述                                 |
  | ------------ | ------------------------------------ |
  | `<meter>`    | 状态标签（实时状态显示：气压、气温） |
  | `<progress>` | 状态标签（任务过程：安装、加载）     |

  - 浏览器兼容：

  | 标签         | 兼容性                 |
  | ------------ | ---------------------- |
  | `<meter>`    | Chrome、Opera          |
  | `<progress>` | Chrome、FireFox、Opera |

- ##### 列表标签

  | 标签         | 描述                                           |
  | ------------ | ---------------------------------------------- |
  | `<datalist>` | 为 `input` 标记定义一个下拉列表，配合 `option` |
  | `<details>`  | 标记定义一个元素的详细内容，配合 `summary`     |

  - 浏览器兼容

  | 标签         | 兼容性         |
  | ------------ | -------------- |
  | `<datalist>` | FireFox、Opera |
  | `<datails>`  | Chrome         |

- ##### Menu 标签

  | 标签         | 描述                                       |
  | ------------ | ------------------------------------------ |
  | `<menu>`     | 命令列表（**目前所有浏览器不支持**）       |
  | `<menuitem>` | menu 命令列表标签（只有 FireFox8.0+ 支持） |
  | `<command>`  | menu 标记定义一个命令按钮（只有 IE9 支持） |

##### 其它标签

- 注释标签

  | 标签     | 描述                         |
  | -------- | ---------------------------- |
  | `<ruby>` | 定义注释或音标               |
  | `<rt>`   | 定义对ruby的注释内容文本     |
  | `<rp>`   | 告诉不支持的浏览器如何去显示 |

- `<mark>` ：定义有标记的文本（黄色选中显示）

  - 兼容IE9以上所有浏览器

- `<output>` ：定义一些输出类型，计算表单结果配合 `oninput` 事件

- `<keygen>` ：定义表单里一个生成的键值（加密信息传送）

- `<time>` ：定义一个日期/事件，目前所有主流浏览器都不支持

#### 删除的标签

- 纯表现的元素
  - basefont、big、center、font、s、strike、tt、u
- 对可用性产生负面影响的元素
  - frame、frameset、noframes
- 产生混淆的元素
  - acronym、applet、isindex、dir

#### 重定义标签

- 显示不变，表达的含义进行了重新定义的标签

  | 标签       | 描述                                                        |
  | ---------- | ----------------------------------------------------------- |
  | `<b>`      | 代表内联文本，通常是粗体，没有传递表示重要的意思            |
  | `<i>`      | 代表内联文本，通常是斜体，没有传递表示重要的意思            |
  | `<dd>`     | 可以同details于figure以前使用，定义包含文本，dialog也可以用 |
  | `<dt>`     | 可以同details于figure以前使用，汇总细节，dialog也可以用     |
  | `<hr>`     | 表示主题结束，而不是水平线，虽然显示相同                    |
  | `<menu>`   | 重新定义用户界面菜单，配合commond或者menitem使用            |
  | `<small>`  | 表示小字体，例如打印注释或者法律条款                        |
  | `<strong>` | 表示重要性而不是强调符号                                    |

  

### 第2课 HTML5网页布局

		HTML5网页布局
		传统布局与HTML5网页布局的区别和意义，通过案例讲解如何使用HTML5搭建网页
#### 传统布局与HTML5布局

<img src="E:\web\学习笔记\HTML5+CSS+JS+Bootstrap+jQuery+CreateJS+TypeScript+实战系列视频_notes\HTML5-imooc.assets\20200104215508.png"/>

![](E:\web\学习笔记\HTML5+CSS+JS+Bootstrap+jQuery+CreateJS+TypeScript+实战系列视频_notes\HTML5-imooc.assets\20200104215554.png)

#### 新布局的意义

- 语义化
  - HTML5 可以让更语义化的结构化代码标签代替大量的无意义的 div 标签
    - 这种语义化特性提升了网页的质量和语义
    - 减少了以前用于 CSS 调用的 class 和 id 属性
  - 对搜索引擎更友好
    - 新的架构标签带来的是网页布局的改变，即提升搜索引擎的友好

#### HTML5 慕课网布局

- 代码：

  ```
  
  ```

  

### 第3课 HTML5属性变化

		HTML5属性变化
		了解这些属性带来的好处，加深对标签的认识，将提高以后的开发效率
		input、表单属性、链接属性、其它属性 
#### input 属性

- email 、url、number、tel ：手机端输入法有效果
- Date picker 类型：
  - Date：选取日、月、年
  - Mouth：选取月、年
  - Week：选取周、年
  - Time：选取时间（小时、分钟）
  - Datetime：选取时间、日、月、年（utc时间），safari opera兼容
  - Datetime-local：选取使时间、日、月、年（本地时间）chrome safari opera兼容
- range 类型：取值范围，`<input type="range" name="range" min="1" max="10">`
- search 类型：带清空的输入框，`<input type="search" name="search">`
- color 类型：取色器，`<input type="color" name="color">`

#### 表单属性

- autocomplete 属性：
  - `form` 或 `input` 域应该拥有自动完成功能
  - `<form autocomplete="on"></form> `
  - autocomplete 适用于 `<form>` 标签，以及以下类型的 `<input>` 标签：
    - text、search、url、telephone、email、password、datepickers、range、color
- `autofocus="autofocus"` 属性：
  - 页面加载时，域自动获得焦点
  - `<input type="text autofocus="autofocus">`
  - 适用于所有 input 标签
- multiple 属性：
  - 规定输入域中可以选择多个值
  - `<input type="text multiple="multiple">`
  - 适用于email、file类型 input标签
- placeholder 属性：
  - 提供一种提示（hint），描述输入域所期待的值
  - `<input type="search" placeholder="Search Content"`
  - 适用于 input 标签 type 属性为：
    - text、search、url、telephone、email、password
- required 属性：
  - 规定必须在提交之前填写输入域（不能为空）
  - `<input type="text" required="required">`
  - 适用于 input 标签 type 属性为：
    - text、search、url、telephone、email、password、date pinckers、number、checkbox、radio、file

#### 链接属性

- `<link>` 的 `sizes` 属性：
  - `<link rel="icon" href="icon.gif" type="image/gif" sizes="16x16">`
- `<base>` 的 `target` 属性 ：
  - `<base href="http://localhost/" target="_blank">`
- 超链接`<a>` 属性：
  - `a:meida=""`：表示对设备进行优化，`handhelp` 对手持设备支持，`tv` 对电视设备支持
  - `a:hreflang="zh"`：设置语言，这里表示中文
  - `a:rel="external"`：设置超链接的引用，这里表示外部链接

#### 其它属性

- script 标签
  - defer：加载完脚本后并不执行，而是等整个页面加载完之后再执行
    - `<script defer src="url"></script>`
    - 原来只兼容IE，现在已经兼容所有浏览器
  - async：加载完脚本后立即执行，不用等整个页面加载完，属于异步执行
    - `<script async src="url"></script>`
    - 兼容所有浏览器
- ol 标签
  - Start：有序列表起始位置
  - Reserved：有序列表倒叙
- html 标签
  - manifest=”cache.manifest" 
    - 定义页面离线应用文件
    - `<html manifest="cache.manifest"`
- style 标签
  - scoped：内嵌 CSS
  - `<style scoped> </style>`

### 第4课 HTML5展望

		HTML5展望
		HTML5快速发展，它还有哪些强大的功能，在什么领域可以使用，以及它的发展方向
		简述Api、简述Canvas、移动端应用

#### 简述Api

API（Application Programming Interface）：应用程序编程接口

- Video-API
  - 六个方法
  - 三十个属性
  - 二十二歌事件

#### 简述Canvas

- 什么是Canvas ？
  - Canvas 元素用于在网页上绘制图形
  - Canvas 元素使用 JavaScript 在网页上绘制图像
  - 画布是一个矩形区域，可以通过API 控制其中每一个像素

#### 移动端应用

移动平台竞争→浏览器之争

- 离线缓存为HTML5开发移动应用提供了基础
  - Web Strorage、Local Storage
  - 加强版的cookie
  - 后台操作记录
- 音视频自由嵌入，多媒体形式更为灵活
- 地理定位，随时随地分享位置
- Canvas 绘图，提升移动平台的绘图能力
- 专为移动平台定制的表单元素
- 丰富的交互方式支持
- HTML5 使用上的优势
- CSS3 视觉设计师的辅助利器
  - 字体嵌入
  - 版面排版
  - 动画
- 实时通讯
- 档案以及硬件支持
  - 拖拽文件
- 语义化
- 双平台融合的app 开发方式，提高工作效率 
  - Hybrid APP

### 总结

HTML5 适合开发哪些应用？

##	步骤2: 搞懂CSS3

	本阶段内容主要涵盖CSS3选择器、边框、圆角、背景、渐变、转换、过渡、动画等知识。
	通过本阶段学习，大家将能够更加准确的控制页面的布局等样式效果，实现非常炫酷的CSS3动画特效，让网页丰富多彩。


### 第1课 CSS3选择器

	CSS3选择器
		详细讲解CSS3的变化，新的概念和理念，及其CSS3新增加的选择器

#### 基本选择器

- 回顾选择器
  - 通配符选择器、元素选择器、类选择器、ID选择器、后代选择器
- 新增基本选择器
  - 子元素选择器、相邻兄弟元素选择器、通用兄弟选择器、群组选择器

### 第2课 CSS3边框与圆角

		CSS3边框与圆角
		带来神奇的圆角边框、阴影框及其图片边框等，非常具有实用价值的新属性
#### CSS3 圆角

- border-radius 属性
  - 一个最多可指定四个 border -*- radius 属性的复合属性，这个属性允许你为元素添加添加圆角边框
    - *top right bottom left
  - 语法：`border-radius:1-4 length|% / 1-4 length|%`
  - 兼容性：IE9+、FireFox4+、Chrome、Safari5+、Opera
  - 多值：
    - 四个值：第一个值为左上角，第二个为右上角，第三个为右下角，第四个为左下角
    - 三个值：第一个为左上角，第二个为右上角和左下角，第三个值为右下角
    - 两个值：第一个为左上角和右下角，第二个为右上角和左下角
    - 一个值：四个圆角值相同

#### CSS3 盒阴影

- box-shadow 属性
  - box-shadow 属性可以设置一个或多个下拉阴影的框
  - 语法：`box-shadow:h-shadow v-shadow blur spread color inset;`
  - 兼容性：IE9+、FireFox4+、Chrome、Safari5+、Opera

#### CSS3 边界图片

- border-image 属性
  - 使用 border-image-* 属性来构建美丽的可扩展按钮 
  - 语法：`border-image: source slice width outset repeat;`
  - 兼容性：IE、Opera 不兼容，FireFox、Chrome、Safari6+ 兼容
- border-image-source 属性
  - border-image-source 属性指定要使用的图像，而不是由 border-style 属性设置的边框样式
  - 语法：`border-image-source: none|image;`
- border-image-slice 属性
  - border-image-slice 属性指定图像的边界向内偏移
  - 语法：`border-image-slice: number|%|fill;`
- border-image-width 属性
  - border-image-width 属性指定图像边界的宽度
  - 语法：`border-image-width: number|%|auto;`
- border-image-outset 属性
  - border-image-outset 属性指定在边框外部绘制 border-image-area 的量
  - 语法：`border-image-outset: length|number;`
- border-image-repeat 属性
  - border-image-repeat 属性用于图像边界是否应用重复（repeated）、拉伸（stretched）或铺满（rounded）
  - 语法：`border-image-repeat: stretch|repeat|round|initial|inherit;`

### 第3课 CSS3背景与渐变

		CSS3背景与渐变
		同样神奇的背景控制属性，以及如何使用颜色过渡实现漂亮的渐变效果
#### background-clip 属性

- background-clip 属性指定背景绘制区域
- 语法：`background-clip:border-box|padding-box|content-box;`
- 兼容性：IE9+，FireFox、Chrome、Safari、Opera

#### background-origin 属性

- 设置元素背景图片的原始起始位置

- background-origin 属性指定 background-position 数值应该是相对位置
- 语法：`background-origin:border-box|padding-box|content-box;`
- 兼容性：IE9+，FireFox4+、Chrome、Safari5+、Opera

#### background-size 属性

- 定义背景图片大小
- 语法：background-size:length|percentage|cover|contain;
- 兼容性：IE9+，FireFox4+、Chrome、Safari5+、Opera

#### CSS3 多重背景图像

- CSS3 允许给元素使用多个背景图像
- 语法：`background-image:url(img1.jpg),url(img2.png)`

#### CSS3 背景属性整合

- 背景缩写属性可以在一个声明中设置所有的背景属性
- 语法：`background:color position size repeat origin clip attachment image`
  - attachment：是否滚动 fixed 固定

#### CSS3 渐变

- 渐变（gradients）可以在两个或多个指定的颜色之间显示平稳的过渡
- 兼容性：IE10+、 Chrome26+(10 -webkit-)、 FireFox16+(3.6 -moz-)、 Safari6.1+(5.1 -webkit)、 Opera12+(11.6 -o-)

#### CSS3 线性渐变

- 线性渐变（Linear Gradients）属性

  - 沿着一根轴线改变颜色，从起点到终点颜色进行顺序渐变（从一边拉到另一边）
  - transparent：透明色

- 语法：`background:linear-gradient(direction,color-stop1,color-stop2, ...)`

- 线性渐变-从上到下（默认）

  - `background:linear-gradient(color-stop1,color-stop2, ...)`

- 线性渐变 - 从左到右

  ```
  background:-webkit-linear-gradient(begin-direction,color-stop1,color-stop2, ...);
  background:   -moz-linear-gradient(	 end-direction,color-stop1,color-stop2, ...);
  background:			-o-linear-gradient(	 end-direction,color-stop1,color-stop2, ...);
  background:				 linear-gradient(to end-direction,color-stop1,color-stop2, ...);
  ```

- 线性渐变 - 对角

  ```
  background:-webkit-linear-gradient(begin-level begin-vertical,color-stop1,color-stop2, ...);
  background:   -moz-linear-gradient(begin-level end-vertical,color-stop1,color-stop2, ...);
  background:			-o-linear-gradient(end-level end-vertical,color-stop1,color-stop2, ...);
  background:				 linear-gradient(to end-level end-vertical,color-stop1,color-stop2, ...);
  ```

- 线性渐变 - 使用角度

  - 语法：`background:linear-gradient(angle,color-stop1,color-stop2, ...);`
  - 角度说明：
    - 角度指水平线和渐变线之间的角度，逆时针方向计算
    - 0deg 将创建一个从上至下的渐变，90deg 将创建一个从左至右的渐变

  ![image-20200105112613428](E:\web\学习笔记\HTML5+CSS+JS+Bootstrap+jQuery+CreateJS+TypeScript+实战系列视频_notes\HTML5-imooc.assets\image-20200105112613428.png)

- 线性渐变 - 颜色节点

  - 语法：`background:linear-gradient(color1 length|percentage,color2 length|percentage, ...);`

- 线性渐变 - 重复渐变

  - 语法：`background:repeating-linear-gradient(color1 length|percentage,color2 length|percentage, ...);`

#### CSS3 径向渐变

- 径向渐变（Radial Gradients）属性
  - 从起点到终点颜色从内到外进行圆形渐变（从中间往外拉）
  - 语法：`background:radial-gradient(center,shape size, start-color, ...,last-color);`
- 径向渐变 - 颜色节点不均匀分布
  - `background: radial-gradient(color1 length|percentage, color2 length|percentage, ...);`
- 径向渐变 - 设置形状
  - 语法：`background:radial-gradient(shape,color-stop1,color-stop2, ...)`
  - 形状：
    - circle：圆形
    - ellipse：椭圆（默认）
- 径向渐变 - 尺寸大小关键字
  - 语法：`background:radial-gradient(size,color-stop1,color-stop2, ...)`
  - 关键字说明：
    - closest-side：最近边；farehest-side：最远边；
    - closest-corner：最近角；farthest-corner：最远角；
- 径向渐变 - 重复渐变
  - 语法：`background:repeating-radial-gradient(color1 length|percentage,color2 length|percentage, ...);`

#### 其它渐变

- Internet Explorer6-8 渐变语法：
  - `filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='startColor',endColorstr='endColor',GradientType=0);`
  - 例：`filter:progid:DXImageTransform.Microsoft.gradient(startColorstr='#ff0000',endColorstr='#0000ff',GradientType=0);`

#### 实战案例：

### 第4课 CSS3转换

		CSS3转换
		深入讲解元素如何扭曲、移位或旋转，让我们可以更自由得装饰和变形HTML组件


### 第5课 CSS3过渡

		CSS3过渡
		一起探索如何通过CSS3属性值的变化实现动画效果，如何触发这些动画产生交互


### 第6课 CSS3动画

		CSS3动画
		使用animation属性，实现以往要用Flash等动画软件才能完成的炫酷效果


### 第7课 CSS3图片切换特效

		CSS3图片切换特效
		介绍了几种非常漂亮的图片切换特效，大家对CSS3的认识会有质的提高



## 步骤3: JavaScript基础

	本阶段内容主要涵盖js基础语法、流程控制语句、函数、内置对象、DOM基础和事件、BOM基础等知识。
	通过本阶段学习，大家不仅可以掌握js的基础知识，还能学会网站开发中常用的图片轮播特效。


### 第1课 语法

		JavaScript语法
		本课程讲解JavaScript的语法、数据类型、基本算数和逻辑运算操作


### 第2课 流程控制语句

		JavaScript流程控制语句
		掌握JavaScript中条件分支语句和循环语句的使用，用简洁的代码实现强大功能


### 第3课 函数

		JavaScript函数
		掌握函数的使用，学习函数的封装，体会代码复用的过程和它带来的便利


### 第4课 内置对象

		JavaScript内置对象
		学习内置对象的常用属性和方法，方便我们开发中直接调用，进而实现更多功能


### 第5课 DOM基础

		JavaScript DOM基础
		DOM的方法和属性既可以获取网页中的元素，也可以设置元素的内容、样式及效果


### 第6课 DOM事件

		JavaScript DOM事件
		为页面中的元素绑定键盘或鼠标事件，从而可以触发和实现我们想要的交互效果


### 第7课 BOM基础

		JavaScript BOM基础
		学习浏览器对象模型“BOM”，可以对浏览器窗口进行访问和操作，与浏览器“对话”


### 第8课 实现轮播特效

		JavaScript实现轮播特效
		综合运用JavaScript知识，做出轮播图、tab页切换等实用特效



## 步骤4: JavaScript进阶

	本阶段，将带领大家进一步探索JavaScript中的奥秘，教大家如何使用调试工具。还有变量、作用域、函数是怎么样来运用， 以及它们之前的关系是怎样的，我们来一步一步揭开它们的面纱。


### 第1课 调试工具

		调试工具
		学习调试工具，实践如何快速调试代码，并实时预览，体验快速调试代码的过程


### 第2课 变量、作用域

		JavaScript变量、作用域
		我们一起探究变量、作用域的本质，了解它们的定义及使用方法


### 第3课 函数深入讲解

		JavaScript函数深入讲解
		研究函数的本质，了解函数的定义、调用，以及函数的参数和返回值


### 第4课 实现简易计算器

		JavaScript实现简易计算器
		本课程讲解简易计算器的实现，体会代码优化过程及其简约而不简单的魅力



## 步骤5: 项目实战

		光学不练假把式，实践是巩固知识最好的方法，本环节，将带领大家一步步开发出炫酷的动态网页，让大家能够从实践中总结经验，并且提升解决问题的能力。


### 第1课 H5+CSS3+JS实现炫酷网页

		H5+CSS3+JS实现炫酷网页
		带领大家实现真实项目：“慕课手机宣传页”，面对综合需求，大展身手的时候到了！