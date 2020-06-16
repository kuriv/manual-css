# CSS 选择器

* [.class - 指定 class 的元素](#class---指定-class-的元素)
* [#id - 指定 id 的元素](#id---指定-id-的元素)
* [* - 所有元素](#--所有元素)
* [element - 指定的 element 元素](#element---指定的-element-元素)
* [element, element - 指定的多个 element 元素](#element-element---指定的多个-element-元素)
* [element element - 指定 element 元素中的 element 元素](#element-element---指定-element-元素中的-element-元素)
* [element > element - 指定 element 父元素的 element 子元素](#element--element---指定-element-父元素的-element-子元素)
* [element + element - 指定 element 元素后的 element 元素](#element--element---指定-element-元素后的-element-元素)
* [element ~ element - 指定 element 元素后的所有 element 元素](#element--element---指定-element-元素后的所有-element-元素)
* [[attribute] - 指定包含属性 attribute 的元素](#attribute---指定包含属性-attribute-的元素)
* [[attribute=value] - 指定包含属性 attribute 且属性值为 value 的元素](#attributevalue---指定包含属性-attribute-且属性值为-value-的元素)
* [[attribute~=value] - 指定包含属性 attribute 且属性值包含独立单词 value 的元素](#attributevalue---指定包含属性-attribute-且属性值包含独立单词-value-的元素)
* [[attribute|=value] - 指定包含属性 attribute 且属性值包含独立单词开头为 value 的元素](#attributevalue---指定包含属性-attribute-且属性值包含独立单词开头为-value-的元素)
* [[attribute^=value] - 指定包含属性 attribute 且属性值以 value 开头的元素](#attributevalue---指定包含属性-attribute-且属性值以-value-开头的元素)
* [[attribute$=value] - 指定包含属性 attribute 且属性值以 value 结尾的元素](#attributevalue---指定包含属性-attribute-且属性值以-value-结尾的元素)
* [[attribute*=value] - 指定包含属性 attribute 且属性值包含 value 字符串的元素](#attributevalue---指定包含属性-attribute-且属性值包含-value-字符串的元素)
* [:link - 指定未被访问的链接](#link---指定未被访问的链接)
* [:visited - 指定已被访问的链接](#visited---指定已被访问的链接)
* [:hover - 指定鼠标指针悬停之上的链接](#hover---指定鼠标指针悬停之上的链接)
* [:active - 指定活动链接](#active---指定活动链接)
* [:focus - 指定获得焦点的输入元素](#focus---指定获得焦点的输入元素)
* [:lang(language) - 指定包含属性 lang 且属性值包含独立单词开头为 language 的元素](#langlanguage---指定包含属性-lang-且属性值包含独立单词开头为-language-的元素)
* [:before - 指定元素前](#before---指定元素前)
* [:after - 指定元素后](#after---指定元素后)
* [:first-letter - 指定元素的首字符](#first-letter---指定元素的首字符)
* [:first-line - 指定元素的首行](#first-line---指定元素的首行)
* [:first-child - 指定属于其父元素的首个子元素](#first-child---指定属于其父元素的首个子元素)
* [:last-child - 指定属于其父元素的最后一个子元素](#last-child---指定属于其父元素的最后一个子元素)
* [:first-of-type - 指定属于其父元素的首个指定元素](#first-of-type---指定属于其父元素的首个指定元素)
* [:last-of-type - 指定属于其父元素的最后一个指定元素](#last-of-type---指定属于其父元素的最后一个指定元素)
* [:only-child - 指定属于其父元素的唯一子元素](#only-child---指定属于其父元素的唯一子元素)
* [:only-of-type - 指定属于其父元素的唯一指定元素](#only-of-type---指定属于其父元素的唯一指定元素)
* [:nth-child(n) - 指定属于其父元素的第 n 个元素](#nth-childn---指定属于其父元素的第-n-个元素)
* [:nth-last-child(n) - 指定属于其父元素的倒数第 n 个元素](#nth-last-childn---指定属于其父元素的倒数第-n-个元素)
* [:nth-of-type(n) - 指定属于其父元素的第 n 个指定元素](#nth-of-typen---指定属于其父元素的第-n-个指定元素)
* [:nth-last-of-type(n) - 指定属于其父元素的倒数第 n 个指定元素](#nth-last-of-typen---指定属于其父元素的倒数第-n-个指定元素)
* [:root - 指定根元素](#root---指定根元素)
* [:empty - 指定没有子元素的元素](#empty---指定没有子元素的元素)
* [:target - 指定的锚点链接](#target---指定的锚点链接)
* [:enabled - 指定启用的输入元素](#enabled---指定启用的输入元素)
* [:disabled - 指定禁用的输入元素](#disabled---指定禁用的输入元素)
* [:not(selector) - 指定非 selector 元素的元素](#notselector---指定非-selector-元素的元素)
* [::selection - 被用户选中的区域](#selection---被用户选中的区域)

<link rel="stylesheet" type="text/css" href="CSS 选择器.css">

## .class - 指定 class 的元素

语法：

```html
<p class="section-class">这是一段普通的段落。</p>
```

```css
.section-class {
    background-color: yellow;
}
```

效果：

<section id="section_1">
    <p class="section-class">这是一段普通的段落。</p>
</section>

## #id - 指定 id 的元素

语法：

```html
<p id="section-id">这是一段普通的段落。</p>
```

```css
#section-id {
    background-color: yellow;
}
```

效果：

<section id="section_2">
    <p id="section-id">这是一段普通的段落。</p>
</section>

## * - 所有元素

语法：

```html
<p>这是一段普通的段落。</p>
```

```css
* {
    background-color: yellow;
}
```

效果：

<section id="section_3">
    <p>这是一段普通的段落。</p>
</section>

## element - 指定的 element 元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
```

```css
p {
    background-color: yellow;
}
```

效果：

<section id="section_4">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
</section>

## element, element - 指定的多个 element 元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
```

```css
div, p {
    background-color: yellow;
}
```

效果：

<section id="section_5">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
</section>

## element element - 指定 element 元素中的 element 元素

语法：

```html
<div>
    <p>
        <span>这是一段普通的段落。</span>
    </p>
</div>
```

```css
div span {
    background-color: yellow;
}
```

效果：

<section id="section_6">
    <div>
        <p>
            <span>这是一段普通的段落。</span>
        </p>
    </div>
</section>

## element > element - 指定 element 父元素的 element 子元素

语法：

```html
<div>
    <span>这是一段普通的段落。</span>
    <p>
        <span>这是一段普通的段落。</span>
    </p>
</div>
```

```css
div > span {
    background-color: yellow;
}
```

效果：

<section id="section_7">
    <div>
        <span>这是一段普通的段落。</span>
        <p>
            <span>这是一段普通的段落。</span>
        </p>
    </div>
</section>

## element + element - 指定 element 元素后的 element 元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
div + p {
    background-color: yellow;
}
```

效果：

<section id="section_8">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## element ~ element - 指定 element 元素后的所有 element 元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
div ~ p {
    background-color: yellow;
}
```

效果：

<section id="section_9">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## [attribute] - 指定包含属性 attribute 的元素

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
```

```css
a[target] {
    background-color: yellow;
}
```

效果：

<section id="section_10">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>

## [attribute=value] - 指定包含属性 attribute 且属性值为 value 的元素

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
```

```css
a[target="_blank"] {
    background-color: yellow;
}
```

效果：

<section id="section_11">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>

## [attribute~=value] - 指定包含属性 attribute 且属性值包含独立单词 value 的元素

语法：

```html
<a href="https://github.com/" target="_blank" title="foo bar">GitHub</a>
<a href="https://www.google.com/" target="_blank" title="foobar">Google</a>
```

```css
a[title~="foo"] {
    background-color: yellow;
}
```

效果：

<section id="section_12">
    <a href="https://github.com/" target="_blank" title="foo bar">GitHub</a>
    <a href="https://www.google.com/" target="_blank" title="foobar">Google</a>
</section>

## [attribute|=value] - 指定包含属性 attribute 且属性值包含独立单词开头为 value 的元素

语法：

```html
<p lang="en">这是一段普通的段落。</p>
<p lang="en-us">这是一段普通的段落。</p>
<p lang="zh">这是一段普通的段落。</p>
<p lang="zh-cmn-hans">这是一段普通的段落。</p>
```

```css
p[lang|="zh"] {
    background-color: yellow;
}
```

效果：

<section id="section_13">
    <p lang="en">这是一段普通的段落。</p>
    <p lang="en-us">这是一段普通的段落。</p>
    <p lang="zh">这是一段普通的段落。</p>
    <p lang="zh-cmn-hans">这是一段普通的段落。</p>
</section>

## [attribute^=value] - 指定包含属性 attribute 且属性值以 value 开头的元素

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
<a href="http://www.example.com/" target="_blank">Example</a>
```

```css
a[href^="https"] {
    background-color: yellow;
}
```

效果：

<section id="section_14">
    <a href="https://github.com/" target="_blank">GitHub</a>
    <a href="http://www.example.com/" target="_blank">Example</a>
</section>

## [attribute$=value] - 指定包含属性 attribute 且属性值以 value 结尾的元素

语法：

```html
<a href="https://github.com/" target="_blank" title="GitHub">GitHub</a>
<a href="https://www.google.com/" target="_blank" title="Google">Google</a>
```

```css
a[title$="e"] {
    background-color: yellow;
}
```

效果：

<section id="section_15">
    <a href="https://github.com/" target="_blank" title="GitHub">GitHub</a>
    <a href="https://www.google.com/" target="_blank" title="Google">Google</a>
</section>

## [attribute*=value] - 指定包含属性 attribute 且属性值包含 value 字符串的元素

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
<a href="https://www.google.com/" target="_blank">Google</a>
```

```css
a[href*="github"] {
    background-color: yellow;
}
```

效果：

<section id="section_16">
    <a href="https://github.com/" target="_blank">GitHub</a>
    <a href="https://www.google.com/" target="_blank">Google</a>
</section>

## :link - 指定未被访问的链接

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
```

```css
a:link {
    background-color: yellow;
}
```

效果：

<section id="section_17">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>

## :visited - 指定已被访问的链接

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
```

```css
a:visited {
    color: red;
}
```

效果：

<section id="section_18">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>

## :hover - 指定鼠标指针悬停之上的链接

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
```

```css
a:hover {
    color: red;
}
```

效果：

<section id="section_19">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>

## :active - 指定活动链接

语法：

```html
<a href="https://github.com/" target="_blank">GitHub</a>
```

```css
a:active {
    color: red;
}
```

效果：

<section id="section_20">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>

## :focus - 指定获得焦点的输入元素

语法：

```html
<input type="text" name="foo">
<input type="text" name="bar">
```

```css
input:focus {
    background-color: yellow;
}
```

效果：

<section id="section_21">
    <input type="text" name="foo">
    <input type="text" name="bar">
</section>

## :lang(language) - 指定包含属性 lang 且属性值包含独立单词开头为 language 的元素

语法：

```html
<p lang="en">这是一段普通的段落。</p>
<p lang="en-us">这是一段普通的段落。</p>
<p lang="zh">这是一段普通的段落。</p>
<p lang="zh-cmn-hans">这是一段普通的段落。</p>
```

```css
p:lang(zh) {
    background-color: yellow;
}
```

效果：

<section id="section_22">
    <p lang="en">这是一段普通的段落。</p>
    <p lang="en-us">这是一段普通的段落。</p>
    <p lang="zh">这是一段普通的段落。</p>
    <p lang="zh-cmn-hans">这是一段普通的段落。</p>
</section>

## :before - 指定元素前

语法：

```html
<p>这是一段普通的段落。</p>
```

```css
p:before {
    content: "#";
}
```

效果：

<section id="section_23">
    <p>这是一段普通的段落。</p>
</section>

## :after - 指定元素后

语法：

```html
<p>这是一段普通的段落。</p>
```

```css
p:after {
    content: "#";
}
```

效果：

<section id="section_24">
    <p>这是一段普通的段落。</p>
</section>

## :first-letter - 指定元素的首字符

语法：

```html
<p>这是一段普通的段落。</p>
```

```css
p:first-letter {
    color: red;
}
```

效果：

<section id="section_25">
    <p>这是一段普通的段落。</p>
</section>

## :first-line - 指定元素的首行

语法：

```html
<p>这是一段普通的段落。<br>这是一段普通的段落。</p>
```

```css
p:first-line {
    color: red;
}
```

效果：

<section id="section_26">
    <p>这是一段普通的段落。<br>这是一段普通的段落。</p>
</section>

## :first-child - 指定属于其父元素的首个子元素

语法：

```html
<section>
    <p>这是一段普通的段落。</p>
    <div>
        <p>这是一段普通的段落。</p>
    </div>
    <p>这是一段普通的段落。</p>
</section>
```

```css
p:first-child {
    background-color: yellow;
}
```

效果：

<section id="section_27">
    <section>
        <p>这是一段普通的段落。</p>
        <div>
            <p>这是一段普通的段落。</p>
        </div>
        <p>这是一段普通的段落。</p>
    </section>
</section>

## :last-child - 指定属于其父元素的最后一个子元素

语法：

```html
<section>
    <p>这是一段普通的段落。</p>
    <div>
        <p>这是一段普通的段落。</p>
    </div>
    <p>这是一段普通的段落。</p>
</section>
```

```css
p:last-child {
    background-color: yellow;
}
```

效果：

<section id="section_28">
    <section>
        <p>这是一段普通的段落。</p>
        <div>
            <p>这是一段普通的段落。</p>
        </div>
        <p>这是一段普通的段落。</p>
    </section>
</section>

## :first-of-type - 指定属于其父元素的首个指定元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
p:first-of-type {
    background-color: yellow;
}
```

效果：

<section id="section_29">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## :last-of-type - 指定属于其父元素的最后一个指定元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<div>这是一段普通的段落。</div>
```

```css
p:last-of-type {
    background-color: yellow;
}
```

效果：

<section id="section_30">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <div>这是一段普通的段落。</div>
</section>

## :only-child - 指定属于其父元素的唯一子元素

语法：

```html
<div>
    <p>这是一段普通的段落。</p>
</div>
<div>
    <p>这是一段普通的段落。</p>
    <div>这是一段普通的段落。</div>
</div>
```

```css
p:only-child {
    background-color: yellow;
}
```

效果：

<section id="section_31">
    <div>
        <p>这是一段普通的段落。</p>
    </div>
    <div>
        <p>这是一段普通的段落。</p>
        <div>这是一段普通的段落。</div>
    </div>
</section>

## :only-of-type - 指定属于其父元素的唯一指定元素

语法：

```html
<div>
    <p>这是一段普通的段落。</p>
</div>
<div>
    <p>这是一段普通的段落。</p>
    <div>这是一段普通的段落。</div>
</div>
```

```css
p:only-of-type {
    background-color: yellow;
}
```

效果：

<section id="section_32">
    <div>
        <p>这是一段普通的段落。</p>
    </div>
    <div>
        <p>这是一段普通的段落。</p>
        <div>这是一段普通的段落。</div>
    </div>
</section>

## :nth-child(n) - 指定属于其父元素的第 n 个元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
p:nth-child(2) {
    background-color: yellow;
}
```

效果：

<section id="section_33">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## :nth-last-child(n) - 指定属于其父元素的倒数第 n 个元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
p:nth-last-child(2) {
    background-color: yellow;
}
```

效果：

<section id="section_34">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## :nth-of-type(n) - 指定属于其父元素的第 n 个指定元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
p:nth-of-type(2) {
    background-color: yellow;
}
```

效果：

<section id="section_35">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## :nth-last-of-type(n) - 指定属于其父元素的倒数第 n 个指定元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
<p>这是一段普通的段落。</p>
```

```css
p:nth-last-of-type(2) {
    background-color: yellow;
}
```

效果：

<section id="section_36">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
    <p>这是一段普通的段落。</p>
</section>

## :root - 指定根元素

```css
:root {
    background-color: yellow;
}
```

## :empty - 指定没有子元素的元素

语法：

```html
<p>这是一段普通的段落。</p>
<p></p>
<p>这是一段普通的段落。</p>
```

```css
p:empty {
    height: 1em;
    background-color: yellow;
}
```

效果：

<section id="section_38">
    <p>这是一段普通的段落。</p>
    <p></p>
    <p>这是一段普通的段落。</p>
</section>

## :target - 指定的锚点链接

语法：

```html
<div>
    <a href="#段落一">跳转至段落一</a>
</div>
<div>
    <a href="#段落二">跳转至段落二</a>
</div>
<p id="段落一">段落一</p>
<p id="段落二">段落二</p>
```

```css
:target {
    background-color: yellow;
}
```

效果：

<section id="section_39">
    <div>
        <a href="#段落一">跳转至段落一</a>
    </div>
    <div>
        <a href="#段落二">跳转至段落二</a>
    </div>
    <p id="段落一">段落一</p>
    <p id="段落二">段落二</p>
</section>

## :enabled - 指定启用的输入元素

语法：

```html
<input type="text" name="foo">
<input type="text" name="bar">
```

```css
input:enabled {
    background-color: yellow;
}
```

效果：

<section id="section_40">
    <input type="text" name="foo">
    <input type="text" name="bar">
</section>

## :disabled - 指定禁用的输入元素

语法：

```html
<input type="text" name="foo">
<input type="text" name="bar" disabled="disabled">
```

```css
input:disabled {
    background-color: yellow;
}
```

效果：

<section id="section_41">
    <input type="text" name="foo">
    <input type="text" name="bar" disabled="disabled">
</section>

## :not(selector) - 指定非 selector 元素的元素

语法：

```html
<div>这是一段普通的段落。</div>
<p>这是一段普通的段落。</p>
```

```css
:not(p) {
    background-color: yellow;
}
```

效果：

<section id="section_42">
    <div>这是一段普通的段落。</div>
    <p>这是一段普通的段落。</p>
</section>

## ::selection - 被用户选中的区域

语法：

```css
::selection {
    background-color: yellow;
}
```

