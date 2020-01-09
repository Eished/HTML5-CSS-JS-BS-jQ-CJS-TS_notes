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

<img src="HTML5-imooc.assets\20200104215508.png"/>

![](HTML5-imooc.assets\20200104215554.png)

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

#### 子元素选择器

- 概念：直接后代选择器
  - 子元素选择器只能选择某些元素的子元素
- 语法：
  - 父元素 > 子元素 （Father > Children）
- 兼容性：
  - IE8+、FireFox、Chrome、Safari、Opera

#### 相邻兄弟元素选择器

- 概念
  - 相邻兄弟元素选择器可以选择紧接在另一元素后的元素，且它们具有相同父元素
- 语法：
  - 元素 + 相邻兄弟元素 (Element + Sibling )
- 兼容性
  - IE8+、FireFox、Chrome、Safari、Opera

#### 通用兄弟选择器

- 概念
  - 选择元素**后面的所有**兄弟元素，且它们具有相同父元素
- 语法：
  - 元素 ~ 相邻兄弟元素 (Element ~ Sibling )
- 兼容性
  - IE8+、FireFox、Chrome、Safari、Opera

#### 群组选择器

- 概念
  - 群组选择器是将具有相同样式的元素分组在一起，每个选择器之间使用逗号 "," 隔开
- 语法：
  - 元素1, 元素2, ..., 元素n { Element1, Element2, ..., Elementn}
- 兼容性
  - IE6+、FireFox、Chrome、Safari、Opera

#### 属性选择器

- 对带有指定属性的HTML 元素设置样式

  - 使用CSS3 属性选择器，你可以只指定元素的某个属性，或者同时指定元素的某个属性和其对应的属性值

- ##### Element[attribute]

  - 概念
    - 为带有 attribute 属性的 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

- ##### Element[attribute = "value"]

  - 概念
    - 为带有 attribute = "value" 属性的 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

- ##### Element[attribute ~= "value"]

  - 概念
    - 为 attribute 属性**包含**单词 "value" 的 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

- ##### Element[attribute ^= "value"]

  - 概念
    - 为 attribute 属性值以 "value" **开头**的所有 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

- ##### Element[attribute $= "value"]

  - 概念
    - 为 attribute 属性值以 "value" **结尾**的所有 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

- ##### Element[attribute *= "value"]

  - 概念：**常用**
    - 为 attribute 属性值包含 "value" 的所有 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

- ##### Element[attribute |= "value"]

  - 概念：**常用**
    - 为 attribute 属性值以 "value" 或以 "-value" 开头的所有 Element 元素设置样式
  - 兼容性
    - IE8+、FireFox、Chrome、Safari、Opera

#### 伪类选择器

##### 动态伪类

- 动态伪类
  - 这些伪类不存在于HTML中，只有当用户和网站交互的时候才能体现出来
- 锚点伪类
  - `:link`, `:visited`
- 用户行为伪类
  - `:hover`, `:active`, `:focus`

##### UI元素状态伪类

- 概念
  - `:enabled`, `:disabled`, `:checked` 伪类称为 UI 状态伪类
- 兼容性
  - IE9+、FireFox、Chrome、Safari、Opera(`:checked`只兼容Op)

##### CSS3结构类

- CSS3的 `:nth` 选择器
  - 我们把 CSS3 的 `:nth` 选择器也称为CSS3结构类
- **选择方法：**
  - `:first-child` `:last-child` `:nth-child()` `:nth-last-child()` `:nth-of-type()` `:nth-last-of-type()` `:first-of-type` `:last-of-type` `:only-child` `:only-of-type` `:empty`
- `Element:first-child`
  - 概念
    - 选择属于其父元素的首个子元素的每个 Element 元素
  - 兼容性：
    - IE8+、FireFox、Chrome、Safari、Opera
- `Element:last-child`
  - 概念
    - 选择属于其父元素的最后一个子元素的 Element 元素
  - 兼容性：
    - IE8+、FireFox4+、Chrome、Safari、Opera
- `Element:nth-child(N)`
  - 概念
    - 选择属于其父元素的第 N 个子元素，不论元素类型
  - 兼容性：
    - IE9+、FireFox4+、Chrome、Safari、Opera
