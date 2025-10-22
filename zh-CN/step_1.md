为了使你的网页布局更精确，你可以使用网格！

### 创建一个类

在你的 `style.css` 文件中创建一个类 —— 最好为此使用 **class** 或 **id**。 如果你设置标签样式，则页面上该标签的每个版本都将是一个网格。

将 `display` 属性设置为 `grid`。

设置 `height`。 你可以为此使用 `vh`，或设置 `px` 值。

定义你的**rows**（`grid-template-rows` 属性）和**columns**（`grid-template-columns` 属性）。

你可以通过以下任意方式设置行的大小：

- 百分比——你可以将行和列设置为宽度或高度的 `%`
- 分数值 – 你可以将它们设置为宽度或高度的 `fr`
- 像素 – 您可以将高度设置为直接的 `px` 值

以下是一些例子：

--- code ---
---
language: css
filename: style.css 
---
// 一个类
.fact-holder {
  display: grid;
  height: 50vh;
  grid-template-rows: 50% 50%;
  grid-template-columns: 50% 50%;
}

--- /code ---

--- code ---
---
language: css
filename: style.css
---
// 一个 ID
#homepage-grid {
  display: grid;
  height: 80vh;
  grid-template-rows: 2fr 1fr 1fr;
  grid-template-columns: 1fr 1fr;
}

--- /code ---

### 将网格添加到 HTML

创建选择器后，将您的类或 ID 添加到 **HTML** 元素。

--- code ---
---
language: html
---

<section class="fact-holder">

</section>

--- /code ---

--- code ---
---
language: html
---

<div id="homepage-grid">

</div>

--- /code ---
