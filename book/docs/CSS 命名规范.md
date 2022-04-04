# CSS 命名规范

* [BEM 是什么](#bem-是什么)
* [为什么要选择 BEM](#为什么要选择-bem)
* [BEM 命名规则](#bem-命名规则)
* [示例](#示例)

## BEM 是什么

`BEM` 是 `Block`、 `Element` 、 `Modifier` 的简写，是一种组件化的 CSS 命名方法和规范，由俄罗斯 Yandex 团队所提出。使用 `BEM` 主要是为了将用户界面划分成独立的块，使开发更为简单和快速，有利于团队协作，方便维护。

## 为什么要选择 BEM

很多新手在开始编写网页时，在命名方面可能都比较随心所欲。但是在一个正式的项目中，会有很多开发人员同时进行开发，如果每个开发人员都用自己的一套命名，这样会造成命名的识别度和一致性成为很大的问题，还会造成命名污染，而使用 `BEM` 就可以很好的解决这个问题。

当然使用 `BEM` 还有很多其他的好处，例如每个块之间都是独立的，因此不会遇到层叠带来的问题，并且这些块可以多次重用，可以减少必须维护的 CSS 代码量等。

## BEM 命名规则

* 块名称为其元素和修饰符定义了命名空间。
* 块名称与元素名称之间用双下划线 `__` 分隔。
* 块名称与修饰符或元素与修饰符之间用双连字符 `--` 分隔。
* 命名一般使用小写字母。
* 单词之间可以使用 `-` 分隔。

命名约定的模式有如下几种：

```css
.block {}
.block__element {}
.block--modifier {}
.block__element--modifier {}
```

其中 .block 代表了更高级别的抽象或组件， .block__element 代表 .block 的后代，用于形成一个完整的 .block 的整体， .block--modifier 代表 .block 的不同状态或不同版本。使用两个连字符和下划线是为了让自己定义的块可以用单个连字符来界定。

## 示例

当我们添加多个按钮时，一个红色按钮、一个绿色按钮、一个蓝色按钮、一个黄色按钮：

```html
<div class="banner__btn">
    <button class="button banner__btn--red"></button>
    <button class="button banner__btn--green"></button>
    <button class="button banner__btn--blue"></button>
    <button class="button banner__btn--yellow"></button>
</div>
```

CSS代码如下所示：

```css
.banner__btn--red { background-color: red; }
.banner__btn--green { background-color: green; }
.banner__btn--blue { background-color: blue; }
.banner__btn--yellow { background-color: yellow; }
```