- **关于参数(N)**
  - `Element:nth-child(Number)` ：
    - 选择属于其父元素的第 Number 个子元素
  - `Element:nth-child(n)` ：
    - **n 是一个简单表达式**，取值从 "0" 开始计算。这里只能是 "n" ，不能用其它字母代替
    - `Element:nth-child(2n+1)`
      - 奇数隔行选择
  - `Element:nth-child(odd)`  `Element:nth-child(even)`：
    - odd 和 even 可用于匹配下表是奇数或偶数的Element元素的关键词（第一个下标是1）
- `:nth-last-child(N)`
  - 概念
    - 选择属于其元素的第 N 个子元素的**每个元素**的类型，不论元素的类型，从最后一个子元素开始计数
  - 兼容性：
    - IE9+、FireFox4+、Chrome、Safari、Opera
- `:nth-of-type(N)`
  - 概念
    - 选择器匹配属于父元素的**特定类型**的第 N 个子元素的每个元素
  - 兼容性：
    - IE9+、FireFox4+、Chrome、Safari、Opera
- `:nth-last-of-type(N)`
  - 概念
    - 选择器匹配属于父元素的**特定类型**的第 N 个子元素的每个元，,从最后一个子元素开始计数
  - 兼容性：
    - IE9+、FireFox4+、Chrome、Safari、Opera
- `:first-of-type`
  - 概念
    - 选择器匹配属于其父元素的特定类型的首个子元素的每个元素
  - 兼容性
    - IE9+、FireFox、Chrome、Safari、Opera
- `:last-of-type`
  - 概念
    - 选择器匹配属于其父元素的特定类型的最后一个子元素的每个元素
  - 兼容性
    - IE9+、FireFox、Chrome、Safari、Opera
- `:only-child`
  - 概念
    - 选择器匹配属于其父元素的子元素的每个元素
  - 兼容性
    - IE9+、FireFox、Chrome、Safari、Opera
- `:only-child-type`
  - 概念
    - 选择器匹配属于其父元素的忒的那个类型的子元素的每个元素
  - 兼容性
    - IE9+、FireFox4+、Chrome、Safari、Opera
- `:empty`
  - 概念
    - 选择器匹配没有子元素（包括文本节点）的每个元素
  - 兼容性
    - IE9+、FireFox、Chrome、Safari、Opera

##### 否定伪类

- 否定选择器 `:not`
  - 概念
    - `:not(Element/ selector)` 选择器匹配非指定元素/选择器的每个元素
  - 语法
    - 父元素:not(子元素/子选择器)  ( Father:not(Children/selector) )
  - 兼容性
    - IE9+、FireFox、Chrome、Safari、Opera

##### 伪元素

- CSS 伪元素用于向某些选择器设置特殊效果
  - 语法
    - 元素::伪元素    ( Element::pseudo-element )
    - "::" 是为了区分伪类，单:也可以用
  - 兼容性
    - IE9+、FireFox、Chrome、Safari、Opera
- `Element::first-line`
  - 概念
    - 根据 "first-line" 伪元素中的样式对 Element 元素的第一行文本进行格式化
  - 说明
    - "first-line" 伪元素只能用于块级元素
- `Element::first-letter`
  - 概念
    - 用于向文本的首字母设置特殊样式
  - 说明
    - "first-letter" 伪元素只能用于块级元素
- `Element::before`
  - 概念
    - 在元素的内容前面插入新内容
  - 说明
    - 常用 "content" 配合使用
    - 行级元素
    - 标签中找不到对应的标签，无法选择
- `Element::after`
  - 概念
    - 在元素的内容后面插入新内容
  - 说明
    - 常用 "content"， 多用于清除浮动
    - 行级元素
    - 标签中找不到对应的标签，无法选择
- `Element::selection`
  - 概念
    - 用于设置在浏览器中选中文本后代背景色与前景色
  - 兼容性
    - IE9+、FireFox加前缀、Chrome、Safari、Opera

#### CSS权重

- 什么是权重
  - 当很多规则别应用到某一个元素上时，权重是决定哪种规则生效、或者优先级的过程
- 权重等级与权值
  - 行内样式(1000) > ID 选择器(100) > **类、属性、伪类选择器(10)** > 元素和伪元素(1) > *(0)
- 权重计算口诀
  - 从0开始，一个行内样式 +1000，一个ID+100，一个属性、class、伪类+10，一个元素名、伪元素+1
