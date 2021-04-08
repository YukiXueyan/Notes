## intro

[TOC]



## Internet

### Internet是如何工作的

### HTTP

1. 从URL输入到返回请求的过程

   

   [参考：阿里面试官问“说一下从 url 输入到返回请求的过程”的难度就是不一样！](https://mp.weixin.qq.com/s?__biz=MzA4Nzg0MDM5Nw==&mid=2247493730&idx=1&sn=84243eb5ddcf2560618bfb2086a96a0a&chksm=9031eb80a74662968e7562a15c9637025dd00de20609f2a7c271b24abda6711423de545dfa44&mpshare=1&scene=23&srcid=0323s8a44g5c8ZEKQMoJbwUm&sharer_sharetime=1616491855557&sharer_shareid=383af18a6aef4a4861a0cc66f7ecde88#rd)

2. 状态码

3. 



### 浏览器及其工作方式

### DNS

### 域名

##  HTML

## 



1. img标签的title和alt

   title：鼠标覆盖上去显示的文字。

   alt:图片加载不出来的时候的占位字

2. meta标签

   https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/meta

   

   元数据（Metadata）是数据的数据信息。

   <meta> 标签提供了 HTML 文档的元数据。元数据不会显示在客户端，但是会被浏览器解析。


   META元素通常用于指定网页的描述，关键词，文件的最后修改时间，作者及其他元数据。

   元数据可以被使用浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他 Web 服务调用。

3. DOCTYPE标签

   <!DOCTYPE> 声明位于文档中的最前面的位置，处于 <html> 标签之前。


   <!DOCTYPE> 声明不是一个 HTML 标签；它是用来**告知 Web 浏览器页面使用了哪种 HTML 版本。**


   在 HTML 4.01 中，<!DOCTYPE> 声明需引用 DTD （文档类型声明），因为 HTML 4.01 是基于 SGML （Standard Generalized Markup Language 标准通用标记语言）。DTD 指定了标记语言的规则，确保了浏览器能够正确的渲染内容。

   HTML5 不是基于 SGML，因此不要求引用 DTD。

   **提示：**总是给您的 HTML 文档添加 <!DOCTYPE> 声明，确保浏览器能够预先知道文档类型。

4. W3C盒模型和怪异盒模型

   > 盒模型：外边距（margin）、边框（border）、内边距（padding）、实际内容（content）四个属性。
   >
   > W3C：width，height只是content的width和height，padding和margin的值另外计算。
   >
   > 怪异盒模型（IE）width = content+padding+border
   >
   > 定义了完整的doctype的标准文档类型，无论是哪种模型情况，最终都会触发标准模式，
   >
   > 如果doctype协议缺失，会由浏览器自己界定，在IE浏览器中IE9以下（IE6.IE7.IE8）的版本触发怪异模式，其他浏览器中会默认为W3c标准模式。

5. 懒加载和预加载

   > **懒加载也就是延迟加载。**
   > 当访问一个页面的时候，先把img元素或是其他元素的背景图片路径替换成一张大小为1*1px图片的路径（这样就只需请求一次，俗称占位图），只有当图片出现在浏览器的可视区域内时，才设置图片真正的路径，让图片显示出来。这就是图片懒加载。
   >
   > 懒加载的原理就是先在页面中把所有的图片统一使用一张占位图进行占位，把真正的路径存在元素的“data-url”（这个名字起个自己认识好记的就行）属性里，要用的时候就取出来，再设置
   >
   > 实现步骤
   >
   > 1)首先，不要将图片地址放到src属性中，而是放到其它属性(data-original)中。
   > 2)页面加载完成后，根据scrollTop判断图片是否在用户的视野内，如果在，则将data-original属性中的值取出存放到src属性中。
   > 3)在滚动事件中重复判断图片是否进入视野，如果进入，则将data-original属性中的值取出存放到src属性中。
   >
   > 优点：页面加载速度快，减轻服务器的压力
   >
   > -
   >
   > **预加载：提前加载图片，当用户需要查看时可直接从本地缓存中渲染**
   >
   > 图片预先加载到浏览器中，访问者便可顺利地在你的网站上冲浪，并享受到极快的加载速度。这对图片画廊及图片占据很大比例的网站来说十分有利，它保证了图片快速、无缝地发布，也可帮助用户在浏览你网站内容时获得更好的用户体验。
   >
   > ### 3.实现预加载的方法有哪些？
   >
   > 方法一：用CSS和JavaScript实现预加载
   > 方法二：仅使用JavaScript实现预加载
   > 方法三：使用Ajax实现预加载

6. 减少DOM操作是什么

7. 渐进增强与优雅降级

8. img 的 alt 与 title 有何异同？ strong 与 em 的异同？ 

   a:alt(alt text):为不能显示图像、窗体或 applets 的用户代理（UA），alt 属性用来指 定替换文字。替换文字的语言由 lang 属性指定。(在 IE 浏览器下会在没有 title 时把 alt 当成 tool tip 显示) title(tool tip):该属性为设置该属性的元素提供建议性的信息。 strong:粗体强调标签，强调，表示内容的重要性 em:斜体强调标签，更强烈强调，表示内容的强调点

9. 行内元素和块级元素

   > 内联元素(inline element) 
   >
   > a – 锚点 
   >
   > abbr – 缩写 
   >
   > acronym – 首字 
   >
   > b – 粗体(不推荐) 
   >
   > big – 大字体 
   >
   > br – 换行 
   >
   > em – 强调 
   >
   > font – 字体设定(不推荐) 
   >
   > i – 斜体 
   >
   > img – 图片 
   >
   > input – 输入框 
   >
   > label – 表格标签 
   >
   > s – 中划线(不推荐) 
   >
   > select – 项目选择 
   >
   > small – 小字体文本 
   >
   > span – 常用内联容器，定义文本内区块 
   >
   > strike – 中划线 
   >
   > strong – 粗体强调 
   >
   > sub – 下标 
   >
   > sup – 上标 
   >
   > textarea – 多行文本输入框 
   >
   > tt – 电传文本 
   >
   > u – 下划线 
   >
   > var – 定义变量 
   >
   > 2、块级元素 
   >
   > address – 地址 
   >
   > blockquote – 块引用 
   >
   > center – 举中对齐块 
   >
   > dir – 目录列表 
   >
   > div – 常用块级容易，也是 css layout 的主要标签 
   >
   > dl – 定义列表 
   >
   > fieldset – form 控制组 
   >
   > form – 交互表单 
   >
   > h1 – 大标题 
   >
   > h2 – 副标题 
   >
   > h3 – 3 级标题 
   >
   > h4 – 4 级标题 
   >
   > h5 – 5 级标题 
   >
   > h6 – 6 级标题 
   >
   > hr – 水平分隔线 
   >
   > isindex – input promptmenu – 菜单列表 
   >
   > noframes – frames 可选内容，（对于不支持 frame 的浏览器显示此区块内容） 
   >
   > noscript – ）可选脚本内容（对于不支持 script 的浏览器显示此内容） 
   >
   > ol – 排序表单 
   >
   > p – 段落 
   >
   > pre – 格式化文本 
   >
   > table – 表格 
   >
   > ul – 非排序列表 

10. **浏览器标准模式和怪异模式之间的区别是什么？** 

    标准模式是指，浏览器按 W3C 标准解析执行代码； 

    怪异模式则是使用浏览器自己的方式解析执行代码，因为不同浏览器解析执行的方式不一 样，所以我们称之为怪异模式。浏览器解析时到底使用标准模式还是怪异模式，与你网页中的 DTD 声明直接相关，DTD 声 明定义了标准文档的类型（标准模式解析）文档类型，会使浏览器使用相应的方式加载网页并显示，忽略 DTD 声明,将使网页进入怪异模式


## CSS

### 引入

