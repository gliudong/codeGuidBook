<a name="shorthand"></a>
## 4. 简写形式的属性声明

在需要显示地设置所有值的情况下，应当尽量限制使用简写形式的属性声明。常见的滥用简写属性声明的情况如下：
* padding
* margin
* font
* background
* border
* border-radius
当然合理的使用简写是一种良好的防御性编码方式，可以抵御未来的风险，例如以下

```css
.color {
  background: rebeccapurple;
}
.color {
  background-color: rebeccapurple;
}
```
前者是简写，可以确保得到一个纯色背景，而后者则有可能被background-image的图片替换

