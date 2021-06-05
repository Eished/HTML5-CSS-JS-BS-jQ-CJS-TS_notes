# [VS Code 快捷键（中英文对照版）](https://segmentfault.com/a/1190000007688656)

[visual-studio-code](https://segmentfault.com/t/visual-studio-code)

 阅读约 14 分钟

> 本文为 Visual Studio Code [Keyboard Shortcuts Windows](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf) 翻译版。
> 与官网同步更新，如未及时更新欢迎指正提醒，也欢迎大家关注我的专栏。
> 本文翻译版权归作者本人所有，在 **注明出处并附上原文链接** 的情况下可自由转载。

## 常用 General

| 按 Press             | 功能 Function                       |
| -------------------- | ----------------------------------- |
| Ctrl + Shift + P，F1 | 显示命令面板 Show Command Palette   |
| Ctrl + P             | 快速打开 Quick Open                 |
| Ctrl + Shift + N     | 新窗口/实例 New window/instance     |
| Ctrl + Shift + W     | 关闭窗口/实例 Close window/instance |
| Ctrl + ,             | 用户设置 User Settings              |
| Ctrl + K Ctrl + S    | 设置键盘快捷方式 Keyboard Shortcuts |

## 基础编辑 Basic editing

| 按 Press             | 功能 Function                                               |
| -------------------- | ----------------------------------------------------------- |
| Ctrl + X             | 剪切行（空选定） Cut line (empty selection)                 |
| Ctrl + C             | 复制行（空选定）Copy line (empty selection)                 |
| Alt + ↑ / ↓          | 向上/向下移动行 Move line up/down                           |
| Shift + Alt + ↓ / ↑  | 向上/向下复制行 Copy line up/down                           |
| Ctrl + Shift + K     | 删除行 Delete line                                          |
| Ctrl + Enter         | 在下面插入行 Insert line below                              |
| Ctrl + Shift + Enter | 在上面插入行 Insert line above                              |
| Ctrl + Shift + \     | 跳到匹配的括号 Jump to matching bracket                     |
| Ctrl + ] / [         | 缩进/缩进行 Indent/outdent line                             |
| Home                 | 转到行首 Go to beginning of line                            |
| End                  | 转到行尾 Go to end of line                                  |
| Ctrl + Home          | 转到文件开头 Go to beginning of file                        |
| Ctrl + End           | 转到文件末尾 Go to end of file                              |
| Ctrl + ↑ / ↓         | 向上/向下滚动行 Scroll line up/down                         |
| Alt + PgUp / PgDown  | 向上/向下滚动页面 Scroll page up/down                       |
| Ctrl + Shift + [     | 折叠（折叠）区域 Fold (collapse) region                     |
| Ctrl + Shift + ]     | 展开（未折叠）区域 Unfold (uncollapse) region               |
| Ctrl + K Ctrl + [    | 折叠（未折叠）所有子区域 Fold (collapse) all subregions     |
| Ctrl + K Ctrl + ]    | 展开（未折叠）所有子区域 Unfold (uncollapse) all subregions |
| Ctrl + K Ctrl + 0    | 折叠（折叠）所有区域 Fold (collapse) all regions            |
| Ctrl + K Ctrl + J    | 展开（未折叠）所有区域 Unfold (uncollapse) all regions      |
| Ctrl + K Ctrl + C    | 添加行注释 Add line comment                                 |
| Ctrl + K Ctrl + U    | 删除行注释 Remove line comment                              |
| Ctrl + /             | 切换行注释 Toggle line comment                              |
| Shift + Alt + A      | 切换块注释 Toggle block comment                             |
| Alt + Z              | 切换换行 Toggle word wrap                                   |

## 导航 Navigation

| 按 Press           | 功能 Function                                        |
| ------------------ | ---------------------------------------------------- |
| Ctrl + T           | 显示所有符号 Show all Symbols                        |
| Ctrl + G           | 转到行... Go to Line...                              |
| Ctrl + P           | 转到文件... Go to File...                            |
| Ctrl + Shift + O   | 转到符号... Go to Symbol...                          |
| Ctrl + Shift + M   | 显示问题面板 Show Problems panel                     |
| F8                 | 转到下一个错误或警告 Go to next error or warning     |
| Shift + F8         | 转到上一个错误或警告 Go to previous error or warning |
| Ctrl + Shift + Tab | 导航编辑器组历史记录 Navigate editor group history   |
| Alt + ← / →        | 返回/前进 Go back / forward                          |
| Ctrl + M           | 切换选项卡移动焦点 Toggle Tab moves focus            |

## 搜索和替换 Search and replace

| 按 Press          | 功能 Function                                                |
| ----------------- | ------------------------------------------------------------ |
| Ctrl + F          | 查找 Find                                                    |
| Ctrl + H          | 替换 Replace                                                 |
| F3 / Shift + F3   | 查找下一个/上一个 Find next/previous                         |
| Alt + Enter       | 选择查找匹配的所有出现 Select all occurences of Find match   |
| Ctrl + D          | 将选择添加到下一个查找匹配 Add selection to next Find match  |
| Ctrl + K Ctrl + D | 将最后一个选择移至下一个查找匹配项 Move last selection to next Find match |
| Alt + C / R / W   | 切换区分大小写/正则表达式/整个词 Toggle case-sensitive / regex / whole word |

## 多光标和选择 Multi-cursor and selection

| 按 Press                           | 功能 Function                                                |
| ---------------------------------- | ------------------------------------------------------------ |
| Alt +单击                          | 插入光标 Insert cursor                                       |
| Ctrl + Alt +↑/↓                    | 在上/下插入光标 Insert cursor above / below                  |
| Ctrl + U                           | 撤消上一个光标操作 Undo last cursor operation                |
| Shift + Alt + I                    | 在选定的每一行的末尾插入光标 Insert cursor at end of each line selected |
| Ctrl + L                           | 选择当前行 Select current line                               |
| Ctrl + Shift + L                   | 选择当前选择的所有出现 Select all occurrences of current selection |
| Ctrl + F2                          | 选择当前字的所有出现 Select all occurrences of current word  |
| Shift + Alt + →                    | 展开选择 Expand selection                                    |
| Shift + Alt + ←                    | 缩小选择 Shrink selection                                    |
| Shift + Alt + （拖动鼠标）         | 列（框）选择 Column (box) selection                          |
| Ctrl + Shift + Alt +（箭头键）     | 列（框）选择 Column (box) selection                          |
| Ctrl + Shift + Alt + PgUp / PgDown | 列（框）选择页上/下 Column (box) selection page up/down      |

## 丰富的语言编辑 Rich languages editing

| 按 Press             | 功能 Function                            |
| -------------------- | ---------------------------------------- |
| Ctrl + 空格          | 触发建议 Trigger suggestion              |
| Ctrl + Shift + Space | 触发器参数提示 Trigger parameter hints   |
| Shift + Alt + F      | 格式化文档 Format document               |
| Ctrl + K Ctrl + F    | 格式选定区域 Format selection            |
| F12                  | 转到定义 Go to Definition                |
| Alt + F12            | Peek定义 Peek Definition                 |
| Ctrl + K F12         | 打开定义到边 Open Definition to the side |
| Ctrl + .             | 快速解决 Quick Fix                       |
| Shift + F12          | 显示引用 Show References                 |
| F2                   | 重命名符号 Rename Symbol                 |
| Ctrl + K Ctrl + X    | 修剪尾随空格 Trim trailing whitespace    |
| Ctrl + K M           | 更改文件语言 Change file language        |

## 编辑器管理 Editor management

| 按 Press                     | 功能 Function                                                |
| ---------------------------- | ------------------------------------------------------------ |
| Ctrl + F4, Ctrl + W          | 关闭编辑器 Close editor                                      |
| Ctrl + K F                   | 关闭文件夹 Close folder                                      |
| Ctrl + \                     | 拆分编辑器 Split editor                                      |
| Ctrl + 1 / 2 / 3             | 聚焦到第 1，第 2 或第 3 编辑器组 Focus into 1st, 2nd or 3rd editor group |
| Ctrl + K Ctrl + ← / →        | 聚焦到上一个/下一个编辑器组 Focus into previous/next editor group |
| Ctrl + Shift + PgUp / PgDown | 向左/向右移动编辑器 Move editor left/right                   |
| Ctrl + K ← / →               | 移动活动编辑器组 Move active editor group                    |

## 文件管理 File management

| 按 Press           | 功能 Function                                                |
| ------------------ | ------------------------------------------------------------ |
| Ctrl + N           | 新文件 New File                                              |
| Ctrl + O           | 打开文件... Open File...                                     |
| Ctrl + S           | 保存 Save                                                    |
| Ctrl + Shift + S   | 另存为... Save As...                                         |
| Ctrl + K S         | 全部保存 Save All                                            |
| Ctrl + F4          | 关闭 Close                                                   |
| Ctrl + K Ctrl + W  | 关闭所有 Close All                                           |
| Ctrl + Shift + T   | 重新打开关闭的编辑器 Reopen closed editor                    |
| Ctrl + K Enter     | 输入保持打开 Enter Keep Open                                 |
| Ctrl + Tab         | 打开下一个 Open next                                         |
| Ctrl + Shift + Tab | 打开上一个 Open previous                                     |
| Ctrl + K P         | 复制活动文件的路径 Copy path of active file                  |
| Ctrl + K R         | 显示资源管理器中的活动文件 Reveal active file in Explorer    |
| Ctrl + K O         | 显示新窗口/实例中的活动文件 Show active file in new window/instance |

## 显示 Display

| 按 Press         | 功能 Function                                              |
| ---------------- | ---------------------------------------------------------- |
| F11              | 切换全屏 Toggle full screen                                |
| Shift + Alt + 0  | 切换编辑器布局 Toggle editor layout                        |
| Ctrl + = / -     | 放大/缩小 Zoom in/out                                      |
| Ctrl + B         | 切换侧栏可见性 Toggle Sidebar visibility                   |
| Ctrl + Shift + E | 显示浏览器/切换焦点 Show Explorer / Toggle focus           |
| Ctrl + Shift + F | 显示搜索 Show Search                                       |
| Ctrl + Shift + G | 显示 Git Show Git                                          |
| Ctrl + Shift + D | 显示调试 Show Debug                                        |
| Ctrl + Shift + X | 显示扩展 Show Extensions                                   |
| Ctrl + Shift + H | 替换文件 Replace in files                                  |
| Ctrl + Shift + J | 切换搜索详细信息 Toggle Search details                     |
| Ctrl + Shift + C | 打开新命令提示符/终端 Open new command prompt/terminal     |
| Ctrl + Shift +U  | 显示输出面板 Show Output panel                             |
| Ctrl + Shift + V | 切换 Markdown 预览 Toggle Markdown preview                 |
| Ctrl + K V       | 从旁边打开 Markdown 预览 Open Markdown preview to the side |
| Ctrl + K Z       | 打开禅模式（ Esc 键退出） Zen Mode (Esc Esc to ecit)       |

## 调试 Debug

| 按 Press          | 功能 Function               |
| ----------------- | --------------------------- |
| F9                | 切换断点 Toggle breakpoint  |
| F5                | 开始/继续 Start/Continue    |
| Shift + F5        | 停止 Stop                   |
| F11 / Shift + F11 | 下一步/上一步 Step into/out |
| F10               | 跳过 Step over              |
| Ctrl + K Ctrl + I | 显示悬停 Show hover         |

## 集成终端 Integrated terminal

| 按 Press              | 功能 Function                             |
| --------------------- | ----------------------------------------- |
| Ctrl + `              | 显示集成终端 Show integrated terminal     |
| Ctrl + Shift + `      | 创建新终端 Create new terminal            |
| Ctrl + C              | 复制选定 Copy selection                   |
| Ctrl + V              | 粘贴到活动端子 Paste into active terminal |
| Ctrl + ↑ / ↓          | 向上/向下滚动 Scroll up/down              |
| Shift + PgUp / PgDown | 向上/向下滚动页面 Scroll page up/down     |
| Ctrl + Home / End     | 滚动到顶部/底部 Scroll to top/bottom      |

### VScode 快捷键

- > 记住快捷键能够提高工作效率
  >
  > Ctrl+Shift+P,F1 展示全局命令面板
  >
  > Ctrl+P 快速打开最近打开的文件
  >
  > Ctrl+Shift+N 打开新的编辑器窗口
  >
  > Ctrl+Shift+W 关闭编辑器
  >
  > Ctrl + X 剪切
  >
  > Ctrl + C 复制
  >
  > **Alt + up/down 移动行上下**
  >
  > **Shift + Alt up/down 在当前行上下复制当前行**
  >
  > **Ctrl + Shift + K 删除行**
  >
  > **Ctrl + Enter 在当前行下插入新的一行**
  >
  > **Ctrl + Shift + Enter 在当前行上插入新的一行**
  >
  > Ctrl + Shift + | 匹配花括号的闭合处，跳转
  >
  > Ctrl + ] 或 [ 行缩进
  >
  > Home 光标跳转到行头
  >
  > End 光标跳转到行尾
  >
  > Ctrl + Home 跳转到页头
  >
  > Ctrl + End 跳转到页尾
  >
  > Ctrl + up/down 行视图上下偏移
  >
  > Alt + PgUp/PgDown 屏视图上下偏移
  >
  > **Ctrl + Shift + [ 折叠区域代码**
  >
  > **Ctrl + Shift + ] 展开区域代码**
  >
  > **Ctrl + / 添加关闭行注释**
  >
  > **Shift + Alt +A 块区域注释**
  >
  > **Alt + Z 添加关闭词汇包含**
  >
  > **导航快捷键**
  >
  > Ctrl + T 列出所有符号
  >
  > Ctrl + G 跳转行
  >
  > Ctrl + P 跳转文件
  >
  > Ctrl + Shift + O 跳转到符号处
  >
  > Ctrl + Shift + M 或 Ctrl + J 打开问题展示面板
  >
  > F8 跳转到下一个错误或者警告
  >
  > Shift + F8 跳转到上一个错误或者警告
  >
  > Ctrl + Shift + Tab 切换到最近打开的文件
  >
  > Alt + left / right 向后、向前
  >
  > Ctrl + M 进入用Tab来移动焦点
  >
  > Ctrl + F 查询
  >
  > Ctrl + H 替换
  >
  > F3 / Shift + F3 查询下一个/上一个
  >
  > Alt + Enter 选中所有出现在查询中的
  >
  > Ctrl + D 匹配当前选中的词汇或者行，再次选中-可操作
  >
  > **多行光标快捷键**
  >
  > **Alt + Click 插入光标-支持多个**
  >
  > Ctrl + Alt + up/down 上下插入光标-支持多个
  >
  > Ctrl + U 撤销最后一次光标操作
  >
  > Shift + Alt + I 插入光标到选中范围内所有行结束符
  >
  > **Ctrl + I 选中当前行**
  >
  > Ctrl + Shift + L 选择所有出现在当前选中的行-操作
  >
  > Ctrl + F2 选择所有出现在当前选中的词汇-操作
  >
  > **Shift + Alt + right 从光标处扩展选中全行**
  >
  > Shift + Alt + left 收缩选择区域
  >
  > Shift + Alt + (drag mouse) 鼠标拖动区域，同时在多个行结束符插入光标
  >
  > Ctrl + Shift + Alt + (Arrow Key) 也是插入多行光标的[方向键控制]
  >
  > Ctrl + Shift + Alt + PgUp/PgDown 也是插入多行光标的[整屏生效]
  >
  > Esc Esc 连续按两次Esc键取消多行光标
  >
  > Shift + Alt + F 格式化代码
  >
  > F12 跳转到定义处
  >
  > Alt + F12 代码片段显示定义
  >
  > Ctrl + K F12 在其他窗口打开定义处
  >
  > Ctrl + . 快速修复部分可以修复的语法错误
  >
  > Shift + F12 显示所有引用
  >
  > F2 重命名符号
  >
  > Ctrl + Shift + . / , 替换下个值
  >
  > **编辑器管理快捷键**
  >
  > Ctrl + F4, Ctrl + W 关闭编辑器
  >
  > Ctrl + |切割编辑窗口
  >
  > Ctrl + 1/2/3 切换焦点在不同的切割窗口
  >
  > Ctrl + Shift + PgUp/PgDown 切换标签页的位置
  >
  > **文件管理快捷键**
  >
  > Ctrl + N 新建文件
  >
  > Ctrl + O 打开文件
  >
  > Ctrl + S 保存文件
  >
  > Ctrl + Shift + S 另存为
  >
  > Ctrl + F4 关闭当前编辑窗口
  >
  > Ctrl + W 关闭所有编辑窗口
  >
  > Ctrl + Shift + T 撤销最近关闭的一个文件编辑窗口
  >
  > Ctrl + Enter 保持开启
  >
  > Ctrl + Shift + Tab 调出最近打开的文件列表，重复按会切换
  >
  > Ctrl + Tab 与上面一致，顺序不一致
  >
  > Ctrl + P 复制当前打开文件的存放路径
  >
  > Ctrl + R 打开当前编辑文件存放位置【文件管理器】
  >
  > **显示快捷键**
  >
  > F11 切换全屏模式
  >
  > Ctrl + =/- 放大 / 缩小
  >
  > **Ctrl + B 侧边栏显示隐藏**
  >
  > **Ctrl + Shift + E 资源视图和编辑视图的焦点切换**
  >
  > Ctrl + Shift + F 打开全局搜索
  >
  > **Ctrl + Shift + G 打开Git可视管理**
  >
  > Ctrl + Shift + D 打开DeBug面板
  >
  > Ctrl + Shift + X 打开插件市场面板
  >
  > Ctrl + Shift + H 在当前文件替换查询替换
  >
  > Ctrl + Shift + J 开启详细查询
  >
  > Ctrl + Shift + V 预览Markdown文件【编译后】
  >
  > Ctrl + K v 在边栏打开渲染后的视图【新建】
  >
  > **调试快捷键**
  >
  > **F9 添加解除断点**
  >
  > F5 启动调试、继续
  >
  > F11 / Shift + F11 单步进入 / 单步跳出
  >
  > **F10 单步跳过**
  >
  > **集成终端快捷键**
  >
  > Ctrl + ` 打开集成终端
  >
  > **Ctrl + Shift + ` 创建一个新的终端**
  >
  > Ctrl + C 复制所选
  >
  > Ctrl + V 复制到当前激活的终端
  >
  > Shift + PgUp / PgDown 页面上下翻屏
  >
  > Ctrl + Home / End 滚动到页面头部或尾部



# Vscode 前端快捷键及字符补全方法

------

## 欢迎大家访问我的主页:[西城Gether学习网](http://www.gether.cn)

## 我的博客:[浅作序](http://www.gether.cn/blog)

1. 快捷键的使用

| 快捷键           | 说明                   |
| ---------------- | :--------------------- |
| **Tab**          | 补全代码               |
| **Alt +  Tab**   | 切换windows窗口        |
| **Ctrl + A**     | 选择全部代码           |
| **Ctrl + C**     | 复制                   |
| **Ctrl + V**     | 粘贴                   |
| **Ctrl + X**     | 剪切                   |
| **Ctrl + Z**     | 返回上一次操作         |
| **Ctrl + F**     | 查找                   |
| **Ctrl + /**     | 添加或取消注释         |
| **Ctrl + + / -** | 放大/缩小              |
| **Ctrl + F1**    | 打开浏览器             |
| **F12**          | 浏览器中为启用调试模式 |
| **F11**          | 浏览器中为全屏         |

1. 字符补全( ♥ 为常用项 )

   - ♥多项：* , 缩写：

     ```
     ul>li*5
     ```

     

     ```css
     <ul>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
        <li></li>
     </ul>
     ```

   - ♥Class类：

     .

      , 缩写：

     ```
     div.top*2
     ```

     （Class类可以多次使用）

     

     ```css
     <div class="top"></div>
     <div class="top"></div>
     ```

     缩写：

     ```
     p.class1.class2.class3
     ```

     

     ```css
     <p class="class1 class2 class3"></p>
     ```

   - ♥Id类：**# ** , 缩写：

     ```
     div#top
     ```

     (一个Id类只能使用一次)

     

     ```css
     <div id="top"></div>
     ```

     缩写：

     ```
     form#search.wide
     ```

     

     ```css
     <form id="search" class="wide"></form>
     ```

   - ♥自增符号：*

     ![**, 缩写：`ul>li.item](https://math.jianshu.com/math?formula=**%2C%20%E7%BC%A9%E5%86%99%EF%BC%9A%60ul%3Eli.item)

     5`

     

     ```css
     <ul>
         <li class="item1"></li>
         <li class="item2"></li>
         <li class="item3"></li>
         <li class="item4"></li>
         <li class="item5"></li>
     </ul>
     ```

   - ♥子元素：

     \>

      , 缩写： 

     ```
     nav>ul>li
     ```

     

     ```css
     <nav>
         <ul>
             <li></li>
         </ul>
     </nav>
     ```

   - ♥兄弟元素：

     +

      , 缩写：

     ```
     div+div >p> span+em
     ```

     

     ```css
     <div></div>
     <div>
         <p><span></span><em></em></p>
     </div>
     ```

   - 自定义属性：

     []

     缩写：

     ```
     p[title=”Hello world”]
     ```

     

     ```css
     <p title="Hello world"></p>
     ```

     缩写：

     ```
     td[rowspan=2 colspan=3 title]
     ```

     

     ```css
     <td rowspan="2" colspan="3" title=""></td>
     ```

     缩写：

     ```
     [a=’value1’ b=”value2”]
     ```

     (a,b为属性，value为属性值。具体使用见上面的例子)

     

     ```css
     <div a="value1" b="value2"></div>
     ```

   - 文本：

     {}

     缩写：

     ```
     a{Click me}
     ```

     

     ```css
      <a href="">Click me</a>
     ```



作者：浅作序
链接：https://www.jianshu.com/p/61a1de2b45cc
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。



# 方法二： 拓展emmet支持类型(非常通用)

在阅读官方文档的时候发现有一种方式也可以达到效果，就是修改emmet的提示范围，如果emmet支持vue文件，不一样是支持tab自动补全吗？来看一下怎么弄

点vscode左下角齿轮，有一个settings，点击！

找到如下图的settings.json点击(往下滑就能找到，很多的地方会出现，都一样，指向同一个文件)

![[外链图片转存失败(VScode快捷键.assets/20190915170755624.png)("./images/settingsjson.png")]](https://img-blog.csdnimg.cn/20190915170755624.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2NoZW5jaGVuODE4,size_16,color_FFFFFF,t_70)


在最后补上这么一段代码(截图如下，记住不要写到最大的一对打括号外)

```
"emmet.includeLanguages": {
"vue": "html",
"javascript": "html"
}
```


大功告成，保存退出，重启vscode！

提示：如果emmet默认tab被覆盖禁止掉，就在settings.json最后加上"emmet.triggerExpansionOnTab":true
————————————————
版权声明：本文为CSDN博主「就是闫先森」的原创文章，遵循 CC 4.0 BY-SA 版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/chenchen818/article/details/100858217





```json
// VScode 配置文件 202001252308
{
    "liveServer.settings.donotShowInfoMsg": true,
    "open-in-browser.default": "C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe",
    "editor.tabSize": 2,
    "[html]": {
        "editor.defaultFormatter": "HookyQR.beautify"
    },
    "workbench.sideBar.location": "left",
    "editor.wordWrap": "on",
    "workbench.iconTheme": "vscode-icons",
    "vsicons.dontShowNewVersionMessage": true,
    
    "eslint.migration.2_x": "off",
    "eslint.format.enable": true,
    "prettier.eslintIntegration": true,
    "eslint.codeActionsOnSave": true,
    "prettier.eslintItegration": true,
    "prettier.semi": false,
    "prettier.singleQuote": true,
    "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
    "vetur.format.defaultFormatter.html": "js-beautify-html",
    "vetur.format.defaultFormatter.js": "vscode-typescript",
    "vetur.format.defaultFormatterOptions": {
        "js-beautify-html": {
            "wrap_attributes": "force-aligned"
        },
        "prettyhtml": {
            "printWidth": 100,
            "singleQuote": false,
            "wrapAttributes": false,
            "sortAttributes": false
        },
        "eslint.validate": [
            "javascript",
            "javascriptreact",
            "html",
            {
              "language": "html",
              "autoFix": true
            },
            {
              "language": "vue",
              "autoFix": true
            }
          ],
        "eslint.options": {
            "plugins": ["html"]
        },
        "window.zommLevel": 1,
        "editor.formatOnSave": true,
    },
    "[javascript]": {
        "editor.defaultFormatter": "HookyQR.beautify"
    },
    "files.autoSave": "off",
    "[json]": {
        "editor.defaultFormatter": "HookyQR.beautify"
    },
    "emmet.includeLanguages": {
        "vue": "html",
        "javascript": "html",
    },
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    },
    "eslint.codeActionsOnSave": true
}
```

```
// 拷贝 vue 版, eslint 自动修复
{
    "eslint.autoFixOnSave": true,
    "prettier.eslintIntegration": true,
    "prettier.semi": false,
    "prettier.singleQuote": true,
    "javascript.format.insertSpaceBeforeFunctionParenthesis": true,
    "vetur.format.defaultFormatter.html": "js-beautify-html",
    "vetur.format.defaultFormatter.js": "vscode-typescript",
    "vetur.format.defaultFormatterOptions": {
        "js-beautify-html": {
            "wrap_attributes": "force-aligned"
        }
    },
    "eslint.validate": [
        "javascript",
        "html"
    ],
    "eslint.options": {
        "plugins": [
            "html"
        ]
    },
    // "window.zoomLevel": 1,
    "editor.formatOnSave": true,
    "html.format.enable": false,
    "html.format.indentHandlebars": true,
    "html.format.preserveNewLines": true,
    "workbench.sideBar.location": "left",
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    },
    "emmet.includeLanguages": {
        "vue": "html",
        "javascript": "html",
    }
}
```