1. link和@import的区别

   > Link 属于 html 标签，而@import 是 CSS 中提供的 
   >
   > 在页面加载的时候，link 会同时被加载，而@import 引用的 CSS 会在页面加载完成后才会加 
   >
   > 载引用的 CSS 
   >
   > @import 只有在 ie5 以上才可以被识别，而 link 是 html 标签，不存在浏览器兼容性问题 
   >
   > Link 引入样式的权重大于@import 的引用（@import 是将引用的样式导入到当前的页面中）

2. 



### 选择器

**CSS 选择符有哪些？哪些属性可以继承？优先级算法如何计算？ CSS3 新增** 

**伪类有那些？** 

\* 

1.id 选择器（ # myid） 

2.类选择器（.myclassname） 

3.标签选择器（div, h1, p） 

4.相邻选择器（h1 + p） 

5.子选择器（ul < li） 

6.后代选择器（li a） 

7.通配符选择器（ * ） 

8.属性选择器（a[rel = "external"]） 

9.伪类选择器（a: hover, li: nth - child） 

\* 

可继承： font-size font-family color, UL LI DL DD DT; 

\* 

不可继承 ：border padding margin width height ; 

\* 

优先级就近原则，样式定义最近者为准; 

\* 

载入样式以最后载入的定位为准; 

优先级为:

!important > 

id > class > tag 

important 比 内联优先级高 

CSS3 新增伪类举例： 

p:first-of-type 选择属于其父元素的首个 <p> 元素的每个 <p> 元素。 

p:last-of-type 

选择属于其父元素的最后 <p> 元素的每个 <p> 元素。 

p:only-of-type 

选择属于其父元素唯一的 <p> 元素的每个 <p> 元素。 

p:only-child 

选择属于其父元素的唯一子元素的每个 <p> 元素。 

p:nth-child(2) 

选择属于其父元素的第二个子元素的每个 <p> 元素。 

:enabled、:disabled 控制表单控件的禁用状态。 

:checked，单选框或复选框被选中。 



**伪类**选择元素基于的是当前元素处于的状态，或者说元素当前所具有的特性，而不是元素的id、class、属性等静态的标志。由于状态是动态变化的，所以一个元素达到一个特定状态时，它可能得到一个伪类的样式；当状态改变时，它又会失去这个样式。由此可以看出，它的功能和class有些类似，但它是基于文档之外的抽象，所以叫伪类。

与伪类针对特殊状态的元素不同的是，**伪元素**是对元素中的特定内容进行操作，它所操作的层次比伪类更深了一层，也因此它的动态性比伪类要低得多。实际上，设计伪元素的目的就是去选取诸如元素内容第一个字（母）、第一行，选取某些内容前面或后面这种普通的选择器无法完成的工作。它控制的内容实际上和元素是相同的，但是它本身只是基于元素的抽象，并不存在于文档中，所以叫伪元素。

### 盒模型

`box-sizing: content-box`（W3C盒模型，又名标准盒模型）：元素的宽高大小表现为内容的大小。 `box-sizing: border-box`（IE盒模型，又名怪异盒模型）：元素的宽高表现为内容 + 内边距 + 边框的大小。背景会延伸到边框的外沿。



1. BFC的概念

   > **块格式化上下文（Block Formatting Context，BFC）** 是Web页面的可视CSS渲染的一部分，是块盒子的布局过程发生的区域，也是浮动元素与其他元素交互的区域。
   >
   > W3C CSS 2.1 规范中的一个概念,它是一个独立容器，**决定了元素如何对其内容进行定位,以及与其他元素的关系和相互作用**。）
   > 一个页面是由很多个 Box 组成的,元素的类型和 display 属性,决定了这个 Box 的类型。
   > 不同类型的 Box,会参与不同的 Formatting Context（决定如何渲染文档的容器）,因此Box内的元素会以不同的方式渲染,也就是说BFC内部的**元素和外部的元素不会互相影响。**

2. 解释盒子模型

   >  CSS中组成一个块级盒子需要:
   >
   >  - **Content box**: 这个区域是用来显示内容，大小可以通过设置 [`width`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/width) 和 [`height`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/height).
   >  - **Padding box**: 包围在内容区域外部的空白区域； 大小通过 [`padding`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/padding) 相关属性设置。
   >  - **Border box**: 边框盒包裹内容和内边距。大小通过 [`border`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/border) 相关属性设置。
   >  - **Margin box**: 这是最外面的区域，是盒子和其他元素之间的空白区域。大小通过 [`margin`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/margin) 相关属性设置。

3. 普通盒模型和怪异盒模型

   > 在标准模型中，如果你给盒设置 `width` 和 `height`，实际设置的是 *content box*。 padding 和 border 再加上设置的宽高一起决定整个盒子的大小。 
   >
   > 使用这个模型，所有宽度都是可见宽度，所以内容宽度是该宽度减去边框和填充部分。使用上面相同的样式得到 (width = 350px, height = 150px).



### 定位 position

https://developer.mozilla.org/zh-CN/docs/Web/CSS/position_value

- **static** ：HTML 元素的默认值，即没有定位，遵循正常的文档流对象。静态定位的元素不会受到 top, bottom, left, right影响。
- **relative** ：相对定位元素的定位是相对其正常位置。
- **fixed**   ：相对于浏览器窗口是固定位置，窗口滚动也不会移动
- **absolute**：绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于`<html>`:
- **sticky**: 基于用户的滚动位置来定位。

z-index  指定堆叠顺序。数字越大越在前面。

position 的取值 

