# CSS 选择器

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

<style type="text/css">
    \.section\-class {
        background-color: yellow;
    }
</style>
<section>
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

<style type="text/css">
    \#section\-id {
        background-color: yellow;
    }
</style>
<section>
    <p id="section-id">这是一段普通的段落。</p>
</section>


## *

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

<style type="text/css">
    \#section\_ \* {
        background-color: yellow;
    }
</style>
<section id="section_">
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

<style type="text/css">
    \#section\_\_ p {
        background-color: yellow;
    }
</style>
<section id="section__">
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

<style type="text/css">
    \#section\_\_\_ div, \#section\_\_\_ p {
        background-color: yellow;
    }
</style>
<section id="section___">
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

<style type="text/css">
    \#section\_\_\_\_ div span {
        background-color: yellow;
    }
</style>
<section id="section____">
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
div span {
    background-color: yellow;
}
```

效果：

<style type="text/css">
    \#section\_\_\_\_\_ div \> span {
        background-color: yellow;
    }
</style>
<section id="section_____">
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

<style type="text/css">
    \#section\_\_\_\_\_\_ div + p {
        background-color: yellow;
    }
</style>
<section id="section______">
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

<style type="text/css">
    \#section\_\_\_\_\_\_\_ div ~ p {
        background-color: yellow;
    }
</style>
<section id="section_______">
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

<style type="text/css">
    \#section\_\_\_\_\_\_\_\_ a[target] {
        background-color: yellow;
    }
</style>
<section id="section________">
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

<style type="text/css">
    \#section\_\_\_\_\_\_\_\_\_ a[target=_blank] {
        background-color: yellow;
    }
</style>
<section id="section_________">
    <a href="https://github.com/" target="_blank">GitHub</a>
</section>