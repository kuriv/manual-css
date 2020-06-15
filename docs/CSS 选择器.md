# CSS 选择器

* [.class](#class)
* [#id](#id)
* [* 通配符](#通配符)
* [element](#element)
* [element, element]
* [element element]
* [element > element]

<link rel="stylesheet" type="text/css" href="CSS 选择器.css">

## .class

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

## #id

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

## * 通配符

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


## element

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


## element, element

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


## element element

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


## element > element

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


## element + element

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


## element ~ element

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


## [attribute]

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


## [attribute=value]

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


## [attribute~=value]

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


## [attribute|=value]

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


## [attribute^=value]

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


## [attribute$=value]

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


## [attribute*=value]

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


## :link

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


## :visited

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


## :hover

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


## :active

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


## :focus

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


## :lang(language)

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


## :before

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


## :after

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

## :first-letter



## :first-line



## :first-child



## :last-child



## :first-of-type



## :last-of-type



## :only-child



## :only-of-type



## :nth-child



## :nth-last-child



## :nth-of-type



## :nth-last-of-type