> static，relative，absolute，fixed
>
> | [absolute](https://www.runoob.com/css/css-positioning.html#position-absolute) | 生成绝对定位的元素，相对于 static 定位以外的第一个父元素进行定位。元素的位置通过 "left", "top", "right" 以及 "bottom" 属性进行规定。 |
> | ------------------------------------------------------------ | ------------------------------------------------------------ |
> | [fixed](https://www.runoob.com/css/css-positioning.html#position-fixed) | 生成固定定位的元素，相对于浏览器窗口进行定位。元素的位置通过 "left", "top", "right" 以及 "bottom" 属性进行规定。 |
> | [relative](https://www.runoob.com/css/css-positioning.html#position-relative) | 生成相对定位的元素，相对于其正常位置进行定位。因此，"left:20" 会向元素的 LEFT 位置添加 20 像素。 |
> | [static](https://www.runoob.com/css/css-positioning.html#position-static) | 默认值。没有定位，元素出现在正常的流中（忽略 top, bottom, left, right 或者 z-index 声明）。 |
> | [sticky](https://www.runoob.com/css/css-positioning.html#position-sticky) | 粘性定位，该定位基于用户滚动的位置。它的行为就像 position:relative; 而当页面滚动超出目标区域时，它的表现就像 position:fixed;，它会固定在目标位置。**注意:** Internet Explorer, Edge 15 及更早 IE 版本不支持 sticky 定位。 Safari 需要使用 -webkit- prefix (查看以下实例)。 |
> | inherit                                                      | 规定应该从父元素继承 position 属性的值。                     |



### 布局

#### float

- 

1. 清除浮动：

```css
.clear{
    clear:both;
}
```

2. 浮动有什么问题



#### flex



#### grid



### 新特性

#### 边框

#### 背景

#### 渐变

#### 文本和字体

#### 2D/3D转换

#### 过渡

#### 动画







1. CSS动画，transition和animation区别

   > `transition`属性可以被指定为一个或多个 CSS 属性的过渡效果，多个属性之间用逗号进行分隔。
   >
   > `animation` 属性用来指定一组或多组动画，每组之间用逗号相隔。
   >
   > transition： 强调过渡；
   > 需要触发一个事件，比如鼠标移上去、焦点、点击。
   >
   > animation：多个关键帧，实现自由动画；
   > 不需要触发任何事件也可随时间变化达到一种动画效果；
   > 与transition不同是animation可以通过@keyframe控制当前帧属性，更灵活。

2. 

### 响应式设计

@media 规则允许在相同样式表为不同媒体设置不同的样式。



## JavaScript

### 基础

- 区分大小写

#### 关键字



#### 数据类型

#### 变量

1. 什么是值？什么是类型？什么是变量？ 它们之间的区别和联系？

> 值：
>
> 变量是数据的命名存储，只有定义了变量，值才有意义。
>
> 类型是值的类型，不同的类型有不同的方法

2. let，const，var 三者的本质不同是什么？为什么不推荐使用 var

   > var:
   >
   > ​	支持变量声明与解析，不支持块级作用域，允许重复声明。“var” 声明的变量，可以在其声明语句前被使用("提升")，但是赋值不会提升。
   >
   > ​	if (true) {  var test = true; // 使用 "var" 而不是 "let" } *alert(test); // true，变量在 if 结束后仍存在*
   >
   > let：
   >
   > ​	不支持变量声明与解析，支持块级作用域，不允许重复声明。用let声明的变量只会在代码块中有效。
   >
   > `if (true) {  let test = true; // 使用 "let" } *alert(test); // Error: test is not defined*
   >
   > const:
   >
   > ​	不支持变量声明与解析，支持块级作用域，不允许重复声明，声明变量一旦确定就**不允许被修改**。因此声明变量必须赋值，不能像var一样声明再在定义。
   >
   > 对同一个变量（let和const声明的）进行重复声明会触发 error

   

#### 作用域

- LHS ,RHS

##### 词法作用域

- 逐级嵌套
- eval（） 接受一个字符串作为参数，将其中的内容视为代码语句
- with 重复引用同一个对象中的多个属性的快捷方式，不需要重复引用对象本身。
- eval(...)和with，会使代码变慢：引擎不发在词法分析阶段明确知道eval(...)会接收到什么样的代码，这些代码如何对作用域进行修改，也无法知道with用来创建新词法作用域的对象的内容是什么

##### 函数作用域、块作用域

块作用域：`for(){};if(){}`

变量的声明距离使用的地方越近越好，并最大限度本地化。



1. 作用域的本质是什么？闭包和作用域的关系是什么？

   > 作用域的本质是词法环境。可以对数据进行操作的空间。
   >
   > 闭包是一个函数在创建时允许自身函数访问并操作该自身函数之外的变量时所创建的作用域。闭包可以让函数访问所有的变量和函数，只要这些变量和函数都存在于该函数声明时的作用域中就行。

2. js的作用域分为哪几类，作用域大小怎么定义？ 

   > 全局作用域
   >
   > 函数作用域 function x(){}
   >
   > 块级作用域 if{}

#### 操作符

1. == 的判断逻辑是什么？

   > ==  转化成数字，再比较大小。

#### 语句

#### 条件

#### 循环



### 基本类型

- typeof [1,2,3]输出什么？那js如何判断数组

  > object
  >
  > 判断数组：isArray()

- typeof String(“asdfasdf”)

  > string

- 

#### null

注意：`typeof null === "object";//true`

#### undefined

undefined  是值的一种，表示未赋值。undecleard表示变量未定义。

#### boolean

#### number

#### String

#### symbol

 

1. js数据基本类型说一下，number和其他语言有什么不同 

   > js数据基本类型有字符串（String）、数字(Number)、布尔(Boolean)、对空（Null）、未定义（Undefined）、Symbol。
   >
   > (**引用数据类型**：对象(Object)、数组(Array)、函数(Function)。)
   >
   > JavaScript 只有一种数字类型。数字可以带小数点，也可以不带.其他语言还需要区分整数、浮点数等。

2. 判断数据类型有哪些方式 

   1. typeof()

   2. `===`

   3. instanceof    `A instanceof B`,instanceof 检测的是原型

   4. constructor

   5. toString

      https://www.cnblogs.com/onepixel/p/5126046.html

3. 

### 引用类型



#### object

- 创建

  `var person  = new Object();person.age = 23;person.name = "May"`

  `var person  = {};person.age = 23;person.name = "May"`

  或

  ````javascript
  var person = {
  name : "May",
  age : 23
  };
  ````

  

- 访问对象属性

  - 点表示法：使用变量来访问属性，属性中可以有空格
  - 方括号表示法



- new的过程

  > • 创建一个空对象，将它的引用赋给 this，继承函数的原型。
  > • 通过 this 将属性和方法添加至这个对象
  > • 最后返回 this 指向的新对象，也就是实例（如果没有手动返回其他的对象）

- Object.create()的内部原理

- 实现一个sleep函数

- reduce将一个对象数组合并成一个对象

- Object.freeze()如何冻结对象

#### Array

- 创建

  ```javascript
  var color = new Array()
  //设置长度
  var color = new Array(20)
  //嵌入包含的项
  var color = new Array("red","yellow","blue")
  //省略new也行
  var color = Array()
  
  var color = ["red","yellow","blue"]
  var color = []
  ```

- 修改数组

  - 访问数组时，如果索引超过了数组的现有项数，那么数组会自动增加length到该索引+1的长度。新增的每一项都是undefined。
  - 设置length如果设为大于原来的length，数组会自动增加length到该索引+1的长度。新增的每一项都是undefined。
  - 设置length如果设为小于原来的length，数组移除多余的项
  - 向末尾增加新的项：`arr[arr.length] = "x"`

- 检测数组

  instanceof  `arr instanceof Array`

  `Array.isArray(value)`

- 转换

  - toLocaleString()
  - toString()
  - ValueOf()
  - join()   以不同的分隔符构建字符串

- 栈方法

  - pop()移除最后一项，并返回
  - push()  添加到数组末尾

- 队列方法

  - shift() 移除数组中的第一个并返回该项
  - unshift()  在前端添加任意个项，并返回长度

- 重排序

  - reverse()   倒序

  - sort()  按字符串排序

    - 按值排序：

      ```javascript
      val arr = [1,2,3,9,8,7,6,5]
      function compare(x1,x2){
      return x2-x1;
      }
      arr.sort(compare)
      ```

      

- 操作方法

  - concat()  基于当前数组，创建一个新数组。先创建当前数组的一个副本，将接收到的参数添加到副本的末尾，最后返回该副本
  - slice() 基于当前数组的一项或多项创建一个新数组，不会影响原始数组。两个参数：起始索引和结束索引。当只有一个参数时，默认从起始索引开始到数组的末尾。
  - splice()  
    - 删除splice(0,2)  从索引为0的地方开始，删除2项
    - 插入 splice(2,0,"x","y") 从索引为2的地方开始，在后面插入
    - 替换splice(2,1,"x","y")从索引为2的地方开始，删除1项，在后面插入

- 位置方法

  - indexOf()
  - lastIndexOf()

- 迭代：参数：要在每一项运行的函数和（可选）运行在该函数上的作用域对象

  - every()：对数组的每一项运行给定函数，如果函数对**每一项都返回true，则返回true**
  - filter()：对数组的每一项运行给定函数，返回该函数中会返回true的项形成的**数组**
  - forEach()：对数组的每一项运行给定函数，没有返回值
  - map()：对数组的每一项运行给定函数，返回每次函数的调用结果形成的数组
  - some()：对数组的每一项运行给定函数，任一项返回true，则返回true

  以上方法都不会修改数组的值

- 缩小方法：遍历所有项，返回一个最终值

  - reduce()从前往后
  - reduceRight()：从后往前

1. [数组去重](https://segmentfault.com/a/1190000016418021)

- 实现数组的slice方法

  > ```javascript
  > Array.prototype.slice2 = function (start, end) {
  > let len = this.length;
  > let l = start === undefined ? 0 : start < 0 ? Math.max(start + len, 0) : Math.min(start, len);
  > let r = end === undefined ? len : end < 0 ? Math.max(end + len, 0) : Math.min(end, len);
  > const res = [];
  > while (l < r) {
  >  res.push(this[l++])
  > }
  > return res;
  > }
  > ```

3. 数组的本质是什么，运用了什么样的设计模式？数组和对象的关系是什么？

   > 数组的本质是一种特殊的对象

4. 判断数组有哪些方法

   > 1. arr.isArray()  ---ES5
   > 2. arr.constructor === Array
   > 3. Object.prototype.toString.call(obj) == "[object Array]"   原生对象的toString检测

5. 求两个数组的交集和并集

   > 使用Set(),解构赋值，filter，has()
   >
   > ```javascript
   > let a = new Set([1, 2, 3]);
   > let b = new Set([4, 3, 2]);
   > 
   > // 并集
   > let union = new Set([...a, ...b]);
   > // Set {1, 2, 3, 4}
   > 
   > // 交集
   > let intersect = new Set([...a].filter(x => b.has(x)));
   > // set {2, 3}
   > 
   > // 差集
   > let difference = new Set([...a].filter(x => !b.has(x)));
   > // Set {1}
   > ```
   >
   > 

   

#### Date

`var now = new Date()`

- Date.parse()  接收日期的字符串，返回毫秒
- Date.UTC(年份，基于0的月份，月中的哪一天，小时，分钟，秒，毫秒)。其他参数省略：则返回0

| 方法                   | 说明                                                         |
| ---------------------- | ------------------------------------------------------------ |
| getTime()              | 返回表示日期的毫秒数;与valueOf()方法返回的值相同             |
| setTime()              | 以毫秒数设置日期,会改变整个日期                              |
| getFullYear ( )        | 取得4位数的年份（如2007而非仅07)                             |
| getUTCFullYear()       | 返回UTC日期的4位数年份                                       |
| setFullYear()          | 设置日期的年份。传入的年份值必须是4位数字（如2007而非仅07)   |
| getMonth()             | 返回日期中的月份，其中0表示一月，11表示十二月                |
| getUTCMonth ( )        | 返回UTC日期中的月份，其中0表示一月，11表示十二月             |
| setMonth(月)           | 设置日期的月份。传入的月份值必须大于0、超过11则增加年份      |
| setUTCMonth(月)        | 设置UTC日期的月份。传人的月份值必须大于0，超过11则增加年份   |
| getDate()              | 返回日期月份中的天数〔 1到31                                 |
| getUTCDate()           | 返回UTC日期月份中的天数（ 1到31)                             |
| setDate (日)           | 设置日期月份中的天数。如果传入的值超过了该月中应有的天数，则增加月份 |
| setUTCDate(日)         | 设置UTC日期月份中的天数。如果传入的值超过了该月中应有的天数,则增加月份 |
| getDay ()              | 返回日期中星期的星期几(其中0表示星期日，6表示星期六)         |
| getUTCDay ()           | 返回UTC日期中星期的星期几（其中0表示星期日，6表示星期六)     |
| getHours ( )           | 返回日期中的小时数〔0到23)                                   |
| getUTCHours ( )        | 返回UTC日期中的小时数（ 0到23)                               |
| setHours(时)           | 设置日期中的小时数。传入的值超过了23则增加月份中的天数       |
| setUTCHours(时)        | 设置UTC日期中的小时数。传人的值超过了23则增加月份中的天数    |
| getMinutes ( )         | 返回日期中的分钟数（0到59)                                   |
| getUTCMinutes ()       | 返回UTC日期中的分钟数（0到59)                                |
| setMinutes(分)         | 设置日期中的分钟数。传入的值超过59则增加小时数               |
| setUTCMinutes(分)      | 设置UTC日期中的分钟数。传入的值超过59则增加小时数            |
| getSeconds ( )         | 返回日期中的秒数（0到59)                                     |
| getUTCSeconds ( )      | 返回UTC日期中的秒数（0到59                                   |
| setseconds (秒)        | 设置日期中的秒数。传入的值超过了59会增加分钟数               |
| setUTcSeconds(秒)      | 设置UTC日期中的秒数。传入的值超过了59会增加分钟数            |
| getMil1iseconds ( )    | 返回日期中的毫秒数                                           |
| getUTCMilliseconds ( ) | 返问UTC日期中的毫秒数                                        |
| setMilliseconds (毫秒) | 设置日期中的毫秒数                                           |







