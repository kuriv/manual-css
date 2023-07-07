# CSS 弹性布局

* [display](#display)
* [flex-direction](#flex-direction)
* [flex-wrap](#flex-wrap)
* [flex-flow](#flex-flow)
* [justify-content](#justify-content)
* [align-items](#align-items)
* [align-content](#align-content)
* [order](#order)
* [flex-grow](#flex-grow)
* [flex-shrink](#flex-shrink)
* [flex-basis](#flex-basis)
* [flex](#flex)
* [align-self](#align-self)
* [单列布局示例](#单列布局示例)
* [经典导航示例](#经典导航示例)
* [隔行交叉示例](#隔行交叉示例)
* [网格布局示例](#网格布局示例)
* [圣杯布局示例](#圣杯布局示例)
* [垂直居中示例](#垂直居中示例)
* [自动对齐示例](#自动对齐示例)

<link rel="stylesheet" type="text/css" href="CSS 弹性布局.css">

# display

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}
```

效果：

<section id="section_1">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex-direction

语法：

```html
<main class="row">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="row-reverse">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="column">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="column-reverse">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

.row {
    flex-direction: row;
}

.row-reverse {
    flex-direction: row-reverse;
}

.column {
    flex-direction: column;
}

.column-reverse {
    flex-direction: column-reverse;
}
```

效果：

<section id="section_2">
    <main class="row">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="row-reverse">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="column">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="column-reverse">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex-wrap

语法：

```html
<main class="nowrap">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="wrap">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="wrap-reverse">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 1000px;
    height: 100px;
}

.nowrap {
    flex-wrap: nowrap;
}

.wrap {
    flex-wrap: wrap;
}

.wrap-reverse {
    flex-wrap: wrap-reverse;
}
```

效果：

<section id="section_3">
    <main class="nowrap">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="wrap">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="wrap-reverse">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex-flow

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
    flex-flow: row-reverse wrap-reverse;
}

div {
    background-color: red;
    width: 1000px;
    height: 100px;
}
```

效果：

<section id="section_4">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# justify-content

语法：

```html
<main class="flex-start">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="center">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="flex-end">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="space-between">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="space-around">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="space-evenly">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

.flex-start {
    justify-content: flex-start;
}

.center {
    justify-content: center;
}

.flex-end {
    justify-content: flex-end;
}

.space-between {
    justify-content: space-between;
}

.space-around {
    justify-content: space-around;
}

.space-evenly {
    justify-content: space-evenly;
}
```

效果：

<section id="section_5">
    <main class="flex-start">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="center">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="flex-end">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="space-between">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="space-around">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="space-evenly">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# align-items

语法：

```html
<main class="flex-start">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="center">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="flex-end">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

div:nth-child(2) {
    height: 200px;
}

div:nth-child(3) {
    height: 300px;
}

.flex-start {
    align-items: flex-start;
}

.center {
    align-items: center;
}

.flex-end {
    align-items: flex-end;
}
```

效果：

<section id="section_6">
    <main class="flex-start">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="center">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="flex-end">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# align-content

语法：

```html
<main class="flex-start">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="center">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="flex-end">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="space-between">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="space-around">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="space-evenly">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
    flex-wrap: wrap;
    width: 200px;
    height: 300px;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

.flex-start {
    align-content: flex-start;
}

.center {
    align-content: center;
}

.flex-end {
    align-content: flex-end;
}

.space-between {
    align-content: space-between;
}

.space-around {
    align-content: space-around;
}

.space-evenly {
    align-content: space-evenly;
}
```

效果：

<section id="section_7">
    <main class="flex-start">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="center">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="flex-end">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="space-between">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="space-around">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="space-evenly">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# order

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

div:nth-child(1) {
    order: 2;
}

div:nth-child(2) {
    order: 1;
}

div:nth-child(3) {
    order: 3;
}
```

效果：

<section id="section_8">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex-grow

语法：

```html
<main class="flex-grow-1">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="flex-grow-2">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

.flex-grow-1 div:nth-child(2) {
    flex-grow: 1;
}

.flex-grow-2 div:nth-child(1) {
    flex-grow: 1;
}

.flex-grow-2 div:nth-child(2) {
    flex-grow: 3;
}

.flex-grow-2 div:nth-child(3) {
    flex-grow: 1;
}
```

效果：

<section id="section_9">
    <main class="flex-grow-1">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="flex-grow-2">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex-shrink

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 500px;
    height: 100px;
}

div:nth-child(2) {
    flex-shrink: 0;
}
```

效果：

<section id="section_10">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex-basis

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 200px;
    height: 100px;
}

div:nth-child(2) {
    flex-basis: 500px;
}
```

效果：

<section id="section_11">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# flex

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

div:nth-child(1) {
    flex: auto;
}

div:nth-child(2) {
    flex: 2 0 500px;
}

div:nth-child(3) {
    flex: none;
}
```

效果：

<section id="section_12">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# align-self

语法：

```html
<main class="flex-start">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="center">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
<main class="flex-end">
    <div>1</div>
    <div>2</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: red;
    width: 100px;
    height: 100px;
}

div:nth-child(2) {
    height: 200px;
}

div:nth-child(3) {
    height: 300px;
}

.flex-start div:nth-child(2) {
    align-self: flex-start;
}

.center div:nth-child(2) {
    align-self: center;
}

.flex-end div:nth-child(2) {
    align-self: flex-end;
}
```

效果：

<section id="section_13">
    <main class="flex-start">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="center">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
    <main class="flex-end">
        <div>1</div>
        <div>2</div>
        <div>3</div>
    </main>
</section>

# 单列布局示例

语法：

```html
<header>header</header>
<main>main</main>
<footer>footer</footer>
```

```css
* {
    margin: 0;
    padding: 0;
}

html {
    height: 100%;
}

body {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
}

header {
    width: 100%;
    height: 100px;
    background-color: lightseagreen;
    flex-shrink: 0;
}

main {
    width: 500px;
    background-color: lightcoral;
    flex-grow: 1;
}

footer {
    width: 100%;
    height: 100px;
    background-color: lightseagreen;
    flex-shrink: 0;
}
```

效果：

<section id="section_14">
    <header>header</header>
    <main>main</main>
    <footer>footer</footer>
</section>

# 经典导航示例

语法：

```html
<header>
    <a href="#" class="logo"></a>
    <nav class="navbar">
        <a href="#">导航1</a>
        <a href="#">导航2</a>
        <a href="#">导航3</a>
    </nav>
    <a href="#" class="username">用户名</a>
    <a href="#" class="logout">退出</a>
</header>
```

```css
header {
    display: flex;
    align-items: center;
}

.logo {
    width: 50px;
    height: 50px;
    background-color: lightblue;
    flex-shrink: 0;
}

.navbar {
    margin: 0 10px;
    flex-shrink: 0;
}

.username {
    margin-left: auto;
    flex-shrink: 0;
}

.logout {
    margin-left: 10px;
    flex-shrink: 0;
}
```

效果：

<section id="section_15">
    <header>
        <a href="#" class="logo"></a>
        <nav class="navbar">
            <a href="#">导航1</a>
            <a href="#">导航2</a>
            <a href="#">导航3</a>
        </nav>
        <a href="#" class="username">用户名</a>
        <a href="#" class="logout">退出</a>
    </header>
</section>

# 隔行交叉示例

语法：

```html
<main>
    <div class="box">
        <div class="img">img</div>
        <div class="info">info</div>
    </div>
    <div class="box">
        <div class="img">img</div>
        <div class="info">info</div>
    </div>
    <div class="box">
        <div class="img">img</div>
        <div class="info">info</div>
    </div>
</main>
```

```css
main {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.box {
    display: flex;
    margin-bottom: 10px;
}

.box:nth-child(2) {
    flex-direction: row-reverse;
}

.img {
    width: 100px;
    height: 200px;
    background-color: lightpink;
}

.info {
    width: 300px;
    height: 200px;
    background-color: lightblue;
}
```

效果：

<section id="section_16">
    <main>
        <div class="box">
            <div class="img">img</div>
            <div class="info">info</div>
        </div>
        <div class="box">
            <div class="img">img</div>
            <div class="info">info</div>
        </div>
        <div class="box">
            <div class="img">img</div>
            <div class="info">info</div>
        </div>
    </main>
</section>

# 网格布局示例

语法：

```html
<main>
    <div>1</div>
    <div>2</div>
    <div>3</div>
    <div>4</div>
    <div>5</div>
    <div>6</div>
    <div>7</div>
    <div>8</div>
    <div>9</div>
</main>
```

```css
main {
    display: flex;
    flex-wrap: wrap;
}

div {
    width: 30%;
    min-width: 100px;
    height: 100px;
    margin: 10px;
    background-color: lightpink;
    flex-grow: 1;
}
```

效果：

<section id="section_17">
    <main>
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
        <div>6</div>
        <div>7</div>
        <div>8</div>
        <div>9</div>
    </main>
</section>

# 圣杯布局示例

语法：

```html
<header>header</header>
<main>
    <div class="left">left</div>
    <div class="center">center</div>
    <div class="right">right</div>
</main>
<footer>footer</footer>
```

```css
* {
    margin: 0;
    padding: 0;
}

html {
    height: 100%;
}

body {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
}

header {
    width: 100%;
    height: 100px;
    background-color: lightseagreen;
    flex-shrink: 0;
}

main {
    width: 100%;
    display: flex;
    background-color: lightcoral;
    flex-grow: 1;
}

.left {
    width: 100px;
    background-color: lightcoral;
}

.center {
    flex-grow: 1;
    background-color: lightblue;
}

.right {
    width: 100px;
    background-color: lightcoral;
}

footer {
    width: 100%;
    height: 100px;
    background-color: lightseagreen;
    flex-shrink: 0;
}
```

效果：

<section id="section_18">
    <header>header</header>
    <main>
        <div class="left">left</div>
        <div class="center">center</div>
        <div class="right">right</div>
    </main>
    <footer>footer</footer>
</section>

# 垂直居中示例

语法：

```html
<main>
    <div></div>
</main>
```

```css
main {
    width: 100px;
    height: 300px;
    background-color: lightcoral;
    display: flex;
    align-items: center;
}

div {
    width: 100px;
    height: 100px;
    background-color: lightseagreen;
}
```

效果：

<section id="section_19">
    <main>
        <div></div>
    </main>
</section>

# 自动对齐示例

语法：

```html
<main>
    <div>1</div>
    <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum voluptates minus ipsum quaerat sit quis, soluta dolore animi autem nemo veritatis similique facere, amet laborum blanditiis, ratione, quisquam iure impedit.</div>
    <div>3</div>
</main>
```

```css
main {
    display: flex;
}

div {
    background-color: lightcoral;
    margin: 10px;
    flex: 1;
}
```

效果：

<section id="section_20">
    <main>
        <div>1</div>
        <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum voluptates minus ipsum quaerat sit quis, soluta dolore animi autem nemo veritatis similique facere, amet laborum blanditiis, ratione, quisquam iure impedit.</div>
        <div>3</div>
    </main>
</section>