- 包含更高权重选择器的一条规则拥有更高的权重
- ID选择器（#idValue）的权重比属性选择器（[id="idValue"]）高
- 带有上下文关系的选择器比单纯的元素选择器权重要高
- 离元素更近的规则生效
- 最后定义的这条规则会覆盖上面与之冲突的规则
- 无论多少个元素组成的选择器，都没有一个 class 选择器权重高
- 通配符选择器权重是0，被继承的CSS属性也带有权重，权重也是0

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

  ![image-20200105112613428](HTML5-imooc.assets\image-20200105112613428.png)

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

#### CSS3 Transform

##### CSS3 的变形（Transform）属性

- 让元素在一个坐标系中变形。这个属性包含一系列变形函数，可以移动、旋转和缩放元素。
- 语法：
  - `transform : none |<transform-funciton> [<transform-function>]*;`
- 默认值：
  - transform: none;
- 兼容性：
  - IE12+、FireFox16+、Chrome36+、Safari16+、Opera23+

#### CSS3 2D转换

##### rotate() 旋转

- 通过指定角度参数对原元素指定一个2D rotation（2D 旋转）
- 语法
  - `transform: rotate(<angle>);`
- 参数说明
  - angle 指旋转角度，正数表示顺时针旋转，负数表示逆时针旋转

##### translate() 平移

- 根据左（X轴）和顶部（Y轴）位置给定的参数，从当前元素位置移动
- 三种情况
  - translateX(x) 仅水平移动（X轴移动）
  - translateY(y) 仅垂直移动（Y轴移动）
  - translate(x, y) 水平和垂直方向同时移动（X轴Y轴同时移动）
- `translateX(<translation-value>);`
  - 语法：X轴移动
    - `transform:translateX(<translation-value>);`
- `translateY(<translation-value>);`
  - 语法：Y轴移动
    - `transform:translateY(<translation-value>);`
- `transform:translate(<translation-value>[,<translation-value>]);`
  - X轴Y轴同时移动

##### scale() 缩放

- 指定对象的2D scale（2D缩放）
- 三种情况
  - scaleX(x) 仅水平缩放（X轴缩放）
  - scaleY(y) 仅垂直缩放（Y轴缩放）
  - scale(x, y) 水平和垂直方向同时缩放（X轴Y轴同时缩放）
- `scaleX(<number>)`
  - 使用 [sx, 1] 缩放矢量执行缩放操作，sx 为所需参数
  - 语法
    - `transform: scaleX(<number>);`
- `scaleY(<number>)`
  - 使用 [sy, 1] 缩放矢量执行缩放操作，sy 为所需参数
  - 语法
    - `transform: scaleY(<number>);`
- `scale(<number>[, <number>])`
  - 使用 [sx, sy] 缩放矢量的两个参数指定一个 2D scale（2D缩放）
  - 语法
    - `transform: scale(<number>[, <number>]);`

##### skew() 扭曲或斜切

- 指定对象skew transformation（斜切扭曲）
- 三种情况
  - skewX(x) 仅水平扭曲变形（X轴扭曲变形）
  - skewY(y) 仅垂直扭曲变形（Y轴扭曲变形）
  - skew(x, y) 水平和垂直方向同时扭曲变形（X轴Y轴同时扭曲变形）
- `skewX(<angle>)`
  - 水平斜切变换（X轴扭曲变形）
  - 语法
    - `transform: skewX(<angle>);`
- `skewY(<angle>)`
  - 垂直斜切变换（Y轴扭曲变形）
  - 语法
    - `transform: skewY(<angle>);`
- `skew(<angle>[,<angle>])`
  - skew(x, y) 水平和垂直方向同时斜切变换（X轴Y轴同时扭曲变形）
  - 语法
    - `transform: skew(<angle>[,<angle>]);`

##### matrix() 矩阵或混合

- 以一个含六个值的(a,b,c,d,e,f) 变换矩阵的形式指定一个2D变换
- 相当于直接应用一个[a,b,c,d,e,f] 变换矩阵
- 语法
  - `transform: matrix(a, c, b, d, tx, ty);`
- 参数说明
  - tx, ty 就是基于X和Y坐标重新定位元素

#### CSS3 3D转换

##### rotate3d()

- 旋转rotateX
  - 指定对象在X轴上的旋转角度
  - 语法
    - `transform: rotateX(angle);`
- 旋转rotateY
  - 指定对象在Y轴上的旋转角度
  - 语法
    - `transform: rotateY(angle);`