#### RegExp

正则表达式

`var expression = /pattern/flags`

- 实例属性
  - global ：布尔值，是否设置了g标志
  - ignoreCase： 布尔值，是否设置了i标志
  - lastIndex: 整数，表示开始搜索下一个匹配项的字符位置，从0开始
  - multiline 布尔值，是否设置了m标志
  - source 正则表达式的字符串表示
- 实例方法
  - exec() :接收要匹配的字符串，返回第一个匹配信息的数组。没有就返回null
- 构造函数属性



1. 引用类型有哪几种？简单类型呢？

   > 引用类型：object，array,Date,RegExp,Function
   >
   > 简单类型：number , string, boolean,symbol,null,undefined

2. 对对象进行遍历有哪些方法？ 

   > `for(let key in obj)` 循环。

### 函数

每一个函数都是function的实例，都与其他引用类型有一样的属性和方法。

函数是对象，因此函数名也是一个指向函数对象的指针，不会与某个函数绑定。

- 没有重载
  - 两个同名函数，后一个会覆盖前一个函数

#### 函数声明

```javascript
//函数声明
alert(sun(10,10));
function sum(x,y){
return x+y;
```

解析器会先读取函数声明，并使其在执行任何代码之前可以访问。

**声明提升**

1. JS变量提升和函数提升的定义、区别

   > 你不知道的JavaScript（上）

2. 

#### 函数表达式

```javascript
//函数表达式
alert(sun(10,10));
var sum = function(x,y){
return x+y;
}
```

函数表达式必须要等到解析器执行到其所在的代码行，才可以被解释执行

#### callee

内部属性

- arguments，this

- callee 指向拥有这个arguments对象的函数 `arguments.callee(x)`

- 实现递归

  ```javascript
   function factorial(num){
                  if (num <= 1){
                      return 1;
                  } else {
                      return num * arguments.callee(num-1);
                  }
              }
  
              var anotherFactorial = factorial;
              factorial = null;
              alert(anotherFactorial(4));  //24
  ```

  

#### 属性和方法

- 属性：length，prototype
- 方法: call(),apply(),bind()



#### call()方法/apply()方法



区别：，`call()`和`apply()`的不同点就是**接收参数的方式不同**。

- **apply()方法**接收两个参数，一个是函数运行的作用域（`this`），另一个是参数数组。
- **call()方法**不一定接受两个参数，第一个参数也是函数运行的作用域（`this`），但是传递给函数的参数必须列举出来。



作者：幽小鬼
链接：https://www.jianshu.com/p/625c35d84a80
来源：简书
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。

#### Function（）构造器

#### 闭包

闭包是指有权访问另一个函数作用域中的变量的函数。

创建闭包的常用方式：在一个函数内部创建另一个函数。

闭包只能取得包含函数中任何变量的最后一个值。

```javascript
function createFunctions(){
	var result = new Array();
    for (var i=0; i < 10; i++){
        result[i] = function(){
        	return i;
        };
    }
	return result;
}
var funcs = createFunctions();
//every function outputs 10
for (var i=0; i < funcs.length; i++){
	document.write(funcs[i]() + "<br />");
}//i打印出来都是10

function createFunctions(){
    var result = new Array();

    for (var i=0; i < 10; i++){
        result[i] = function(num){
            return function(){
                return num;
            };
        }(i);
    }

    return result;
}

var funcs = createFunctions();

//every function outputs 10
for (var i=0; i < funcs.length; i++){
    document.write(funcs[i]() + "<br />");
}//i有不同的取值


```



1. 闭包的优缺点：

   - 优点：重复使用变量，不会造成变量污染。可以用来定义私有属性和方法
   - 缺点：比普通函数更占内存，导致网页性能变差或内存泄漏————内存泄漏的解决：在退出函数之前，将不用的全局变量删除，或者赋值为null。or 避免变量的循环赋值和引用

   闭包 https://www.jianshu.com/p/d903be89f211

