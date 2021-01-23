# 介绍
在这里，将会介绍sass的一些基本属性，例如变量、嵌套、继承、复用以及函数。
[codepen链接](https://codepen.io/habsburger/pen/gOwJbJx)
## 变量
在sass中定义变量很简单，以下就是一个直接的例子：
```sass
$color = red
```
## 嵌套
现有如下html元素：
```html
<ul>
	<li>1</li>
	<li>2</li>
	<li>3</li>
</ul>
```
如果要选择li元素，css中的写法为：
```css
ul li {}
```
而sass中的写法为：
```sass
ul {
  li {
    &:first-child {
      // 选中第一个li
    }
  }
}
```
## 复用
mixin是可以重用的一组CSS声明，只需声明一次，就可在文件中引用。
```sass
@mixin center {
  text-align: center
}

p {
  @include center
}

@mixin style-link-text($color) {
  text-decoration: none
  color: $color
}

p {
  @include style-link-text(#eee)
}
```
## 函数
```sass
@function divide($a, $b) {
  @return $a / $b
}

p {
  font-size: divide(20, 2) * 1px
}
```
