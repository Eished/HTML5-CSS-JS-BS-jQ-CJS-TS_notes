# HTML/CSS-W3school+MDN+w3cplus

## 基础教程

> [css现状和如何学习](https://w3cplus.medium.com/css%E7%8E%B0%E7%8A%B6%E5%92%8C%E5%A6%82%E4%BD%95%E5%AD%A6%E4%B9%A0-1ac786328761)

CSS称为 **层叠样式表，**即是 Cascade Style Sheets三个词的首字母缩写。每个字母代表的含义不同：

- **C（Cascade）：**指的是层叠，在CSS中编写样式规则是一个一个排列下来，可以简单的理解为先后顺序
- **S（Style）** : 第一个S，它指的是样式规则，比如 `body{color: red}`
- **S（Sheets）** ：第二个S，它指的是样式表，就是我们常说的 `.css` 文件，CSS的代码会放置在样式表里

前面提到过，Web页面至少由HTML、CSS和JavaScript三个部分构成，其中HTML会经过HTML Parser将HTML结构转换成[**DOM Tree**](https://www.w3cplus.com/javascript/dom-tree-and-traversals.html)；CSS会经过CSS Parser将CSS转换成[**CSSOM Tree**](https://www.w3cplus.com/javascript/cssom-css-typed-om.html)，正如下图所示：

DOM树和CSSOM树将会构建出渲染树：

![image-20210829212219883](HTML-CSS-W3school+MDN.assets/image-20210829212219883.png)

如果再把AOM（可访问树）引入起来的话，大致就像下图这样：

![image-20210829212347485](HTML-CSS-W3school+MDN.assets/image-20210829212347485.png)

“CSS样式要和相应的HTML元素结合在一起使用，才能在浏览器渲染出来，呈现给用户”。

![image-20210829212636474](HTML-CSS-W3school+MDN.assets/image-20210829212636474-16302435971191.png)

### CSS中的层叠：

- 文档流（Normal Flow）
- 格式化上下文（Formatting Context）
- 层叠上下文（Stacking Context）
- 层叠水平（Stacking Level）
- 层叠顺序（Stacking Order）

#### 文档流（Normal Flow）

- 很多时候她被称为Document Flow，但在CSS的标准被称为Normal Flow，即普通流或常规流。大家更喜欢称之为文档流。
- 除非文档的尺寸被CSS规则限定，否则浏览器垂直扩展文档来容纳全部的内容。每个新的块级元素渲染为新行。行内元素则按照顺序被水平渲染直到当前行遇到边界，然后换到下一行垂直渲染。
- 普通文档流中的盒子属于一种**格式化上下文（Formatting Context）**
  - **块格式化上下文（Block formatting context）**
  - **行内格式化上下文（Inline formatting context）**
  - 任何被渲染的HTML元素都是一个盒子（Box），这些盒子不是块盒子就是行内盒子。

格式化上下文对元素盒子做了一定的范围的限制，**普通流的过程：**

- 块级元素按照其在HTML源码中出现的顺序，在其容器盒子里从左上角开始，从上到下垂直地依次分配**空间层叠（Stack）**，并且独占一行，边界紧贴父盒子边缘。
- 两相邻元素间的距离由margin属性决定，在同一个块格式化上下文中的垂直边界将被**重叠（Collapse margins）**。
- 除非创建一个新的块格式化上下文，否则块级元素的宽度不受浮动元素的影响。
- 在对应的行内格式化上下文中，行内元素从容器的顶端开始，一个接一个地水平排列。

#### 格式化上下文（Formatting Context）

初始元素定义的环境
- 其主要包含两个要点，一个是 **元素定义的环境** ，另一个是 **初始化**。

我们使用[**CSS的** ](https://www.w3cplus.com/css/web-layout-css-display.html)`display`[ **属性**](https://www.w3cplus.com/css/web-layout-css-display.html)可以对元素进行格式化，即 **创建格式化上下文** 。

![0_L2N2kTjgtOvGlY5h](HTML-CSS-W3school+MDN.assets/0_L2N2kTjgtOvGlY5h.png)

设置了 `display: contents` 会改变原有的格式，即`ul`子元素 `li` 都会变成网格项目。

#### 层叠上下文

平时我们从设备终端看到的HTML文档都是一个平面的，事实上HTML文档中的元素却是存在于三个维度中。除了大家熟悉的平面画布中的 `x` 轴和 `y` 轴，还有控制第三维度的`z`轴。

![image-20210829221011478](HTML-CSS-W3school+MDN.assets/image-20210829221011478.png)

> 在DOM树中最先出现的元素被放在首位，之后出现的元素被放在前面的元素之上。但它并不总是那么简单。只有当页面上的所有元素是自然流才起作用。也就是说，当没有元素在流中的位置被改变或者已经脱离文档流，才起作用。

- 每个HTML元素都属于一个层叠上下文。
- 给定层叠上下文中的每个定位元素都具有一个整数的层叠层级，具有更大堆栈级别的元素盒子总是在具有较低堆栈级别的盒子的前面（上面）。
- 盒子可能具有负层叠级别。
- 层叠上下文中具有相同堆栈级别的框根据文档树出现的顺序层叠在一起。

文档中的层叠上下文由满足以下任意一个条件的元素形成：

- 根元素 (HTML)
- `z-index` 值不为 `auto` 的 `position` 值为非 `static` 。
- `position` 值为非 `static`
- 一个 `z-index` 值不为 `auto` 的 Flex 项目 (Flex item)，即：父元素 `display: flex|inline-flex`
- `opacity` 属性值小于 `1` 的元素
- `transform` 属性值不为 `none` 的元素
- `mix-blend-mode` 属性值不为 `normal` 的元素
- `filter` 、 `perspective` 、 `clip-path` 、 `mask` 、 `motion-path` 值不为 `none` 的元素
- `perspective` 值不为 `none` 的元素
- `isolation` 属性被设置为 `isolate` 的元素
- 在 `will-change` 中指定了任意 CSS 属性，即便你没有直接指定这些属性的值

每个页面都有一个默认的层叠上下文。这个层叠上下文的根就是 `html` 元素。 `html` 元素中的一切都被置于这个默认的层叠上下文的一个层叠层上。

#### 层叠水平（Stacking Level）

层叠水平（Stacking Level）决定了**同一个层叠上下文中**元素在z轴上的显示顺序。

普通元素的层叠水平优先由层叠上下文决定，因此，层叠水平的比较只有在当前层叠上下文元素中才有意义。

- **注意**：不要把**层叠水平**和CSS的 `z-index` 属性混为一谈。
  - 没错，某些情况下 `z-index` 确实可以影响层叠水平，但是，只限于定位元素以及Flex盒子的孩子元素；
  - 而层叠水平所有的元素都存在。

#### 层叠顺序（Natural Stacing Order）

在HTML文档中，默认情况之下有一个**自然层叠顺序（Natural Stacing Order）**，即元素在 `z` 轴上的顺序。它是由许多因素决定的。

比如下面这个列表，它显示了元素盒子放入层叠顺序上下文的顺序，从层叠的底部开始，共有七种层叠等级：

- 背景和边框：形成层叠上下文的元素的背景和边框。 层叠上下文中的最低等级。
- 负 `z-index` 值：层叠上下文内有着负 `z-index` 值的子元素。
- 块级盒：文档流中非行内非定位子元素。
- 浮动盒：非定位浮动元素。
- 行内盒：文档流中行内级别非定位子元素。
- `z-index: 0` ：定位元素。 这些元素形成了新的层叠上下文。
- 正 `z-index` 值：定位元素。 层叠上下文中的最高等级。

![image-20210829222708063](HTML-CSS-W3school+MDN.assets/image-20210829222708063.png)

这七个层叠等级构成了层叠次序的规则。 

在层叠等级七上的元素会比在等级一至六上的元素显示地更上方（更靠近观察者）。 

![image-20210829222808206](HTML-CSS-W3school+MDN.assets/image-20210829222808206.png)

其实对于层叠顺序规则还是较为复杂的。

当页面包含浮动元素、绝对定位的元素、固定定位的元素或相对定位的元素（元素从正常位置偏移一定量）以及内联元素时，浏览器会以不同的方式显示它们（放置它们）。

元素从最靠近查看者的地方排列到最远的地方，如下所示：

![image-20210829223329293](HTML-CSS-W3school+MDN.assets/image-20210829223329293.png)

- 定位元素按源代码中的外观顺序排列。源代码中的最新内容最接近查看者
- 内联元素（比如文本和图像）是流入和非定位（它们的位置是静态的）
- 非浮动元素按照源代码中外观的顺序排列
- 非定位和非浮动块级元素
- 根元素 `html` 是全局层叠上下文的根，包含页面上的所有元素

这就是浏览器在呈现页面上的元素时应用的默认层叠顺序。

 **`z-index` 属性只适用于定位元素。**

具有除 `static` 之外的 `position` 值。

因此，如果所有定位的元素具有z-index的索引值，则将元素从最靠近查看者排列到最远的位置，如下所示：

具有正值的 `z-index` 的定位元素。较高的值更接近屏幕。然后，按照它们出现在源代码中的顺序排列：

![image-20210829224151106](HTML-CSS-W3school+MDN.assets/image-20210829224151106.png)

- 定位元素的 `z-index:0` 或 `z-index: auto` ;
- 内联元素（如文本和图像）是流中的和非定位的（它们的位置是静态的）
- 源代码中出现顺序的非定位浮动元素
- 非定位和非浮动块级元素
- 具有负值的 `z-index` 的定位元素。较低的 `z-index` 索引值更近。然后按照它们在源代码中出现的顺序
- 根元素 `html` 是全局层叠上下文的根，包含页面上的所有元素

当我们在定位元素上设置 `z-index` 值时，它指定该元素在它所属的**层叠顺序上下文**中的顺序，并且它将根据上述步骤在屏幕上渲染。

#### 样式层叠

### 权重

### 继承

### 视觉格式化模型

#### 行内格式化上下文

#### 块格式化上下文

#### Flex格式化上下文

#### Grid格式化上下文

### 盒模型

### 布局

### 写CSS的姿势

### 如何学习CSS

### 选择器

[选择器相关笔记 HTML5-imooc.md](HTML5-imooc.md)

#### 并列类或标签选择器

两个选择器之间无空格。

```css
<ul>
  <li>项目一</li>
  <li class="special">项目二</li>
  <li>项目 <em>三</em></li>
  <span class="special">项目二</span>
</ul>


li.special {
  color: orange;
  font-weight: bold;
}
```

这个意思是说，“选中每个 `special` 类的 `li` 元素”。

并列选择：

```css
li.special,
span.special {
  color: orange;
  font-weight: bold;
}
```

#### 包含选择符

在两个选择器之间加上一个空格。

该选择器将选择`<li>`内部的任何`<em>`元素（`<li>`的后代）。

```css
li em {
  color: rebeccapurple;
}
```

#### 相邻兄弟元素选择器

元素 + 相邻兄弟元素 (Element + Sibling )

在两个选择器之间添加一个 `+` 号

```css
h1 + p {
  font-size: 200%;
}
```

```html
<h1>I am a level one heading</h1>

<p>This is a paragraph of text. In the text is a <span>span element</span> 
and also a <a href="#">link</a>.</p>

<p>This is the second paragraph. It contains an <em>emphasized</em> element.</p>

<ul>
    <li>Item <span>one</span></li>
    <li>Item two</li>
    <li>Item <em>three</em></li>
</ul>
```

#### 根据状态确定样式

```css
a:link {
  color: pink;
}

a:visited {
  color: green;
}
```

#### [专一性](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/First_steps/How_CSS_is_structured#专一性)

CSS语言有规则来控制在发生碰撞时哪条规则将获胜--这些规则称为**级联规则和专用规则**。

后面的样式覆盖前面的同名样式。

在我们使用类选择器和元素选择器的早期块中，类将获胜。

#### 权重等级与权值：

- 行内样式(1000) > ID 选择器(100) > **类、属性、伪类选择器(10)** > 元素和伪元素(1) > `*(0)`

### float

脱离文档流，不脱离文本流。

图文环绕使用。

对自身的影响：

- BFC（Block format context，块级格式化上下文），形成块
- 靠上、靠左

对兄弟节点影响：

- 上面贴非 float 元素
- 旁边贴 float 元素
- 不影响其它块级元素位置
- 影响其它块级元素內部文本

对父级元素的影响：

- 从布局上“消失”
- 高度塌陷
  - `overflow:auto`

## 中级教程

### CSS 布局 - display 属性

`display` 属性规定是否/如何显示元素。

每个 HTML 元素都有一个默认的 display 值，具体取决于它的元素类型。大多数元素的默认 display 值为 block 或 inline。

#### 块级元素（block element）

块级元素总是从新行开始，并占据可用的全部宽度（尽可能向左和向右伸展）。

- `<div>`
- `<h1> - <h6>`
- `<p>`
- `<form>`
- `<header>`
- `<footer>`
- `<section>`

#### 行内元素（inline element）

内联元素不从新行开始，仅占用所需的宽度。

- `<span>`
- `<a>`
- `<img>`

#### Display: none;

每个元素都有一个默认 display 值。

#### 隐藏元素 - display:none 还是 visibility:hidden？

`display:none`：该元素将被隐藏，并且页面将显示为好像该元素不在其中。

`visibility:hidden`：该元素仍将占用与之前相同的空间。元素将被隐藏，但仍会影响布局。

#### CSS display 属性值

| 值                 | 描述                                                         |
| :----------------- | :----------------------------------------------------------- |
| none               | 此元素不会被显示。                                           |
| block              | 此元素将显示为块级元素，此元素前后会带有换行符。             |
| inline             | 默认。此元素会被显示为内联元素，元素前后没有换行符。         |
| inline-block       | 行内块元素。（CSS2.1 新增的值）                              |
| list-item          | 此元素会作为列表显示。                                       |
| run-in             | 此元素会根据上下文作为块级元素或内联元素显示。               |
| compact            | CSS 中有值 compact，不过由于缺乏广泛支持，已经从 CSS2.1 中删除。 |
| marker             | CSS 中有值 marker，不过由于缺乏广泛支持，已经从 CSS2.1 中删除。 |
| table              | 此元素会作为块级表格来显示（类似 `<table>`），表格前后带有换行符。 |
| inline-table       | 此元素会作为内联表格来显示（类似 `<table>`），表格前后没有换行符。 |
| table-row-group    | 此元素会作为一个或多个行的分组来显示（类似 `<tbody>`）。     |
| table-header-group | 此元素会作为一个或多个行的分组来显示（类似 `<thead>`）。     |
| table-footer-group | 此元素会作为一个或多个行的分组来显示（类似 `<tfoot>`）。     |
| table-row          | 此元素会作为一个表格行显示（类似 `<tr>`）。                  |
| table-column-group | 此元素会作为一个或多个列的分组来显示（类似 `<colgroup>`）。  |
| table-column       | 此元素会作为一个单元格列显示（类似 `<col>`）                 |
| table-cell         | 此元素会作为一个表格单元格显示（类似 `<td>` 和 `<th>`）      |
| table-caption      | 此元素会作为一个表格标题显示（类似 `<caption>`）             |
| inherit            | 规定应该从父元素继承 display 属性的值。                      |

#### [`display` 的各个取值](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display#%E6%8C%87%E5%8D%97%E5%92%8C%E7%A4%BA%E4%BE%8B)

##### [CSS Flow Layout (`display: block`, `display: inline`)](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display#css_flow_layout_display_block_display_inline)

##### [`display: flex`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display#display_flex)

##### [`display: grid`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display#display_grid)

##### [`display: none;`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display#display_none)

将 `display` 设置为 `none` 会将元素从 [可访问性树 *accessibility tree*](https://developer.mozilla.org/zh-CN/docs/Learn/Accessibility/What_is_accessibility#accessibility_apis) 中移除。这会导致该元素及其所有子代元素不再被屏幕阅读技术 *screen reading technology* 访问。

如果你只是想从视觉上隐藏这个元素，对可访问性更加友好的做法是使用 [属性组合](https://gomakethings.com/hidden-content-for-better-a11y/#hiding-the-link) 来将其从屏幕上隐藏，但仍可以被屏幕阅读器 *screen readers* 等辅助技术解析。

##### [`display: contents;`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/display#display_contents)

当前大多数浏览器对 `display: contents;` 的实现是：将设置了该值的元素从 [可访问性树 *accessibility tree*](https://developer.mozilla.org/zh-CN/docs/Learn/Accessibility/What_is_accessibility#accessibility_apis) 中移除，但保留其子代元素。这会导致该元素自身不再被屏幕阅读技术 *screen reading technology* 访问。这在 [CSS 规范](https://drafts.csswg.org/css-display/#valdef-display-contents) 中被视为不正确的行为。





## 高级教程



## 响应式设计

在不同设备上正常使用

- 一般主要处理屏幕大小问题

主要方法

- 隐藏+折行+自适应空间
- rem/viewport/media query

## 网格布局