2. 闭包

   > 闭包：有权访问另一个函数作用域中的变量的函数。
   >
   > 创建闭包：在一个函数内部创建另一个函数

3. 作用域链，那么如果在一个函数a里面定义了一个变量，要在b函数里面访问ａ里面的私有变量有什么方式吗？

   > 在a函数内部声明b函数

#### 匿名函数

```javascript
function(){}
```

没有名称标识符的函数。

函数表达式可以匿名，函数声明不可以。

缺点：

- 匿名函数在栈追踪中不会显示出有意义的函数名，这使调试变得困难。
- 没有函数名，需要引用自身时只能使用arguments.callee()
- 可读性差

立即执行函数表达式IIFE：

函数被包含在括号内部，成为一个表达式，在末尾加上一个（）就可以立即执行这个函数。

普遍用法：

- 当做函数调用并传递参数进去。
- 倒置代码的运行顺序



#### 箭头函数



1. 箭头函数与普通函数的区别（this和new）

   > **箭头函数是普通函数的简写，可以更优雅的定义一个函数，和普通函数相比，** 
   >
   > **有以下几点差异：** 
   >
   > 函数体内的 this 对象，就是定义时所在的对象，而不是使用时所在的对 
   >
   > 象。 
   >
   > 不可以使用 arguments 对象，该对象在函数体内不存在。如果要用，可 
   >
   > 以用 rest 参数代替。 
   >
   > 不可以使用 yield 命令，因此箭头函数不能用作 Generator 函数。 
   >
   > 不可以使用 new 命令，因为： 
   >
   > 1.没有自己的 this，无法调用 call，apply。 
   >
   > 2.没有 prototype 属性 ，而 new 命令在执行时需要将构造函数的 prototype 赋值给新的对象的 __proto__

2. 箭头函数是用来解决什么问题的？

   > 箭头函数是针对那些没有自己的“上下文”，但在当前上下文中起作用的短代码的。
   >
   > 箭头函数：
   >
   > - 没有 `this`
   > - 没有 `arguments`
   > - 不能使用 `new` 进行调用
   > - 它们也没有 `super`

#### 函数参数

#### 函数调用

#### this 

this提供了一种“隐式”传递对象引用的方式，可以将API设计得更加简洁且易于复用。

this实际上是函数被调用时发生的绑定，它指向什么取决于函数在哪里被调用。

判断this的绑定对象：

- 由new调用：绑定到新创建的对象

- call或apply调用：绑定到指定的对象

- 上下文对象调用：绑定到该上下文对象

  

  ```javascript
  function foo(){
  console.log(this.a)
  }
  var obj2 = {
      a:42;
      foo:foo;
  }
  var obj1 = {
      a:2;
      obj2:obj2;
  }
  obj1.obj2.foo();//42
  ```

- 默认：严格模式——undefined；否则——全局对象

  ```javascript
  function foo(){
  console.log(this.a)
  }
  var a = 2;
  foo();//2
  ```

  

1. 下列代码的输出

   ```javascript
       var length = 10;
       function fn() {
       return this.length+1;
       }
       var obj = {
       length: 5,
       test1: function() {
       return fn();
       
       },
       test3:fn()
       };
       obj.test2=fn;
       //下面代码输出是什么
       console.log(obj.test1())//11
   
       console.log(fn()===obj.test2()) //false
       console.log(obj.test2()) //6
   ```

   

2. 



#### 函数柯里化



### 对象

#### 基础概念

- 属性
- 方法
- 数据属性 
  - 修改属性默认的特性：Object.defineProperty(属性所在的对象，属性的名字，描述符对象)
  - 描述符对象：
    - configurable——能否通过delete删除属性从而重新定义属性，能否修改属性的特性，能否把属性修改为访问器属性。（默认：true）
    - enumerable——能否通过for-in返回属性。（默认：true）
    - writeable——能否修改属性的值。（默认：true）
    - value——包含该属性的数据值。（默认：undefined）
    - 调用Object.defineProperty后，configurable，enumerable，writeable默认是false

##### 访问器属性

getter() ,setter()



定义多个属性：Object.defineProperties()

读取属性的特性：Object.getOwnpropertyDescriptor()

#### 对象创建

- 工厂模式

  用函数封装接口来创建对象

  ```javascript
  function createPerson(name, age, job){
              var o = new Object();
              o.name = name;
              o.age = age;
              o.job = job;
              o.sayName = function(){
                  alert(this.name);
              };    
              return o;
          }
          
          var person1 = createPerson("Nicholas", 29, "Software Engineer");
          var person2 = createPerson("Greg", 27, "Doctor");
  ```

  

- 构造器模式

  - 没有显式地创建对象
  - 直接将属性和方法赋给this
  - 没有return

  ```javascript
  function Person(name, age, job){
              this.name = name;
              this.age = age;
              this.job = job;
              this.sayName = function(){
                  alert(this.name);
              };    
          }
          
          var person1 = new Person("Nicholas", 29, "Software Engineer");
          var person2 = new Person("Greg", 27, "Doctor");
  ```

  步骤：

  - 创建一个新对象
  - 将作用域赋给新对象
  - 执行构造函数的代码
  - 返回新对象

- 原型模式

  ```javascript
  function object(o){
              function F(){}
              F.prototype = o;
              return new F();
          }
          
          var person = {
              name: "Nicholas",
              friends: ["Shelby", "Court", "Van"]
          };
          
          var anotherPerson = object(person);
          anotherPerson.name = "Greg";
          anotherPerson.friends.push("Rob");
          
          var yetAnotherPerson = object(person);
          yetAnotherPerson.name = "Linda";
          yetAnotherPerson.friends.push("Barbie");
          
          alert(person.friends);   //"Shelby,Court,Van,Rob,Barbie"
  ```

  

- 其他组合或演进模式



手写new：

> ```javascript
> function myNew (fn, ...args) {
> let instance = Object.create(fn.prototype);
> let result = fn.call(instance, ...args)
> return typeof result === 'object' ? result : instance;
> }
> ```



#### 继承

P162

- 原型链继承

  - 利用原型让一个引用类型的对象继承另一个引用类型的属性和方法。层层递进，构成了实例与原型的链条——原型链

  - ```javascript
    function SuperType(){
               this.property = true;
           }
           
           SuperType.prototype.getSuperValue = function(){
               return this.property;
           };
           
           function SubType(){
               this.subproperty = false;
           }
           
           //inherit from SuperType
           SubType.prototype = new SuperType();
           
           SubType.prototype.getSubValue = function (){
               return this.subproperty;
           };
           
           var instance = new SubType();
           alert(instance.getSuperValue());   //true
    ```

  - 给原型添加方法的代码要写在替换原型的语句之后。

  - 存在问题：

    - 引用类型值
    - 在创建子类型的实例时，不能向超类型的构造函数中传递参数。

- 构造继承

  - ```javascript
    function SuperType(){
                this.colors = ["red", "blue", "green"];
            }
    
            function SubType(){  
                //inherit from SuperType
                SuperType.call(this);
            }
    
            var instance1 = new SubType();
            instance1.colors.push("black");
            alert(instance1.colors);    //"red,blue,green,black"
            
            var instance2 = new SubType();
            alert(instance2.colors);    //"red,blue,green"
    ```

  - 优势在于：可以在子类型构造函数中向超类型构造函数传递参数

- 组合继承

  - 将原型链和借用构造函数的技术组合到一块，发挥二者之长的模式。

    ```javascript
    function SuperType(name){
                this.name = name;
                this.colors = ["red", "blue", "green"];
            }
            
            SuperType.prototype.sayName = function(){
                alert(this.name);
            };
    
            function SubType(name, age){  
                SuperType.call(this, name);
                
                this.age = age;
            }
    
            SubType.prototype = new SuperType();
            
            SubType.prototype.sayAge = function(){
                alert(this.age);
            };
            
            var instance1 = new SubType("Nicholas", 29);
            instance1.colors.push("black");
            alert(instance1.colors);  //"red,blue,green,black"
            instance1.sayName();      //"Nicholas";
            instance1.sayAge();       //29
            
           
            var instance2 = new SubType("Greg", 27);
            alert(instance2.colors);  //"red,blue,green"
            instance2.sayName();      //"Greg";
            instance2.sayAge();       //27
    ```

    