- 旋转rotateZ
  - 指定对象在Z轴上的旋转角度
  - 语法
    - `transform: rotateZ(angle);`
- 旋转rotate3d
  - 指定对象在X轴上的旋转角度
  - 语法
    - `transform: rotateX(x, y, z, angle);`
  - 参数说明
    - 前三个参数分别表示方向，第四个表示旋转的角度，参数不允许省略
    - x,y,z 取值0~1 可以为小数0.01

##### translate3d()

- 移动 translateZ
  - 指定对象Z轴的平移
  - 语法
    - `transform: translateZ(z);`
  - 参数说明
    - 参数对应Z轴，不能省略
- 移动 translate3d
  - 指定对象的3d位移
  - 语法
    - `transform: translate3d(x, y, z);`
  - 参数说明
    - 参数对应X,Y,Z轴，不能省略

##### scale3d()

- 缩放 scaleZ
  - 指定对象的z 轴缩放
  - 语法
    - `transform: scaleZ(z);`
  - 参数说明
    - 参数对应Z轴，参数不能省略
- 缩放 scale3d
  - 指定对象的3d缩放
  - 语法
    - `transform: scale3d(x, y, z);`
  - 参数说明
    - 参数对应X,Y,Z轴，不能省略

##### matrix3d()

- 矩阵 matrix3d
  - 以一个4x4矩阵的形式指定一个3D变换
  - 语法
    - `transform: matrix3d(sx, n,n,n,n, sy, n,n,n,n, sz, n,n,n,n, 1);`
  - 参数说明
    - 使用 16个值得 4x4 矩阵

#### CSS3 Transform与坐标系统

- transform-origin 属性
  - 更改转换元素的位置(原点)
  - 语法
    - `transform-origin: x-axis y-axis z-axis;`

#### CSS3 矩阵

- 矩阵的概念
  - 矩阵可以理解为方阵，方阵中站的是人，矩阵中是数值。所谓的矩阵计算就是两个方针的人相互冲杀。
- CSS3 中的矩阵
  - CSS3 中的矩阵指的是一个方法，书写为 matrix() 和 matrix3d()；
  - matrix 是元素2D平面的移动变换（transform），2D变换矩阵为 3x3；
  - matrix3d 是元素3D 移动变换（transform），3D变换矩阵为 4x4；

##### 矩阵matrix

- `transform: matrix(a, c, d, tx, ty);`
  - 注意书写方向是竖直方向
- 转换公式
  - x, y 表示转换元素的所有坐标
- 目标矩阵说明
  - `ax + cy + e` 为变换后的水平坐标，`bx + dy + f` 表示变换后的垂直位置

![image-20200106150408525](HTML5-imooc.assets\image-20200106150408525.png)

##### 矩阵matrix 举例

- ```css
  transform: matrix(1, 0, 0, 1, 30, 30); /* a=1, b=0, c=0, e=30, f=30 */
  根据这个矩阵偏移元素的中心点
  假设是(0, 0)，即 x=0, y=0;
  变换后，
  x = ax + cy + e = 1*0 + 0*0 + 30 = 30;
  y = bx + dy + f = 0*0 + 0*1 + 30 = 30;
  
  于是，整个元素的中心点从(0,0) 变成了(30,30)
  整个元素就发生了平移
  ```

- 说明

  - ```css
    transform: matrix(1, 0, 0, 1, 30, 30); 
    等同于 transform: translate(x,y);
    ```

- 注意

  - matrix 在 FF 浏览器下需要添加单位，webkit 内核默认px，translate 等方法需要加单位

##### 矩阵matrix缩放(scale)

- ```css
  matrix(sx,0,0,sy,0,0) 等同于 scale(sx,sy)
  ```

##### 矩阵matrix旋转(rotate)

- ```css
  matrix(cosθ,sinθ,-sinθ,cosθ,0,0) 等同于 rotate(θdeg)
  ```

##### 矩阵matrix拉伸(skew)

- ```css
  matrix(1,tanθy,tanθx,1,0,0) 等同于 skew(θxdeg,θydeg)
  ```

##### 矩阵matrix镜像对称效果

- ```css
  matrix((1-k*k)/(1+k*k),2k/(1+k*k),2K/(1+k*k),(k*k-1)/(1+k*k),0,0)
  ```

  对称轴一定通过元素变换的中心点，k是对称轴的斜率

  ![image-20200106154232828](HTML5-imooc.assets\image-20200106154232828.png)

