# SASS

Sass是CSS预处理器，是CSS的扩展，为基本语言增添了力量和优雅

## 主要特征

- 变量：用于可重用的值，例如颜色，字体大小，间距等
- 嵌套：将选择器相互嵌套，使我们可以编写更少的代码
- 运算符：用于CSS内的数学运算
- 局部和导入：将CSS写入不同的文件并将它们全部导入到一个文件中
- Mixins：编写可重用的CSS代码
- 函数：类似于mixin，不同之处在于它们产生的值可以使用
- 继承：使不同的选择器继承所有选择器共同的声明
- 控制指令：用于使用条件和循环编写复杂的代码

## 示例语法

sass语法示例

```sass
.navigation
  list-style: none
  float: left
  
  & li
    display: inline-block
    margin-left: 30px
```

scss语法示例

```scss
.navigation {
  list-style: none;
  float: left;

  & li {
    display: inline-block;
    margin-left: 30px;
  }
}
```

