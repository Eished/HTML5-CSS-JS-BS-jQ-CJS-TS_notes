# HTML/CSS-W3school+MDN

## 基础教程

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