##### 3D变换中的矩阵

- 从二维变到三维，是从 4到 9；而在矩阵里头是从 3\*3 变成 4\*4

- 例子：

  ```css
  transform: matrix3d(sx,0,0,0,0,sy,0,0,0,0,sz,0,0,0,0,1)
  ```

  ![image-20200106155507645](HTML5-imooc.assets\image-20200106155507645.png)

#### CSS3 扩展属性

##### transform-style属性

- 指定嵌套元素是怎么样在三维空间中呈现

- 语法
  - `transform-style: flat|preserve-3d;`
- 默认值
  - `transform-style: flat;`

##### perspective属性

- 指定观察者与 [z=0] 平面的距离，使具有三维位置变换的元素产生透视效果
- 语法
  - `perspective: number|none; `
- 默认值
  - `perspective: number|none;`

##### perspective-origin属性

- 指定透视点的位置
- 语法
  - `perspective-origin: x-axis y-axis; `
- 默认值
  - `perspective: 50% 50%;`

##### backface-visibility属性

- 指定元素背面面向用户时是否可见
- 语法
  - `backface-visibility: visible|hidden; `
- 默认值
  - `perspective: visible;`

### 第5课 CSS3过渡

		CSS3过渡
		一起探索如何通过CSS3属性值的变化实现动画效果，如何触发这些动画产生交互

#### 过渡（Transition）

- 允许CSS的属性值在一定事件区间内平滑的变化
- 在鼠标点击、获得焦点、被点击或对元素任何改变中触发，并圆滑的以动画效果改变CSS的属性值
- 兼容性
  - IE10+、FireFox16+、Chrome26+、Safari6.1+、Opera12.1+

#### transform-property属性

- 检索或设置对象中的参与过渡的属性
- 语法
  - `transform-property:none|all|"property";`
- 参数说明
  - none（没有属性改变）
  - all （所有属性改变）
  - "property"（元素属性名）
- 默认所有属性过渡

#### transition-furation属性

- 检索或设置对象过渡的持续时间
- 语法
  - `transition-duration:time;`
- 参数说明
  - 规定完成过渡效果需要花费的时间（以秒或毫秒计算）
  - 默认值 0

#### transition-timing-function属性

- 检索或设置对象中过渡的动画类型

- 语法

  - ```css
    transition-timing-funxtion:ease|linear|ease-in|oase-out|ease-in-out|step-start|step-end|steps(<integer>[,[start|end]]?)|cubic-bezier(<number>,<number>,<number>,<number>);	
    ```

- 参数说明

  - linear：线性过渡。等同于贝塞尔曲线(0.0, 0.0, 1.0, 1.0)
  - ease：平滑过渡。等同于贝塞尔曲线(0.25, 0.1, 0.25, 1.0)
  - ease-in：由慢到快。等同于贝塞尔曲线(0.41, 0, 1.0, 1.0)
  - ease-out：由快到慢。等同于贝塞尔曲线(0, 0, 0.58, 1.0)
  - ease-in-out：由慢到快再到慢。等同于贝塞尔曲线(0.42, 0, 0.58, 1.0)
  - step-start：等同于 steps(1, start)
  - step-end：等同于 steps(1, end)
  - `steps(<integer>[,[start|end]]?)`：接受两个参数的步进函数
    - 第一个参数：必须为正整数，指定函数的步数
    - 第二个参数：取值可能是start或end，指定每一步的值发生变化的时间点
    - 第二个参数：可选，默认值为end
  - `cubic-bezier(<number>,<number>,<number>,<number>);`
    - 特定的贝塞尔曲线类型，4个数值需在[0,1] 区间内

#### transition-delay属性

- 检索或设置对象延迟过渡的时间
- 语法
  - `transition-delay:time;`
- 参数说明
  - 指定秒或毫秒之前要等待切换效果开始
  - 默认值 0

#### transition属性

- **复合属性**检索或设置对象变换时的过渡
- 语法
  - `transition: property duration timing-function delay;`



### 第6课 CSS3动画

		CSS3动画
		使用animation属性，实现以往要用Flash等动画软件才能完成的炫酷效果

#### CSS3动画(animation)

