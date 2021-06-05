- less

  - 官网 http://lesscss.cn/

  - 注释

    - //不会暴露出去

    - /**/里的注释会暴露到css文件中

  - 变量

    - 使用@  定义

    - 实现代码复用，修改一个地方即可改变全部

    - 用法

      - 作为普通属性值使用

      - 作为选择器名和属性名

      - 作为URL

      - 变量的延迟加载

  - 嵌套规则

    - 不断嵌套，成为子选择器

    - 不想作为子选择器的定义，消除掉编译之后的空格：在前面加入&，作为平级使用

    - @ 规则（例如 @media 或 @supports）可以与选择器以相同的方式进行嵌套。@ 规则会被放在前面，同一规则集中的其它元素的相对顺序保持不变。这叫做冒泡（bubbling）

  - 混合

    - 在开头定义一个选择器及其样式，之后就可以在各个地方的样式中直接写该选择器的名字。在编译的时候就可以把定义好的样式编译出来，达到重复使用的效果

    - 将一系列属性从一个规则集引入到另一个规则集的方式

    - 分类

      - 普通混合

      - .juzhong()

      - 不带输出的混合

      - 带参数的混合

        - .juzhong(@w,@h,@c){    position:absolute;    background-color: @c;    width: @w;    height: @h;}

        - 使用时：.juzhong(100px,100px,pink)

      - 带参数且有默认值的混合
        - .juzhong(@w=100px,@h=100px,@c=pink){    position:absolute;    background-color: @c;    width: @w;    height: @h;}

      - 命名参数

        - 只想传入几个参数，但传入顺序未定时：

        - .juzhong(@c:blue)

      - 匹配模式
        - 引用另一个less文件：import""

      - arguments变量

  - 运算

    - 算术运算符 +、-、*、/ 可以对任何数字、颜色或变量进行运算。如果可能的话，算术运算符在加、减或比较之前会进行单位换算。计算的结果以最左侧操作数的单位类型为准。如果单位换算无效或失去意义，则忽略单位。无效的单位换算例如：px 到 cm 或 rad 到 % 的转换。

    - calc() 并不对数学表达式进行计算，但是在嵌套函数中会计算变量和数学公式的值。

  - 转义
    - 转义（Escaping）允许你使用任意字符串作为属性或变量值。任何 ~"anything" 或 ~'anything' 形式的内容都将按原样输出，除非 [interpolation](https://less.bootcss.com/features/#variables-feature-variable-interpolation)。

- sass

  - 变量

    - 变量声明

      - 使用$声明一个变量

      - $highlight-color: #F90;

      - 当变量定义在css规则块内，那么该变量只能在此规则块内使用。如果它们出现在任何形式的{...}块中（如@media或者@font-face块），情况也是如此

    - 变量引用

      - 凡是css属性的标准值（比如说1px或者bold）可存在的地方，变量就可以使用。

      - 在声明变量时，变量值也可以引用其他变量

    - 变量命名
      - 使用中划线的方式更为普遍

  - 嵌套css

    - sass在输出css时会帮你把这些嵌套规则处理好，避免你的重复书写。

    - 父选择器的标识符&

    - 群组选择器的嵌套

      - 当sass解开一个群组选择器规则内嵌的规则时，它会把每一个内嵌选择器的规则都正确地解出来：

      - .container {  h1, h2, h3 {margin-bottom: .8em}}

    - 子组合选择器和同层组合选择器 >  + ～

      - article {  ~ article { border-top: 1px dashed #ccc }  > section { background: #eee }  dl > {    dt { color: #333 }    dd { color: #555 }  }  nav + & { margin-top: 0 }}

      - sass会如你所愿地将这些嵌套规则一一解开组合在一起：

      - article ~ article { border-top: 1px dashed #ccc }article > footer { background: #eee }article dl > dt { color: #333 }article dl > dd { color: #555 }nav + article { margin-top: 0 }

    - 嵌套属性

      - nav {  border: {  style: solid;  width: 1px;  color: #ccc;  }}

      - 嵌套属性的规则是这样的：把属性名从中划线-的地方断开，在根属性后边添加一个冒号:，紧跟一个{ }块，把子属性部分写在这个{ }块中。就像css选择器嵌套一样，sass会把你的子属性一一解开，把根属性和子属性部分通过中划线-连接起来，最后生成的效果与你手动一遍遍写的css样式一样：

      - nav {  border-style: solid;  border-width: 1px;  border-color: #ccc;}

  - 导入sass文件

    - sass的@import规则在生成css文件时就把相关文件导入进来。这意味着所有相关的样式被归纳到了同一个css文件中，而无需发起额外的下载请求。

    - 使用部分

    - 默认变量值
      - !default用于变量，含义是：如果这个变量被声明赋值了，那就用它声明的值，否则就用这个默认值。

    - 嵌套导入
      - sass允许@import命令写在css规则内。这种导入方式下，生成对应的css文件时，局部文件会被直接插入到css规则内导入它的地方。

    - 原生的css导入

  - 静默注释
    - 静默注释，其内容不会出现在生成的css文件中。静默注释的语法跟JavaScriptJava等类C的语言中单行注释的语法相同，它们以//开头，注释内容直到行末。

  - 混合器

    - 混合器使用@mixin标识符定义。在你的样式表中通过@include来使用这个混合器，放在你希望的任何地方。@include调用会把混合器中的所有样式提取出来放在@include被调用的地方。

    - 何时使用
      - 在不停地重复一段样式，那就应该把这段样式构造成优良的混合器，尤其是这段样式本身就是一个逻辑单元，比如说是一组放在一起有意义的属性。

    - css规则

    - 传参
      - @mixin link-colors($normal, $hover, $visited) {  color: $normal;  &:hover { color: $hover; }  &:visited { color: $visited; }}

    - 默认参数值

      - 参数默认值使用$name: default-value的声明形式，默认值可以是任何有效的css属性值，甚至是其他参数的引用，

      - @mixin link-colors(    $normal,    $hover: $normal,    $visited: $normal  ){  color: $normal;  &:hover { color: $hover; }  &:visited { color: $visited; }}

  - 继承

    - 通过@extend语法实现

    - 何时使用

    - 继承的高级用法

    - 继承的工作细节

    - 最佳实践

- 参考

  - https://www.bilibili.com/video/av59710179/?p=3&spm_id_from=pageDriver

  - https://less.bootcss.com/

  - https://www.sass.hk/guide/