- 寄生继承

  - 创建一个仅用于封装继承过程的函数，该函数以内部方式来增强对象，最后返回对象。

- 寄生组合继承





1. js原型是什么

   > `[[Prototype]]`（如规范中所命名的），它要么为 `null`，要么就是对另一个对象的引用
   >
   > `object` 中读取一个缺失的属性时，JavaScript 会自动从原型中获取该属性。在编程中，这种行为被称为“原型继承”。

2. Js存在类吗？本质是什么？ 

   > 存在  本质是object

3. js为什么要设置原型 

   > 让所有对象实例共享原型的属性和方法。

4. 继承这种概念解决什么问题 

5. 原型继承挂在的方法，属性是引用还是拷贝关系  

6. 原型链

7. 原型链能够实现所谓的继承的本质原因是什么

   > 原型链利用原型让一个引用类型继承另一个引用类型的属性和方法。

8. 原型链的实现：

   ```javascript
   function SuperType(){
     this.prototype = true;
   }
   SuperType.prototype.getSuperValue = function(){
     return this.property;
   }
   function SubType(){
     this.subproperty = false;
   }
   SubType.prototype = new SuperType()
   SubType.prototype.getSuperValue = function(){
     return this.subproperty;
   }
   var instance = new SubType()
   
   ```

   ```javascript
   let animal = {
     eats: true,
     walk() {
       alert("Animal walk");
     }
   };
   
   let rabbit = {
     jumps: true,
     __proto__: animal
   };
   
   // walk 方法是从原型中获得的
   rabbit.walk(); // Animal walk
   ```

   

9. 继承的实现

   ```javascript
   function Shape() {}
   
   function Rect() {}
   
   // 方法1
   Rect.prototype = new Shape();
   
   // 方法2
   Rect.prototype = Shape.prototype;
   
   // 方法3
   Rect.prototype = Object.create(Shape.prototype);
   
   Rect.prototype.area = function () {
     // do something
   };
   ```



#### 深拷贝

 浅拷贝是将原始对象中的数据型字段拷贝到新对象中去，将引用型字段的“引用”复制到新对象中去，不把“引用的对象”复制进去，所以原始对象和新对象引用同一对象，新对象中的引用型字段发生变化会导致原始对象中的对应字段也发生变化。
    深拷贝是在引用方面不同，深拷贝就是创建一个新的和原始字段的内容相同的字段，是两个一样大的数据段，所以两者的引用是不同的，之后的新对象中的引用型字段发生改变，不会引起原始对象中的字段发生改变。



深拷贝、自定义深拷贝 

浅拷贝：

```javascript
function copy(obj){
  var objCopy = {};
  for (let key in obj){
    objCopy[key] = obj[key];
  }
  return objCopy;
}
var person  = {name:"yuki",age:20,car:{brand:"Ferrari",type:"430"}};
var personCopy = copy(person);
//person和personCopy共用一个car对象————浅拷贝
```

深拷贝：

1. 用JSON

   ```javascript
   function jsonClone(obj) {
       return JSON.parse(JSON.stringify(obj));
   }
   var clone = jsonClone({ a:1 });
   ```

   

2. for循环

   ```javascript
   function deepClone(obj){
     let result  = typeof obj.splice === "function" ? []:{};
     if(obj && typeof obj =='object'){
       for(let key in obj){
         if (obj[key] && typeof obj[key] === 'object' ){
           result[key] = deepClone(obj[key]);
         }else{
           result[key] = obj[key];
         }
       }
       return result;
     }
     return obj;
   }
   ```

   