- 动画(animation)
  - anima：灵魂
  - animate：赋予生命
  - 动画可以定义为使用绘画手法，创造生命运动的艺术
- 视觉暂留原理
  - 人类具有”视觉暂留“ 的特性，人的眼睛看到一幅画或一个物体后，再0.34秒内不会消失。
- 动画原理
  - 通过把人物的表情、动作、变化等分解后画成许多动作瞬间的画面，利用视觉暂留的原理，再上一幅画还没消失前播放下一幅画，就会给人造成一种流畅的视觉变化效果。
- 兼容性
  - IE10+、FireFox16+、Chrome43+、Safari9+、Opera30+、Android(-webkit-)
- CSS 动画
  - 使元素从一种样式逐渐变化称为另一种样式的效果

#### CSS3 animation

##### animation-name属性

- 检索或设置对象所应用的动画名称
- 语法
  - `animation-naem:keyframename|none;`
- 参数说明
  - keyframename：指定要绑定到选择器的关键帧的名称
  - none：指定没有动画（可用于覆盖从级联的动画）

##### animation-duration属性

- 检索或设置对象动画的持续时间
- 语法
  - `animation-duration:time;`
- 参数说明
  - time 指定动画播放完成花费的时间。默认值为 0，意味着没有动画效果

##### animation-timing-function属性

- 检索或设置对象动画的过渡类型

- 语法

  - ```css
    animation-timing-funxtion:ease|linear|ease-in|oase-out|ease-in-out|step-start|step-end|steps(<integer>[,[start|end]]?)|cubic-bezier(<number>,<number>,<number>,<number>);	
    ```

- 参数说明

  - linear：线性过渡。等同于贝塞尔曲线(0.0, 0.0, 1.0, 1.0)
  - ease：平滑过渡。等同于贝塞尔曲线(0.25, 0.1, 0.25, 1.0)
  - ease-in：由慢到快。等同于贝塞尔曲线(0.41, 0, 1.0, 1.0)
  - ease-out：由快到慢。等同于贝塞尔曲线(0, 0, 0.58, 1.0)
  - ease-in-out：由慢到快再到慢。等同于贝塞尔曲线(0.42, 0, 0.58, 1.0)
  - step-start：等同于 steps(1, start)
  - step-end：等同于 steps(1, end)
  - `steps(<integer>[,[start|end]]?)`：接受两个参数的步进函数
    - 第一个参数：必须为正整数，指定函数的步数
    - 第二个参数：取值可能是 start或 end，指定每一步的值发生变化的时间点
    - 第二个参数：可选，默认值为 end
  - `cubic-bezier(<number>,<number>,<number>,<number>);`
    - 特定的贝塞尔曲线类型，4个数值需在[0,1] 区间内

##### animation-delay属性

- 检索或设置对象动画的延迟时间
- 语法
  - `animation-delay:time;`
- 参数说明
  - 可选，定义动画开始前等待的时间。
  - 默认值 0

##### animation-iteration-count属性

- 检索或设置对象动画的循环次数
- 语法
  - `animation-iteration-count:infinite|<number>;`
- 参数说明
  - `<number>`为数字，其默认值为 "1" ；infinite 为无限次数循环。

##### animation-direction属性

- 检索或设置对象动画再循环中是否反方向运动
- 语法
  - `animation-direction:normal|reverse|alternate|alternate-reverse|initial|inherit;`
- 参数说明
  - normal：正常方向；
  - reverse：反方向运行；
  - alternate：动画先正常运行再反方向运行，并持续交替运行；
  - alternate-reverse：动画先反方向运行再正方向运行，并持续交替运行。

##### animation-fill-mode属性

- 规定动画不播放时（当动画完成播放或当动画有延迟未开始播放时），要应用到元素的样式。
- 语法
  - `animation-fill-mode:none|forwards|backwards|both|initial|inherit;`
  - 参数说明
    - none：默认值。不设置对象动画之外的状态；
    - forwards：设置对象状态为动画开始时的状态；
    - backwards：设置对象状态为动画开始时的状态；
    - both：设置对象状态为动画结束或开始的状态。

##### animation-play-state属性

- 指定动画是否正在运行或已暂停
- 语法
  - `animation-play-state:paused|running;`
- 参数说明
  - paused：指定暂停动画；
  - running：默认值，指定正在运行的动画。

##### animation属性

- 复合属性。检索或设置对象所应用的动画特效。

