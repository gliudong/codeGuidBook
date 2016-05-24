## 目录

[CSS](#css-principles)

* [语法](#css-syntax)
* [媒体查询的位置](#media)
* [单行规则声明](#single-declarations)
* [简写形式的属性声明](#shorthand)
* [注释](#comments)
* [选择器](#css-selectors)
<a name="html-syntax"></a>
## 1. 语法

* 用两个空格来代替制表符（tab） -- 这是唯一能保证在所有环境下获得一致展现的方法。
* 嵌套元素应当缩进一次（即两个空格）。
* 对于属性的定义，确保全部使用双引号，绝不要使用单引号。
* 不要省略可选的结束标签（closing tag）（例如，</li> 或 </body>）。

<a name="html-doctype"></a>
## 2. HTML5 doctype

为每个 HTML 页面的第一行添加标准模式（standard mode）的声明，这样能够确保在每个浏览器中拥有一致的展现。
```html-doctype
<!DOCTYPE html>
<html>
  <head>
  </head>
</html>
```

<a name="html-language"></a>
## 3. 语言属性

根据 HTML5 规范：

>强烈建议为 html 根元素指定 lang 属性，从而为文档设置正确的语言。这将有助于语音合成工具确定其所应该采用的发音，有助于翻译工具确定其翻译时所应遵守的规则等等。

更多关于 lang 属性的知识可以从 [此规范](http://w3c.github.io/html/semantics.html#the-html-element) 中了解。
```html
<html lang="zh-CN">
  <!-- ... -->
</html>
```

<a name="html-encode"></a>
## 4. 字符编码

通过明确声明字符编码，能够确保浏览器快速并容易的判断页面内容的渲染方式。这样做的好处是，可以避免在 HTML 中使用字符实体标记（character entity），从而全部与文档编码一致（一般采用 UTF-8 编码）。
```html
<head>
  <meta charset="UTF-8">
</head>
```

<a name="html-practicality"></a>
## 5. 实用为王

尽量遵循 HTML 标准和语义，但是不要以牺牲实用性为代价。任何时候都要尽量使用最少的标签并保持最小的复杂度。

<a name="html-reducing-markup"></a>
## 6. 减少标签的数量
编写 HTML 代码时，尽量避免多余的父元素。很多时候，这需要迭代和重构来实现。请看下面的案例：
```html
<!-- Not so great -->
<span class="avatar">
  <img src="...">
</span>

<!-- Better -->
<img class="avatar" src="...">
```