3. Array.prototype.forEach 

   ```javascript
   let deepClone = function(obj){
     let copy = Object.create(Object.getPrototypeOf(obj));
     let propNames = Object.getOwnPropertyNames(obj);
     propNames.forEach(function(items){
       letitem = Object.getOwnPropertyDescriptor(obj,items);
       Object.defineProperty(copy,items,item);
     });
     return copy;
   }
   ```

   - [Object.create(proto, [descriptors\])](https://developer.mozilla.org/zh/docs/Web/JavaScript/Reference/Global_Objects/Object/create) —— 利用给定的 `proto` 作为 `[[Prototype]]` 和可选的属性描述来创建一个空对象。
   - [Object.getPrototypeOf(obj)](https://developer.mozilla.org/zh/docs/Web/JavaScript/Reference/Global_Objects/Object/getPrototypeOf) —— 返回对象 `obj` 的 `[[Prototype]]`。
   - [Object.setPrototypeOf(obj, proto)](https://developer.mozilla.org/zh/docs/Web/JavaScript/Reference/Global_Objects/Object/setPrototypeOf) —— 将对象 `obj` 的 `[[Prototype]]` 设置为 `proto`。
   - **`Object.getOwnPropertyNames()`**方法返回一个由指定对象的所有自身属性的属性名（包括不可枚举属性但不包括Symbol值作为名称的属性）组成的数组。
   - **`Object.getOwnPropertyDescriptor()`** 方法返回指定对象上一个自有属性对应的属性描述符。（自有属性指的是直接赋予该对象的属性，不需要从原型链上进行查找的属性）
   - `Object.defineProperty()` 方法会直接在一个对象上定义一个新属性，或者修改一个对象的现有属性，并返回此对象

```javascript
function deepClone(obj) {
    var _toString = Object.prototype.toString;

    // null, undefined, non-object, function
    if (!obj || typeof obj !== 'object') {
        return obj;
    }

    // DOM Node
    if (obj.nodeType && 'cloneNode' in obj) {
        return obj.cloneNode(true);
    }

    // Date
    if (_toString.call(obj) === '[object Date]') {
        return new Date(obj.getTime());
    }

    // RegExp
    if (_toString.call(obj) === '[object RegExp]') {
        var flags = [];
        if (obj.global) { flags.push('g'); }
        if (obj.multiline) { flags.push('m'); }
        if (obj.ignoreCase) { flags.push('i'); }

        return new RegExp(obj.source, flags.join(''));
    }

    var result = Array.isArray(obj) ? [] :
        obj.constructor ? new obj.constructor() : {};

    for (var key in obj ) {
        result[key] = deepClone(obj[key]);
    }

    return result;
}

function A() {
    this.a = a;
}

var a = {
    name: 'qiu',
    birth: new Date(),
    pattern: /qiu/gim,
    container: document.body,
    hobbys: ['book', new Date(), /aaa/gim, 111]
};

var c = new A();
var b = deepClone(c);
console.log(c.a === b.a);
console.log(c, b);
```



#### 防抖和节流



### BOM

#### window对象

在全局变量中声明的变量、函数都会变成window的属性和方法。

- 窗口位置：screenLeft和screenTop  表示窗口相对于屏幕左边和上边的位置
- 窗口大小：innerWidth，innerHeight——浏览器页面视图的大小，outerWidth，outerHeight——浏览器窗口本身的尺寸。
- 打开窗口：window.open()  

#### screen对象



#### location对象

- `Location.href`：整个 URL。
- `Location.protocol`：当前 URL 的协议，包括冒号（`:`）。
- `Location.host`：主机。如果端口不是协议默认的`80`和`433`，则还会包括冒号（`:`）和端口。
- `Location.hostname`：主机名，不包括端口。
- `Location.port`：端口号。
- `Location.pathname`：URL 的路径部分，从根路径`/`开始。
- `Location.search`：查询字符串部分，从问号`?`开始。
- `Location.hash`：片段字符串部分，从`#`开始。
- `Location.username`：域名前面的用户名。
- `Location.password`：域名前面的密码。
- `Location.origin`：URL 的协议、主机名和端口。

#### navigator对象



#### history对象

#### 弹框

#### 计时

#### Cookie

### DOM

#### 节点层次、类型、属性

#### DOM操作

- CRUD
- 动态脚本
- 动态样式
- ...

#### 事件！（红宝书）

##### 事件流

##### 事件对象

##### 冒泡/捕获

冒泡（bubbling）原理很简单。

**当一个事件发生在一个元素上，它会首先运行在该元素上的处理程序，然后运行其父元素上的处理程序，然后一直向上到其他祖先上的处理程序。**

停止冒泡的方法是 `event.stopPropagation()`。



事件处理的另一个阶段被称为“捕获（capturing）”。它很少被用在实际开发中，但有时是有用的。

[DOM 事件](http://www.w3.org/TR/DOM-Level-3-Events/)标准描述了事件传播的 3 个阶段：

1. 捕获阶段（Capturing phase）—— 事件（从 Window）向下走近元素。
2. 目标阶段（Target phase）—— 事件到达目标元素。
3. 冒泡阶段（Bubbling phase）—— 事件从元素上开始冒泡。

##### 事件委托

符合 W3C 标准的事件绑定 addEventLisntener /attachEvent 

让利用事件冒泡的原理，让自己的所触发的事件，让他的父元素代替执行

##### 各种事件具体类型

- UI
- 鼠标/滚轮
- 键盘/文本
- ......



1. 事件委托怎么实现

   > 事件委托：
   >
   > 如果我们有许多以类似方式处理的元素，那么就不必为每个元素分配一个处理程序 —— 而是将单个处理程序放在它们的共同祖先上。
   >
   > 在处理程序中，我们获取 `event.target` 以查看事件实际发生的位置并进行处理。
   >
   > 算法：
   >
   > 1. 在容器（container）上放一个处理程序。
   > 2. 在处理程序中 —— 检查源元素 `event.target`。
   > 3. 如果事件发生在我们感兴趣的元素内，那么处理该事件。

2. event是什么

   > **`Event`** 接口表示在 DOM 中出现的事件。

3. 什么是异步加载

   > 异步加载又叫非阻塞加载，浏览器在下载执行js的同时，还会继续进行后续页面的处理。

4. 浏览器的事件循环机制

   > **事件循环** 的概念非常简单。它是一个在 JavaScript 引擎**等待任务，执行任务和进入休眠状态等待更多任务**这几个状态之间转换的无限循环。
   >
   > 一个任务到来时，引擎可能正处于繁忙状态，那么这个任务就会被排入队列。
   >
   > 多个任务组成了一个队列，即所谓的“宏任务队列”
   >
   > 微任务仅来自于我们的代码。它们通常是由 promise 创建的：对 `.then/catch/finally` 处理程序的执行会成为微任务。微任务也被用于 `await` 的“幕后”，因为它是 promise 处理的另一种形式。
   >
   > 还有一个特殊的函数 `queueMicrotask(func)`，它对 `func` 进行排队，以在微任务队列中执行。
   >
   > **每个宏任务之后，引擎会立即执行微任务队列中的所有任务，然后再执行其他的宏任务，或渲染，或进行其他任何操作。**

5. 宏任务和微任务都有哪些

   > ## 宏任务：
   >
   > | #                     | 浏览器 | Node |
   > | --------------------- | :----: | ---: |
   > | I/O                   |   ✅    |    ✅ |
   > | setTimeout            |   ✅    |    ✅ |
   > | setInterval           |   ✅    |    ✅ |
   > | setImmediate          |   ❌    |    ✅ |
   > | requestAnimationFrame |   ✅    |    ❌ |
   >
   > ## 微任务：
   >
   > | #                          | 浏览器 | Node |
   > | -------------------------- | :----: | ---: |
   > | process.nextTick           |   ❌    |    ✅ |
   > | MutationObserver           |   ✅    |    ❌ |
   > | Promise.then catch finally |   ✅    |    ✅ |

6. DOM回调是什么

   > https://developer.mozilla.org/zh-CN/docs/Web/Guide/Events/Event_handlers
   >
   > 广义 [`addEventListener()`](https://developer.mozilla.org/zh-CN/docs/Web/API/EventTarget/addEventListener) 和一组特定的***on-event***处理器。

7. **一次 js 请求一般情况下有哪些地方会有缓存处理？**

   > dns 缓存，cdn 缓存，浏览器缓存，服务器缓存

8. 

### 网络请求

#### AJAX 

#### Fetch

### event loop

?

### 运行机制



#### 事件循环：微任务和宏任务

[事件循环：微任务和宏任务](https://zh.javascript.info/event-loop)

**事件循环** 的概念非常简单。它是一个在 JavaScript 引擎等待任务，执行任务和进入休眠状态等待更多任务这几个状态之间转换的无限循环。

微任务仅来自于我们的代码。它们通常是由 promise 创建的：对 `.then/catch/finally` 处理程序的执行会成为微任务。微任务也被用于 `await` 的“幕后”，因为它是 promise 处理的另一种形式。

还有一个特殊的函数 `queueMicrotask(func)`，它对 `func` 进行排队，以在微任务队列中执行。

**每个宏任务之后，引擎会立即执行微任务队列中的所有任务，然后再执行其他的宏任务，或渲染，或进行其他任何操作。**

### ES6+（6,7,8......）

[阮一峰的ES6教程](https://www.bookstack.cn/read/es6-3rd/sidebar.md)

#### 块级绑定

#### 各种扩展

- 字符串
- 数值
- 函数
- 数组
- 对象
- 正则

#### 解构

#### Symbol

#### Class

#### Set/Map



1. map和set的区别

   > 都可以储存不重复的值集合set 是以 [value, value]的形式储存元素，字典map 是以 [key, value] 的形式储存

#### Promise、async /await等异步编程

##### 回调

##### promise

三种状态：pending、fulfilled、rejected(未决定，履行，拒绝)

1.初始化，状态：pending

2.当调用resolve(成功)，状态：pengding=>fulfilled

3.当调用reject(失败)，状态：pending=>rejected





- 优点：解决了回调地狱的问题 

  缺点：无法取消 Promise ，错误需要通过回调函数来捕获

- promise链的顺序模式（this-then-this-then-that流程控制）

- promise.all([...])

  - 需要一个参数，是一个数组，通常由promise实例组成，从promise.all([])调用返回的promise会得到一个完成消息，这是由一个所传入promise的完成消息组成的数组，与指定的顺序一致，与完成顺序无关。

  - Promise.all 方法接受一个数组作为参数，p1、p2、p3 都是 Promise 实例，如果 不是，就会先调用下面讲到的 Promise.resolve 方法，将参数转为 Promise 实例， 再进一步处理。（Promise.all 方法的参数可以不是数组，但必须具有 Iterator 接 口，且返回的每个成员都是 Promise 实例。）

  - 手写实现promise.all()

    ```javascript
    const promise1 = Promise.resolve(3)
    const promise2 = 42;
    const promise3 = new Promise((resolve,reject)=> {
      setTimeout(resolve,100,'foo');
    })
    
    Promise.all([promise1,promise2,promise3]).then((values)=>{
      console.values;
    });
    ```

    ```javascript
    // 手写Promise.all()
    Promise.property.all = function (iterators) {
      const promises = Array.from(iterators);
      const len = promises.length;
      let count = 0;
      let resultList = [];
      return new Promise((resolve,reject)=>{
          promises.forEach((p,index) =>{
              Promise.resolve(p)
          .then((result)=>{
              count++;
              resultList[index] = result;
              if(count === len){
                  resolve(resultList);
              }
      })
      .catch(e=>{
          reject(e);
      })
      })
      })
    }
    ```

    

  - 

  - 

- promise.race([...])

  - 只响应第一个跨过终点线的promise，抛弃其他的promise

  - 实现

    ```javascript
    Promise._race = promises => new Promise((resolve, reject) => 
    { promises.forEach(promise => { promise.then(resolve, reject) })})
    Promise.myrace = function(iterator) { return new Promise ((resolve,reject) => 
        { try {let it = iterator[Symbol.iterator](); while(true) 
            { let res = it.next(); console.log(res); 
                if(res.done) break; 
                if(res.value instanceof Promise){ 
                    res.value.then(resolve,reject); 
                } else{ 
                    resolve(res.value) 
                } 
            } 
        } catch (error) 
        { 
            reject(error) 
        }
    ```

    

- promise.finally([...])

  - .

  - 实现

    ```javascript
    Promise.prototype.finally = function(callback){
        let P = this.constructor;
        return this.then(
            value => P.resolve(callback()).then(()=> value),
            reason => P.resolve(callback()).then(()=>{ throw reason})
        )
    ```

    

- promise的应用场景

- Promise.all与Promise.race有什么区别 

  > Promise.all可以将多个实例组装成一个新的实例，成功的时候返回一个成功数组，失败的时候则返回最先被reject失败状态的值
  >
  > Promise.race([p1, p2, p3])里面的结果哪个获取的快，就返回哪个结果，不管结果本身是成功还是失败

- Object.defineProperty 的缺陷 .没有Proxy，怎么解决上述缺陷

  > 1、无法监听到数组的长度变化 2、由于只能劫持对象的属性，对于复杂对象需要对每个属性进行深度遍历 3、由于只能劫持对象的属性，对象属性有新增时，需要将对象的所有属性都进行遍历进行监听

##### 生成器

##### 程序性能

#### Iterator / Generater

#### Proxy / Reflect

#### Module模块

## 版本控制系统

## web安全

## 包处理器

### npm

### yarn

## CSS 架构



## CSS 预处理器

### Sass

### Lass



## 建设工具

###  npm scripts

### webpack

### ESLint



## 框架

### Vue.js

### React.js

### Angular



## 现代CSS



## web组件



## CSS框架

### bootstrap

。。。



## 测试工具



## TypeScript



## WebAPP



## 移动设备

### React Native

https://reactnative.cn/docs/getting-started





------



## Git

- 初始化一个Git仓库，使用git init命令。

- 添加文件到Git仓库，分两步：

- 1. 使用命令git add <file>，注意，可反复多次使用，添加多个文件；
  2. 使用命令git commit -m      <message>，完成。

-  

- 要随时掌握工作区的状态，使用git status命令。

- 如果git status告诉你有文件被修改过，用git diff可以查看修改内容。

-  

- HEAD指向的版本就是当前版本，因此，Git允许我们在版本的历史之间穿梭，使用命令git reset --hard commit_id。

- 穿梭前，用git log可以查看提交历史，以便确定要回退到哪个版本。

- 要重返未来，用git reflog查看命令历史，以便确定要回到未来的哪个版本。

-  

- 暂存区是Git非常重要的概念，弄明白了暂存区，就弄明白了Git的很多操作到底干了什么。

-  

- 又到了小结时间。

- 场景1：当你改乱了工作区某个文件的内容，想直接丢弃工作区的修改时，用命令git checkout -- file。

- 场景2：当你不但改乱了工作区某个文件的内容，还添加到了暂存区时，想丢弃修改，分两步，第一步用命令git reset HEAD <file>，就回到了场景1，第二步按场景1操作。

- 场景3：已经提交了不合适的修改到版本库时，想要撤销本次提交，参考[版本回退](https://www.liaoxuefeng.com/wiki/896043488029600/897013573512192)一节，不过前提是没有推送到远程库。

- 命令git rm用于删除一个文件。如果一个文件已经被提交到版本库，那么你永远不用担心误删，但是要小心，你只能恢复文件到最新版本，你会丢失**最近一次提交后你修改的内容**。

-  

- 关联：

- 要关联一个远程库，使用命令`git remote add origin git@server-name:path/repo-name.git`；

- 关联一个远程库时必须给远程库指定一个名字，origin是默认习惯命名；

- 关联后，使用命令git push -u origin master第一次推送master分支的所有内容；

- 此后，每次本地提交后，只要有必要，就可以使用命令git push origin master推送最新修改；

-  

- git clone命令克隆。

- Git支持多种协议，包括https，但ssh协议速度最快。

- Git鼓励大量使用分支：

- 查看分支：git branch

- 创建分支：git branch <name>

- 切换分支：git checkout <name>或者git switch <name>

- 创建+切换分支：git checkout -b <name>或者git switch -c <name>

- 合并某分支到当前分支：git merge <name>

- 删除分支：git branch -d <name>

-  

- 当Git无法自动合并分支时，就必须首先解决冲突。解决冲突后，再提交，合并完成。

- 解决冲突就是把Git合并失败的文件手动编辑为我们希望的内容，再提交。

- 用git log --graph命令可以看到分支合并图。

-  

- 合并分支时，加上--no-ff参数就可以用普通模式合并，合并后的历史有分支，能看出来曾经做过合并，而fast forward合并就看不出来曾经做过合并。

- 修复bug时，我们会通过创建新的bug分支进行修复，然后合并，最后删除；

- 当手头工作没有完成时，先把工作现场git stash一下，然后去修复bug，修复后，再git stash pop，回到工作现场；

- 在master分支上修复的bug，想要合并到当前dev分支，可以用git cherry-pick <commit>命令，把bug提交的修改“复制”到当前分支，避免重复劳动。

-  

- 如果要丢弃一个没有被合并过的分支，可以通过git branch -D <name>强行删除。

-  

- 查看远程库信息，使用git remote -v；

- 本地新建的分支如果不推送到远程，对其他人就是不可见的；

- 从本地推送分支，使用git push origin branch-name，如果推送失败，先用git pull抓取远程的新提交；

- 在本地创建和远程分支对应的分支，使用git checkout -b branch-name origin/branch-name，本地和远程分支的名称最好一致；

- 建立本地分支和远程分支的关联，使用git branch --set-upstream branch-name origin/branch-name；

- 从远程抓取分支，使用git pull，如果有冲突，要先处理冲突。

-  

- rebase操作可以把本地未push的分叉提交历史整理成直线；

- rebase的目的是使得我们在查看历史提交的变化时更容易，因为分叉的提交需要三方对比。

-  

- 命令git tag <tagname>用于新建一个标签，默认为HEAD，也可以指定一个commit id；

- 命令git tag -a <tagname> -m "blablabla..."可以指定标签信息；

- 命令git tag可以查看所有标签。

- 命令git push origin <tagname>可以推送一个本地标签；

- 命令git push origin --tags可以推送全部未推送过的本地标签；

- 命令git tag -d <tagname>可以删除一个本地标签；

- 命令git push origin :refs/tags/<tagname>可以删除一个远程标签。

-  

- 忽略某些文件时，需要编写.gitignore；

- .gitignore文件本身要放到版本库里，并且可以对.gitignore做版本管理！

-  

- 来自 <https://www.liaoxuefeng.com/wiki/896043488029600/900004590234208> 

-  

## Basic Terminal Usage





## 数据结构与算法

### 数据结构

### 排序算法

### 查找算法

#### 二分查找

```javascript
let search = (arr, target) => {
    let begin = 0;
    let end = arr.length-1; 
    while(begin <= end) {
        Math.floor((begin+end)/2
        if(arr[mid] == target) {
            return mid;
        }
        else if(arr[mid] > target) {
            end = mid - 1;
        }
        else if(arr[mid] < target) {
            begin = mid + 1; 
        }
    }
    return -1;
}

```



## GitHub



## Licenses



## SSH 



## Semantic Versioning





## 设计模式







## 参考

- https://github.com/kamranahmedse/developer-roadmap

![frontend roadmap](D:\download\frontend roadmap.png)