- 语法：优先识别 name duration

  - ```css
    animation:name duration timing-function delay iteration-count direction fill-mode plat-state;
    ```

#### CSS3 @keyframes

- Keyframes定义

  - 关键帧，可以指定任何顺序排列来决定Animation动画变化的关键位置

- 使用说明

  - 使用@keyframes规则创建动画，通过逐步改变从一个CSS样式设定到另一个。
  - 再动画过程中可以通过@keyframes规则多词更改CSS样式的设定。

- 语法

  - ```css
    @keyframse animationname { 
      keyframes-selector{
     		css-style;   
      }
    }
    ```

- 参数说明

  - animationname：必写项，定义animation的名称。
  - keyframes-selector：必写项，动画持续时间的百分比，0-100%、from(代替：0%)、to(代替：100%)
  - css-style：必写项，一个或多个合法的CSS样式属性

#### CSS3 will-change

- 目标
  - 增强页面渲染性能
- CPU和GPU
  - CPU即中央处理器，解释计算机指令以及处理计算机软件中的数据。
  - GPU即图形处理器，专门处理和绘制图形相关的硬件。GPU时专为执行复杂的数学和几何计算而设计的，有了它，CPU就从图形处理的认为u中解放出来，可以执行其它更多的系统任务。
- 硬件加速
  - 在计算机中把计算量非常大的工作分配给专门的硬件来处理，减轻CPU的工作量。
- 现状
  - CSS的动画、变形、渐变并不会自动触发GPU加速，而是使用里浏览器稍慢的软件软件渲染引擎。
  - 在transition，transform和animation的世界里，应用卸载进程到GPU以加快速度。
  - 只有3D变形会有自己的layer，2D变形不会。

##### translateZ() （or translate3d()）Hack

- 为元素添加没有变化的3D变形，骗取浏览器触发硬件加速。

- 代价
  - 这种情况通过向他自己的层叠加元素，占用RAM和GPU储存空间。

##### will-change

- 提前通知浏览器元素将要做什么动画，让浏览器提前准备合适的优化设置。

- 语法

  - ```css
    will-change:auto|scroll-position|contents|<custom-ident>|<animateable-frature>;
    ```

- 兼容性

  - IE13+、FireFox47+、Chrome49+、Safari9.1+、Opera39+、IOS9.3+、Android52+

- 关键词说明

  - auto：此关键词表示没有特定的意图，适用于它通常所做的任何启发式和优化。
  - scroll-position：表示将要改变元素的滚动位置。
  - centents：表示将要改变元素的内容。
  - `<custom-ident>`：明确指定将要改变的属性与给定名称。
  - `<animateable-feature>`：可动画的一些特征值，比如left、top、margin等。

- 注意

  - 勿滥用、提前声明、remove。

### 第7课 多列

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

### 第8课 CSS3图片切换特效

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

![image-20200108140019028](HTML5-imooc.assets\image-20200108140019028.png)

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
#### 学习内容

- 前端开发流程以及必要的工具使用
- HTML5的标签、标签的结构：BEM开发模式
- CSS3、CSS过渡动画、帧动画
- JS元素的获取、事件响应处理
- 通过学习，能独立承担工作中前端开发的角色

#### 前端开发流程

1. 需求分析（产品经理）
2. 视觉设计、交互动画设计（视觉交互）
3. 前端静态页开发、动态效果开发（前端开发）

#### 相关工具

- 编辑器：Sublime3
- 标注工具：PxCook
- 切图工具：Photoshop

#### 静态页具体流程

1. 视觉设计稿.psd
2. 标注颜色、行高、字体、大小
3. PS切图
4. 合并图片：雪碧图 (使用在线工具合并)
5. BEM开发模式
   - BEM代表块（Block），元素（Element），修饰符（Modifier）
   - BEM设计模式：
     - 模块(没有前缀，多个单词用 - 连接)
     - 元素(元素在模块之后，可以多个层级，以 __ 连接)
   - 先想好CSS样式名称，再填入HTML标签

#### 动态页面开发

##### 用到的CSS3新特性

- 新的选择器，如：div:last-child
- 多列布局，如：-webkit-column-count:3
- 圆角：border-radius
- transform：位置变动
- transitions：过渡效果
- animation：动画效果

##### 让元素动起来

- 动画样式约定
- 动画测试页面，事件模拟

