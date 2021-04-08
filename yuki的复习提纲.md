## intro

[TOC]



## HTML

### SEO

SEO是指在了解搜索引擎自然排名机制的基础之上，对网站进行内部及外部的调整优化，改进网站在搜索引擎中关键词的自然排名，获得更多的展现量，吸引更多目标客户点击访问网站，从而达到互联网营销及品牌建设的目标。

搜索引擎通过爬虫技术获取的页面就是由一堆 html 标签组成的代码，人可以通过可视化的方式来判断页面上哪些内容是重点，而机器做不到。 但搜索引擎会根据标签的含义来判断内容的权重，因此，在合适的位置使用恰当的标签，使整个页面的语义明确，结构清晰，搜索引擎才能正确识别页面中的重要内容，并予以较高的权值。比如h1~h6这几个标签在SEO中的权值非常高，用它们作页面的标题就是一个简单的SEO优化。

1. img标签的title和alt

   > title：鼠标覆盖上去显示的文字
   >
   > alt:图片加载不出来的时候的占位字

2. meta标签

   > https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/meta
   >
   > 
   >
   > 元数据（Metadata）是数据的数据信息。
   >
   > <meta> 标签提供了 HTML 文档的元数据。元数据不会显示在客户端，但是会被浏览器解析。
   >
   > META元素通常用于指定网页的描述，关键词，文件的最后修改时间，作者及其他元数据。
   >
   > 元数据可以被使用浏览器（如何显示内容或重新加载页面），搜索引擎（关键词），或其他 Web 服务调用。

3. DOCTYPE标签

   > <!DOCTYPE> 声明位于文档中的最前面的位置，处于 <html> 标签之前。
   >
   > <!DOCTYPE> 声明不是一个 HTML 标签；它是用来**告知 Web 浏览器页面使用了哪种 HTML 版本。**
   >
   > 在 HTML 4.01 中，<!DOCTYPE> 声明需引用 DTD （文档类型声明），因为 HTML 4.01 是基于 SGML （Standard Generalized Markup Language 标准通用标记语言）。DTD 指定了标记语言的规则，确保了浏览器能够正确的渲染内容。
   >
   > HTML5 不是基于 SGML，因此不要求引用 DTD。
   >
   > **提示：**总是给您的 HTML 文档添加 <!DOCTYPE> 声明，确保浏览器能够预先知道文档类型。

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

5. BFC

   > 块级格式化上下文
   >
   > （W3C CSS 2.1 规范中的一个概念,它是一个独立容器，**决定了元素如何对其内容进行定位,以及与其他元素的关系和相互作用**。）
   >  一个页面是由很多个 Box 组成的,元素的类型和 display 属性,决定了这个 Box 的类型。
   >  不同类型的 Box,会参与不同的 Formatting Context（决定如何渲染文档的容器）,因此Box内的元素会以不同的方式渲染,也就是说BFC内部的**元素和外部的元素不会互相影响。**

6. 懒加载和预加载

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

7. 减少DOM操作是什么

8. 渐进增强与优雅降级

9. img 的 alt 与 title 有何异同？ strong 与 em 的异同？ 

   a:alt(alt text):为不能显示图像、窗体或 applets 的用户代理（UA），alt 属性用来指 定替换文字。替换文字的语言由 lang 属性指定。(在 IE 浏览器下会在没有 title 时把 alt 当成 tool tip 显示) title(tool tip):该属性为设置该属性的元素提供建议性的信息。 strong:粗体强调标签，强调，表示内容的重要性 em:斜体强调标签，更强烈强调，表示内容的强调点

10. 行内元素和块级元素

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

11. **浏览器标准模式和怪异模式之间的区别是什么？** 

    标准模式是指，浏览器按 W3C 标准解析执行代码； 

    怪异模式则是使用浏览器自己的方式解析执行代码，因为不同浏览器解析执行的方式不一 

    样，所以我们称之为怪异模式。浏览器解析时到底使用标准模式还是怪异模式，与你网页中的 DTD 声明直接相关，DTD 声 

    明定义了标准文档的类型（标准模式解析）文档类型，会使浏览器使用相应的方式加载网页 

    并显示，忽略 DTD 声明,将使网页进入怪异模式

12. 

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
   >

2. 

### 响应式设计

@media 规则允许在相同样式表为不同媒体设置不同的样式。



### 经典面试题

display有哪些，display none和visibility:hidden区别 

none，block，hidden......

| none               | 此元素不会被显示。                                           |
| ------------------ | ------------------------------------------------------------ |
| block              | 此元素将显示为块级元素，此元素前后会带有换行符。             |
| inline             | 默认。此元素会被显示为内联元素，元素前后没有换行符。         |
| inline-block       | 行内块元素。（CSS2.1 新增的值）                              |
| list-item          | 此元素会作为列表显示。                                       |
| run-in             | 此元素会根据上下文作为块级元素或内联元素显示。               |
| compact            | CSS 中有值 compact，不过由于缺乏广泛支持，已经从 CSS2.1 中删除。 |
| marker             | CSS 中有值 marker，不过由于缺乏广泛支持，已经从 CSS2.1 中删除。 |
| table              | 此元素会作为块级表格来显示（类似 <table>），表格前后带有换行符。 |
| inline-table       | 此元素会作为内联表格来显示（类似 <table>），表格前后没有换行符。 |
| table-row-group    | 此元素会作为一个或多个行的分组来显示（类似 <tbody>）。       |
| table-header-group | 此元素会作为一个或多个行的分组来显示（类似 <thead>）。       |
| table-footer-group | 此元素会作为一个或多个行的分组来显示（类似 <tfoot>）。       |
| table-row          | 此元素会作为一个表格行显示（类似 <tr>）。                    |
| table-column-group | 此元素会作为一个或多个列的分组来显示（类似 <colgroup>）。    |
| table-column       | 此元素会作为一个单元格列显示（类似 <col>）                   |
| table-cell         | 此元素会作为一个表格单元格显示（类似 <td> 和 <th>）          |
| table-caption      | 此元素会作为一个表格标题显示（类似 <caption>）               |
| inherit            | 规定应该从父元素继承 display 属性的值。                      |

display none和visibility:hidden区别 :

display none   元素不会渲染在文档流中，不占用空间

visibility:hidden：不显示元素，但是能在文档流中找到。依然占用空间。





#### 垂直水平居中

##### 水平居中



##### 垂直居中

1. line-height

   ```CSS 
   .center {
       line-height: 200px;
       height: 200px;
       border: 3px solid green;
       text-align: center;
   }
    
   /* 如果文本有多行，添加以下代码: */
   .center p {
       line-height: 1.5;
       display: inline-block;
       vertical-align: middle;
   }
   
   ```

2. `padding:x,0`



##### 垂直水平居中

https://blog.csdn.net/weixin_37580235/article/details/82317240

1. positioning 和 transform 属性

   ```css
   .center { 
       height: 200px;
       position: relative;
       border: 3px solid green; 
   }
   
   .center .word {
       margin: 0;
       position: absolute;
       top: 50%;
       left: 50%;
       -ms-transform: translate(-50%, -50%);
       transform: translate(-50%, -50%);
   }
   ```

2. 设置父元素为相对定位，给子元素设置绝对定位，**top: 0; right: 0; bottom: 0; left: 0; margin: auto;**

   ```css
   <style>
       #father {
           width: 500px;
           height: 300px;
           background-color: skyblue;
           position: relative;
   }
    
       #son {
           width: 100px;
           height: 100px;
           background-color: green;
           position: absolute;
           top: 0;
           right: 0;
           bottom: 0;
           left: 0;
           margin: auto;
   }
   </style>
    
   <div id="father">
       <div id="son">我是块级元素</div>
   </div>
   ```

   

3. 。

   ```css
   <div class="parent"> <div class="child"></div></div> 一、div.parent { display: flex; justify-content: center; align-items: center; } 二、div.parent { position: relative;
   }div.child { position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%); }/* 或者 */div.child { width: 50px; height: 10px; position: absolute; top: 50%; left: 50%; margin-left: -25px; margin-top: -5px;}/* 或 */div.child { width: 50px; height: 10px; position: absolute; left: 0; top: 0; right: 0; bottom: 0; margin: auto; } 三、div.parent { display: grid; }div.child { justify-self: center; align-self: center; } 四、div.parent { font-size: 0; text-align: center; &::before { content: ""; display: inline-block; width: 0; height: 100%; vertical-align: middle; }}div.child{ display: inline-block; vertical-align: middle;
   }
   ```

   

4. 



#### 三栏布局

##### flex实现 

- 左边宽度固定，中间与右边宽度相等



- 两边固定宽中间自适应的布局

```html
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title>layout_box</title>
    <style>
      html,body{ margin: 0px;width: 100%; }
h3{height: 100px;margin:20px 0 0;}
#left,#right{width: 200px;height: 200px; background-color: #ffe6b8;position: absolute;}
#left{left:0px;}
#right{right: 0px;}
#center{margin:2px 210px ;background-color: #eee;height: 200px; }
    </style>
	</head>
	<body>
		<div id = "left">我是左边</div>
		<div id = "right">我是右边</div>
		<div id = "center">我是中间</div>
	</body>
</html>
```

自身浮动

```css
#left_self,#right_self{ width: 200px;height: 200px; background-color: #ffe6b8 }
#left_self {float: left;}
#right_self{float: right;}
#center_self{margin: 0 210px;height: 200px; background-color: #a0b3d6}
```



#### 两栏布局

#### 栅格布局

```css
> 栅格布局

​```css
.col-1,
.col-2,
.col-3,
.col-4,
.col-5,
.col-6,
.col-7,
.col-8,
.col-9,
.col-10 {
    position: relative;
    min-height: 1px;
    float: left;
}

.col-1 {
    width: 10%;
}

.col-2 {
    width: 20%;
}

.col-3 {
    width: 30%;
}

.col-4 {
    width: 40%;
}

.col-5 {
    width: 50%;
}

.col-6 {
    width: 60%;
}

.col-7 {
    width: 70%;
}

.col-8 {
    width: 80%;
}
​```


```



#### 圣杯布局

 https://zhuanlan.zhihu.com/p/58355168

1. float实现

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta http-equiv="X-UA-Compatible" content="IE=edge">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Document</title>
       <style>
           *{
               margin: 0;
               padding: 0;
           }
           .header,.footer{
               height:100px ;
               width:100%;
               background-color: palegreen;
           }
           .footer{
               clear: both;
           }
           .container{
               padding-left: 20%;
               padding-right: 25%;
           }
           .container div{
               position: relative;
               float:left;
           }
           .middle{
               width:100%;
               background-color:peachpuff;
           }
           .left{
               width:20%;
               background-color:brown;
               margin-left: -100%;
               left: -20%;
   
           }
           .right{
               width:25%;
               background-color:brown;
               margin-left: -25%;
               left: 25%;
           }
       </style>
   </head>
   <body>
       <div class="header">header</div>
       <div class="container">
           <div class="middle">middle</div>
           <div class="left">left</div>
           <div class="right">right</div>
       </div>
       <div class="footer">footer</div>
   </body>
   </html>
   ```

   

2. flex实现

   > https://developer.mozilla.org/zh-CN/docs/Web/CSS/flex
   >
   > 1)最外层定义flex，并规定主轴方向是竖直
   >
   > 2）中间层再次设定flex
   >
   > 3）左边和右边设置宽度，中间设定flex = 1

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta http-equiv="X-UA-Compatible" content="ie=edge">
   <title>Document</title>
   <style>
     body,html{
         height: 100%;
     }
   #parent{
       height:100%;
       background-color:#36e;
       display: flex;
       justify-content: space-between;
        flex-direction: column;
      }
      div.head{
          height: 100px;
          background-color: #111555;
      }
    div.main{
         flex:1;
         background-color: #0f0;
         display: flex;
    }
    div.child3{
        height: 100px;
        background-color: red;
    }
    div.left{
        width: 100px;
        background-color: #f3f;
    }
    div.middle{
        flex:1;
        background-color:lightgreen;
    }
    div.right{
        width: 100px;
        background-color: black;
    }
   </style>
   </head>
   <body>
   <div id="parent">
         <div class="head">11</div>
         <div class="main">
             <div class="left"></div>
             <div class="middle"></div>
             <div class="right"></div>
         </div>
         <div class="footer">11</div>
   </div>
   </body>
   </html>
   
   ```

   ### 

3. .

   <!DOCTYPE html>
   <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Document</title>
     <style>
       .header { 
         height:3rem;
         background-color: aquamarine;
       }
       .footer { 
         height:3rem;
         background-color:antiquewhite;
       }
       .center { 
         width: 100%;
         height:30rem;
         background-color:palegoldenrod
       }
       .left { 
         width: 200px;
         height:30rem;
         background-color:lightcoral;
         margin-left: -100%;
       }
       .right { 
         width: 200px;
         height:30rem;
         background-color:lightcoral;
         margin-left: -200px;
       }
       .center {
         float: left;
       }
       .left {
             float: left;
       }
       .right {
             float: left;
       }
       .clearfix::after {
         content: "";
         display: block;
         clear: both;
       }
     </style>
   </head>
   <body>
     <div class="header">header </div>
     <div class="main  clearfix">
       <div class="center">center </div>
       <div class="left">left</div>
       <div class="right">right</div>
     </div>
     <div class="footer">footer</div>
   </body>
   </html>

4. 

#### 重排和重绘

Repaint——屏幕的一部分要重画，比如某个CSS的背景色变了。但是元素的几何尺寸没有变。
Reflow——意味着元件的几何尺寸变了，我们需要重新验证并计算Render Tree。是Render Tree的一部分或全部发生了变化。这就是Reflow，或是Layout。（HTML使用的是flow based layout，也就是流式布局，所以，如果某元件的几何尺寸发生了变化，需要重新布局，也就叫reflow）reflow 会从<html>这个root frame开始递归往下，依次计算所有的结点几何尺寸和位置，在reflow过程中，可能会增加一些frame，比如一个文本字符串必需被包装起来。

当你增加、删除、修改DOM结点时，会导致Reflow或Repaint
当你移动DOM的位置，或是搞个动画的时候。
当你修改CSS样式的时候。
当你Resize窗口的时候（移动端没有这个问题），或是滚动的时候。
当你修改网页的默认字体时。
注：display:none会触发reflow，而visibility:hidden只会触发repaint，因为没有发现位置变化。


#### CSS Sprites

### 更改光标

```html
<span style="cursor:auto">auto</span><br>
<span style="cursor:crosshair">crosshair</span><br>
<span style="cursor:default">default</span><br>
<span style="cursor:e-resize">e-resize</span><br>
<span style="cursor:help">help</span><br>
<span style="cursor:move">move</span><br>
<span style="cursor:n-resize">n-resize</span><br>
<span style="cursor:ne-resize">ne-resize</span><br>
<span style="cursor:nw-resize">nw-resize</span><br>
<span style="cursor:pointer">pointer</span><br>
<span style="cursor:progress">progress</span><br>
<span style="cursor:s-resize">s-resize</span><br>
<span style="cursor:se-resize">se-resize</span><br>
<span style="cursor:sw-resize">sw-resize</span><br>
<span style="cursor:text">text</span><br>
<span style="cursor:w-resize">w-resize</span><br>
<span style="cursor:wait">wait</span><br>
```

- 像素最小是1px，如果想要画0.5px的直线该如何实现（通过缩放，CSS 中 transform 的 scale 为 0.5 即可实现）

  ```css
  <style>
  .hr.scale-half {
      height: 1px;
      transform: scaleY(0.5);
  }
  </style>
      <p>1px + scaleY(0.5)</p>
      <div class="hr scale-half"></div>
  ```

  box-shadow

  ```css
  <style>
  .hr.boxshadow {
      height: 1px;
      background: none;
      box-shadow: 0 0.5px 0 #000;
  }
  </style>
  <p>box-shadow: 0 0.5px 0 #000</p>
  <div class="hr boxshadow"></div>
  
  ```

  

- 实现一个三角形

  ```css
  .caret {
    width: 0;
    height: 0;
    border: 50px solid transparent;
    border-top-color: black;
  }
  ```

- 幻灯片

- 

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
  >   let len = this.length;
  >   let l = start === undefined ? 0 : start < 0 ? Math.max(start + len, 0) : Math.min(start, len);
  >   let r = end === undefined ? len : end < 0 ? Math.max(end + len, 0) : Math.min(end, len);
  >   const res = [];
  >   while (l < r) {
  >     res.push(this[l++])
  >   }
  >   return res;
  > }
  > ```
  >

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
   >  1.没有自己的 this，无法调用 call，apply。 
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
>   let instance = Object.create(fn.prototype);
>   let result = fn.call(instance, ...args)
>   return typeof result === 'object' ? result : instance;
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

## 浏览器

内核：

https://www.cnblogs.com/fullhouse/archive/2011/12/19/2293455.html

```
Trident内核：IE,MaxThon,TT,The World,360,搜狗浏览器等。[又称MSHTML]
Gecko内核：Netscape6及以上版本，FF,MozillaSuite/SeaMonkey等
Presto内核：Opera7及以上。      [Opera内核原为：Presto，现为：Blink;]
Webkit内核：Safari,Chrome等。   [ Chrome的：Blink（WebKit的分支）]
```

[浏览器的工作原理：新式网络浏览器幕后揭秘 ](https://www.html5rocks.com/zh/tutorials/internals/howbrowserswork/#The_browsers_we_will_talk_about)





1. 事件模型：

2. 浏览器的主要功能

   > 浏览器的主要功能就是向服务器发出请求，在浏览器窗口中展示您选择的网络资源。这里所说的资源一般是指 HTML 文档，也可以是 PDF、图片或其他的类型。资源的位置由用户使用 URI（统一资源标示符）指定。

3. 在当前的事件模型中，哪些事件可以冒泡，哪些不会冒泡，为什么？不会冒泡的怎么实现事件委托（addEventListener第三个参数可以在捕获阶段添加事件监听)

4. 强缓存和协商缓存

5. 重排和重绘

   **由于节点的几何属性发生改变或者由于样式发生改变而不会影响布局的，称为 重绘，**例如 outline, visibility, color、background-color 等，重绘的代价是高昂的， 因为浏览器必须验证 DOM 树上其他节点元素的可见性。

6. 回流

   **回流是布局或者几何属性需要改变就称为回流。**回流是影响浏览器性能的关键 因素，因为其变化涉及到部分页面（或是整个页面）的布局更新。一个元素的 回流可能会导致了其所有子元素以及 DOM 中紧随其后的节点、祖先节点元素 的随后的回流。

7. 浏览器优化

   **浏览器优化** 
   
   现代浏览器大多都是通过队列机制来批量更新布局，浏览器会把修改操作放在 
   
   队列中，至少一个浏览器刷新（即 16.6ms）才会清空队列，但当你获取布局信 
   
   息的时候，队列中可能有会影响这些属性或方法返回值的操作，即使没有，浏 
   
   览器也会强制清空队列，触发回流与重绘来确保返回正确的值。 
   
   **主要包括以下属性或方法：** 
   
   1、offsetTop、offsetLeft、offsetWidth、offsetHeight 
   
   2、scrollTop、scrollLeft、scrollWidth、scrollHeight 
   
   3、clientTop、clientLeft、clientWidth、clientHeight 
   
   4、width、height 
   
   5、getComputedStyle() 
   
   6、getBoundingClientRect() 
   
   所以，我们应该避免频繁的使用上述的属性，他们都会强制渲染刷新队列。

8. 减少重绘与回流

   **减少重绘与回流** 
   
   **CSS** 
   
   1、使用 transform 替代 top 
   
   2、使用 visibility 替换 display: none ，因为前者只会引起重绘，后者会引发回流（改变了布局 
   
   3、避免使用 table 布局，可能很小的一个小改动会造成整个 table 的重新布局。 
   
   4、尽可能在 DOM 树的最末端改变 class，回流是不可避免的，但可以减少其影 响。尽可能在 DOM 树的最末端改变 class，可以限制了回流的范围，使其影响 尽可能少的节点。 
   
   5、避免设置多层内联样式，CSS 选择符从右往左匹配查找，避免节点层级过多。 
   
   **JavaScript** 
   
   1、避免频繁操作样式，最好一次性重写 style 属性，或者将样式列表定义为 class 并一次性更改 class 属性。 
   
   2、避免频繁操作 DOM，创建一个 documentFragment，在它上面应用所有 DOM 操作，最后再把它添加到文档中。 
   
   3、避免频繁读取会引发回流/重绘的属性，如果确实需要多次使用，就用一个 变量缓存起来。 
   
   4、对具有复杂动画的元素使用绝对定位，使它脱离文档流，否则会引起父元素 及后续元素频繁回流

9. 浏览器的渲染机制->18

10. 跨域 怎么解决跨域

11. 浏览器怎么加载一个HTML的 

12. 浏览器事件机制，事件冒泡、事件捕获，如何阻止事件冒泡

13. 本地浏览器存储了解吗，localStorage会与服务端通信吗，indexDB为什么无限存储 

    1. localStorage会与服务端通信吗:
    2. indexDB为什么无限存储 :

14. 浏览器事件触发有几个阶段，click有哪些属性 

    1. 浏览器事件触发阶段：事件捕获阶段，事件目标处理函数、事件冒泡
    2. **click的属性：**

15. 事件代理及其优缺点说一下

16. 浏览器的同源策略

    如果两个 URL 具有相同的协议，域和端口，则称它们是“同源”的。
    
    以下的几个 URL 都是同源的：
    
    - `http://site.com`
    - `http://site.com/`
    - `http://site.com/my/page.html`
    
    “同源（Same Origin）”策略限制了窗口（window）和 frame 之间的相互访问。
    
    “同源”策略规定：
    
    - 如果我们有对另外一个窗口（例如，一个使用 `window.open` 创建的弹窗，或者一个窗口中的 iframe）的引用，并且该窗口是同源的，那么我们就具有对该窗口的全部访问权限。
    - 否则，如果该窗口不是同源的，那么我们就无法访问该窗口中的内容：变量，文档，任何东西。唯一的例外是 `location`：我们可以修改它（进而重定向用户）。但是我们无法读取 `location`（因此，我们无法看到用户当前所处的位置，也就不会泄漏任何信息）。

17. 解决跨域

18. cors什么意思

    https://developer.mozilla.org/zh-CN/docs/Web/HTTP/CORS
    
    **跨源资源共享** ([CORS](https://developer.mozilla.org/en-US/docs/Glossary/CORS)) （或通俗地译为跨域资源共享）是一种基于[HTTP](https://developer.mozilla.org/en-US/docs/Glossary/HTTP) 头的机制，该机制通过允许服务器标示除了它自己以外的其它[origin](https://developer.mozilla.org/en-US/docs/Glossary/Origin)（域，协议和端口），这样浏览器可以访问加载这些资源。

19. 有的跨域不允许带cookie，可以通过什么设置改变一下

20. 浏览器的缓存策略

    https://www.jiqizhixin.com/articles/2020-07-24-12

21. 渲染机制

    浏览器采用流式布局模型（Flow Based Layout） 
    
    浏览器会把 HTML 解析成 DOM，把 CSS 解析成 CSSOM，DOM 和 CSSOM 合并就 
    
    产生了渲染树（Render Tree）。 
    
    有了 RenderTree，我们就知道了所有节点的样式，然后计算他们在页面上的大 
    
    小和位置，最后把节点绘制到页面上。 
    
    由于浏览器使用流式布局，对 Render Tree 的计算通常只需要遍历一次就可以完 
    
    成，但 table 及其内部元素除外，他们可能需要多次计算，通常要花 3 倍于同 
    
    等元素的时间，这也是为什么要避免使用 table 布局的原因之一。

22. 从输入URL到页面加载发生了什么

    1. DNS解析
       1. 首先，浏览器向本地 DNS 服务器发起请求，由于本地 DNS 服务器没有缓存不能直接将域名转换为 IP 地址，需要采用递归或者迭代查询的方式（图 3）依次向根域名服务器、顶级域名服务器、权威域名服务器发起查询请求，直至找到一个或一组 IP 地址，返回给浏览器
    2. TCP连接
    3. 发送HTTP请求
    4. 服务器处理请求并返回HTTP报文
    5. 浏览器解析渲染页面
    6. 连接结束
    
    
    
    参考[浏览器输入 URL 后发生了什么？](https://zhuanlan.zhihu.com/p/43369093)

23. localstroage,sessionstroage

    ```undefined
    本地离线存储 localStorage 长期存储数据，浏览器关闭后数据不丢失;
    sessionStorage 的数据在浏览器关闭后自动删除;
    ```

24. ## cookies，sessionStorage 和 localStorage 的区别？

    ```js
    cookie是网站为了标示用户身份而储存在用户本地终端（Client Side）上的数据（通常经过加密）。
    cookie数据始终在同源的http请求中携带（即使不需要），记会在浏览器和服务器间来回传递。
    sessionStorage和localStorage不会自动把数据发给服务器，仅在本地保存。
    
    存储大小：
        cookie数据大小不能超过4k。
        sessionStorage和localStorage 虽然也有存储大小的限制，但比cookie大得多，可以达到5M或更大。
    
    有期时间：
        localStorage    存储持久数据，浏览器关闭后数据不丢失除非主动删除数据；
        sessionStorage  数据在当前浏览器窗口关闭后自动删除。
        cookie          设置的cookie过期时间之前一直有效，即使窗口或浏览器关闭
    ```

25. ## cookie 和session 的区别：

    ```undefined
    1、cookie数据存放在客户的浏览器上，session数据放在服务器上。
    2、cookie不是很安全，别人可以分析存放在本地的COOKIE并进行COOKIE欺骗
    考虑到安全应当使用session。
    3、session会在一定时间内保存在服务器上。当访问增多，会比较占用你服务器的性能
     考虑到减轻服务器性能方面，应当使用COOKIE。
    4、单个cookie保存的数据不能超过4K，很多浏览器都限制一个站点最多保存20个cookie。
    
    5、所以个人建议：
    将登陆信息等重要信息存放为SESSION
    其他信息如果需要保留，可以放在COOKIE中
    ```

26. 在浏览器中输入www.baidu.com后执行的全部过程

    答:1、客户端浏览器通过DNS解析到[www.baidu.com](http://www.baidu.com/) 的IP地址220.181.27.48，通过这个IP地址找到客户端到服务器的路径。客户端浏览器发起一个HTTP会话到220.181.27.48，然后通过TCP进行封装数据包，输入到网络层。
    2、在客户端的传输层，把HTTP会话请求分成报文段，添加源和目的端口，如服务器使用80端口监听客户端的请求，客户端由系统随机选择一个端口如5000，与服务器进行交换，服务器把相应的请求返回给客户端的5000端口。然后使用IP层的IP地址查找目的端。
    3、客户端的网络层不用关心应用层或者传输层的东西，主要做的是通过查找路由表确定如何到达服务器，期间可能经过多个路由器，这些都是由路由器来完成的工作，我不作过多的描述，无非就是通过查找路由表决定通过那个路径到达服务器。
    4、客户端的链路层，包通过链路层发送到路由器，通过邻居协议查找给定IP地址的MAC地址，然后发送ARP请求查找目的地址，如果得到回应后就可以使用ARP的请求应答交换的IP数据包现在就可以传输了，然后发送IP数据包到达服务器的地址。

27. 当DNS客户机需要在程序中使用名称时，它会查询DNS服务器来解析该名称。客户机发送的每条查询信息包括三条信息：包括：指定的DNS域名，指定的查询类型，DNS域名的指定类别。基于UDP服务，端口53. 该应用一般不直接为用户使用，而是为其他应用服务，如HTTP，SMTP等在其中需要完成主机名到IP地址的转换。

28. ARP

    答:1：首先，每个主机都会在自己的ARP缓冲区中建立一个ARP列表，以表示IP地址和MAC地址之间的对应关系。
    2：当源主机要发送数据时，首先检查ARP列表中是否有对应IP地址的目的主机的MAC地址，如果有，则直接发送数据，如果没有，就向本网段的所有主机发送ARP数据包，该数据包包括的内容有：源主机 IP地址，源主机MAC地址，目的主机的IP 地址。
    3：当本网络的所有主机收到该ARP数据包时，首先检查数据包中的IP地址是否是自己的IP地址，如果不是，则忽略该数据包，如果是，则首先从数据包中取出源主机的IP和MAC地址写入到ARP列表中，如果已经存在，则覆盖，然后将自己的MAC地址写入ARP响应包中，告诉源主机自己是它想要找的MAC地址。
    4：源主机收到ARP响应包后。将目的主机的IP和MAC地址写入ARP列表，并利用此信息发送数据。如果源主机一直没有收到ARP响应数据包，表示ARP查询失败。
    广播发送ARP请求，单播发送ARP响应。

29. 

## 网络

###  计算机网络

1. **知道各个层使用的是哪个数据交换设备。（交换机、路由器、网关）** 

   网关：应用层、传输层（网关在传输层上以实现网络互连，是最复杂的网络互连设备，仅用于两个高层协议不同的网络互连。网关的结构也和路由器类似，不同的是互连层。网关既可以用于广域网互连，也可以用于局域网互连）

   路由器：网络层（路由选择、存储转发）

   交换机：数据链路层、网络层（识别数据包中的 MAC 地址信息，根据 MAC 地址进行转发，并将这些 MAC 地址与对应的端口记录在自己内部的一个地址表中）

   网桥：数据链路层（将两个 LAN 连起来，根据 MAC 地址来转发帧）

   集线器（Hub）：物理层（纯硬件设备，主要用来连接计算机等网络终端）

   中继器：物理层（在比特级别对网络信号进行再生和重定时，从而使得它们能够在网络上传输更长的距离）
   
2. 网络七层模型

   应用层（数据）：确定进程之间通信的性质以满足用户需要以及提供网络与用户应用

   表示层（数据）：主要解决拥护信息的语法表示问题，如加密解密

   会话层（数据）：提供包括访问验证和会话管理在内的建立和维护应用之间通信的机制，如服务器验证用户登录便是由会话层完成的

   传输层（段）：实现网络不同主机上用户进程之间的数据通信，可靠与不可靠的传输，传输层的错误检测，流量控制等

   网络层（包）：提供逻辑地址（IP）、选路，数据从源端到目的端的传输

   数据链路层（帧）：将上层数据封装成帧，用 MAC 地址访问媒介，错误检测与修正

   物理层（比特流）：设备之间比特流的传输，物理接口，电气特性等

3. ARP的作用：

   ARP 为 IP 地址到对应的硬件地址提供动态映射。

4. 点对点链路使用ARP吗？

   不使用

5. ARP高效运行的关键：

   关键是每个主机上都有一个 ARP 的高速缓存。

6. ARP 协议有什么弱点？

   1）缓存：主机的地址映射是基于高速缓存的，动态更新的。地址刷新是有时间限制的。 可以通过下次更新之前修改计算机上的地址缓存，造成拒绝服务攻击或者 ARP 欺骗。

   2）广播: 攻击者可以伪装 ARP 应答。

   3）ARP 应答没有认证，都是合法的。可以在不接受到请求的时候就发出应答包。

7. ：ARP 代理的概念和应用场景

   若 ARP 请求是从一个网络的主机发送给另一个网络上的主机，那么连接这两个网络的路由器就可以回答该请求，这个过程叫做 ARP 代理。ARP 代理路由器响应 ARP 请求的 MAC 地址为路由器的 MAC 地址而非 ARP 请求的主机的 MAC 地址。

   ARP 代理的应用环境：

   两个物理网络之间的路由是使用相同的网络号，两个路由器设置成 ARP 代理，实现相互隐瞒物理网络

8. 免费ARP

   指主机发送 ARP 查找自己的 IP 地址，即数据链路层 SIP=DIP

   作用有两个：

   1）一个主机使用免费 ARP 确定是有存在有其他主机设置了相同的 IP 地址

   2）如果发送免费 ARP 的主机改变了 MAC 地址，可以通过发送免费 ARP 的方式告知其他主机端更新 ARP 表

9. 如何理解 IP 的不可靠和无连接。 
   不可靠：指的是不能保证数据报能成功地到达目的地。
   发生错误时候，丢弃该数据包，发送 ICMP 消息给信源端。 可靠性由上层提供。
   无连接：IP 不维护关于后续数据报的状态信息。
   体现在，IP 数据可以不按顺序发送和接收。A 发送连续的数据报，到达 B 不一定是连续的，来回路由选择可能不一样，路线也不一样，到达先后顺序也不一样。

10. IP 报文的格式和各个字段的含义

    **版本号**： IPV4 就是 4，IPV6 就是 6 （4）

    **首部长度**：4 个字节为单位。最小为 5，最大为 15。所以最小长度 20 个字节，最大为 60个字节。（4）**服务类型**： Qos 用，目前不怎么使用。（8）

    **总长度**：字节为单位。 最多可以传送 65535 字节的 IP 数据包。（16）

    **标识字段**（8）

    **标志** （3）

    **段偏移**（5）与分片有关。

    **生存时间 TTL**：经过一个路由器减一。 字段为 0 时，数据报被丢弃，并且发送 ICMP 报文

    通知源主机。目的是防止数据报在选路时无休止地在网络中流动。（8）

    **协议**：区分上层协议 （8）

    **首部校验和**：仅对首部进行校验。（16）【对比： ICMP，IGMP，TCP，UDP：对首部和数据进行校验】

    **源地址**：（32）

    **目的地址**：(32)

11. 为什么 IP 首部中要有总长度字段？ 
    因为一些数据链路（以太网）需要填充一些数据以达到最小长度。因为以太网帧的最小长度是 46 个字节，但是 IP 长度可能更短，所以需要总长度来确定 IP 数据部分的内容。

12. ：IP 首部校验和怎么计算的，与 ICMP，IGMP，TCP，UDP 的首部校验和有什么区别与共同点？ 

    （1） 先把校验和字段置 0。 （2） 对首部中每个 16 位比特进行二进制反码求和。
    （3） 结果存在检验和字段中。
    （4） 收到一份 IP 数据包后，同样对首部中每个 16bit 二进制反码求和。
    （5） 最后结果全为 1，表示正确，否则表示错误。
    （6） 如果是错误的，IP 就丢弃该数据报，但是不生成差错报文，由上层去处理。
    共同点：用到的算法都是一样的。
    区别：IP 计算的时候没有将数据包括在内。
    ICMP，IGMP，TCP，UDP 同时覆盖首部和数据检验码

13. 主机和路由器

    主机从不把数据报从一个接口转发到另一个接口，而路由器则要转发数据报。

14. IP 路由选择的过程是怎么样的？ 
    根据最长匹配原则，找到条目，发送到指定的路由器。如果不能找到，返回一个“主机不可达”或“网络不可达”的错误。

15. IP 路由选择的特性有什么？ 
    （１） IP 路由选择是逐跳进行的。
    IP 并不知道到达任何目的的完整路径，只提供下一跳地址。
    （２） 为一个网络指定一个路由器，而不是为每个主机指定一个路由器。
    这样可以缩小路由表规模。

16. IP 搜索路由表的步骤 
    搜索匹配的主机地址 ----》搜索匹配的网络地址 ----》搜索默认选项
    IP 层进行的选路实际上是一种选路机制，它搜索路由表并决定向哪个网络接口发送分组。

17. 如果路由表中没有默认项，而又没有找到匹配项，这时如何处理？ 
    结果取决于该 IP 数据报是由主机产生的还是被转发的。
    如果数据报是由本机产生的，那么就给发送该数据报的应用程序返回一个差错，或者是“主机不可达差错”或者是“网络不可达差错”。
    如果是被转发的数据报，就给原始发送一份 ICMP 主机不可达的差错报文。

18. IP 地址的分类，如何划分的，及会计算各类地址支持的主机数 

    1. A 类地址：首位为 0，1.0.0.1~~126.255.255.254；主机号 24 位
    2. B 类地址：首位为 10，128.0.0.1~~191.255.255.254；主机号 16 位
    3. C 类地址：首位为 110，192.0.0.1~~223.255.255.254；主机号 8 位
    4. D 类地址（多播地址，也叫做组播地址）：首位为 1110，224.0.0.1~~239.255.255.254
    5. E 类地址：此类地址是保留地址，首位为 11110，240.0.0.1~~254.255.255.254

19. 

### HTTP



1. 一次完整的HTTP请求所经历的步骤

   1. 在浏览器中输入域名（www.baidu.com）后，客户端浏览器通过DNS解析到www.baidu的IP地址，通过IP地址找到客户端到服务器的路径。客户端浏览器发送一个HTTP会话到IP地址，然后通过TCP封装数据包，输入到网络层
   2. 在客户端的传输层，把HTTP会话请求分成报文段，添加源和项目的端口。服务器使用80端口监听客户端的请求，客户端由系统随机选择一个端口，与服务器进行交换，服务器把相应的请求返回给客户端的5000端口，然后使用IP层的IP地址查找目的端。
   3. 查找路由表指定如何到达服务器。
   4. 查找IP地址的MAC地址，发送ARP请求查找目的地址。
   5. [《抓包实战 | 浏览器里的 HTTP 请求到底是如何完成的？](https://mp.weixin.qq.com/s/_fB7r53BGZRvpG9YAPRQ8A)

   - [阿里面试官问“说一下从 url 输入到返回请求的过程”的难度就是不一样！](https://mp.weixin.qq.com/s?__biz=MzA4Nzg0MDM5Nw==&mid=2247493730&idx=1&sn=84243eb5ddcf2560618bfb2086a96a0a&chksm=9031eb80a74662968e7562a15c9637025dd00de20609f2a7c271b24abda6711423de545dfa44&mpshare=1&scene=23&srcid=0323s8a44g5c8ZEKQMoJbwUm&sharer_sharetime=1616491855557&sharer_shareid=383af18a6aef4a4861a0cc66f7ecde88#rd)

2. 常见的HTTP Method有哪些？GET/POST区别？Header中常见的key/value对有哪些？Header中能存放二进制数据么？你认为Header中，最重要的那个Key/Value对是什么？

3. HTTP缓存

4. HTTP协议的了解

5. HTTP缓存

7. HTTP状态码

   200：请求已成功，请求所希望的响应头或数据体将随此响应返回。 

   302：请求的资源临时从不同的 URI 响应请求。由于这样的重定向是临时的，客户端应当 

   继续向原有地址发送以后的请求。只有在 Cache-Control 或 Expires 中进行了指定的情况下， 

   这个响应才是可缓存的 

   304：如果客户端发送了一个带条件的 GET 请求且该请求已被允许，而文档的内容（自上 

   次访问以来或者根据请求的条件）并没有改变，则服务器应当返回这个状态码。304 响应禁 

   止包含消息体，因此始终以消息头后的第一个空行结尾。 

   403：服务器已经理解请求，但是拒绝执行它。 

   404：请求失败，请求所希望得到的资源未被在服务器上发现。 

   500：服务器遇到了一个未曾预料的状况，导致了它无法完成对请求的处理。一般来说，这 

   个问题都会在服务器端的源代码出现错误时出现

11. IP地址是什么

12. HTTP和HTTPS的区别

    HTTPS就是在HTTP的基础上加入了SSL加密，更加安全

13. get和post方法区别
    本质区别：GET 产生一个 TCP 数据包；POST 产生两个 TCP 数据包。
    GET 方式的请求，浏览器会把 http header 和 data 一并发送出去，服务器响应 200（返回数据）；而对于 POST，浏览器先发送 header，服务器响应 100（continue），浏览器再发送 data，服务器响应 200（返回数据）。

    GET 在浏览器回退时是无害的，而 POST 会再次提交请求。
    GET 产生的 URL 地址可以被 Bookmark，而 POST 不可以。
    GET 请求会被浏览器主动 cache，而 POST 不会，除非手动设置。
    GET 请求只能进行 URL 编码，而 POST 支持多种编码方式。
    GET 请求参数会被完整保留在浏览器历史记录里，而 POST 中的参数不会被保留。
    GET 请求在 URL 中传送的参数是有长度限制的，而 POST 么有。对参数的数据类型，
    GET 只接受 ASCII 字符，而 POST 没有限制。
    GET 比 POST 更不安全，因为参数直接暴露在 URL 上，所以不能用来传递敏感信息。
    GET 参数通过 URL 传递，POST 放在 Request body 中。

10. ：Cookies 和 Session 的区别 
    1. cookie 是一种发送到客户浏览器的文本串句柄，并保存在客户机硬盘上，可以用来在
    某个 WEB 站点会话间持久的保持数据
    2. session 其实指的就是访问者从到达某个特定主页到离开为止的那段时间。 Session 其
    实是利用 Cookie 进行信息处理的，当用户首先进行了请求后，服务端就在用户浏览器
    上创建了一个 Cookie，当这个 Session 结束时，其实就是意味着这个 Cookie 就过期 了
    3. cookie 数据保存在客户端，session 数据保存在服务器端

11. 



### TCP和UDP

1. TCP和UDP的简单介绍

   UDP 是一个简单的面向数据报的运输层协议：进程的每个输出操作都正好产生一个 UDP 数据报，并组装成一份待发送的 IP 数据报。

   TCP 是面向流字符，应用程序产生的全体数据与真正发送的单个 IP 数据报可能没什么联系。

2. 问题 1：TCP 通过哪些方式来保证可靠性？ 1） 应用数据被分割成 TCP 认为最适合发送的数据块。
   2） 确认机制，发送报文后，等待确认。
   3） 重发机制，没有收到确认，将重发数据段。
   4） 保持它首部和数据的校验和。确认数据的准确性。
   5） 排序，丢弃重复的，流量控制。

3. TCP 与 UDP 的概念相互的区别及优劣 

   1. TCP 面向连接，UDP 面向无链接
   2. TCP 面向报文，UDP 面向字节流
   3. TCP 提供可靠传输服务（数据顺序、正确性），UDP 传输不可靠
   4. TCP 协议传输速度慢，UDP 协议传输速度快
   5. TCP 协议对系统资源要求多（头部开销大），UDP 协议要求少

4. TCP、UDP 为什么存在伪包头？ 
   UDP(TCP)检验和：是根据 UDP(TCP)数据报和伪报头计算得到的差错检测值。
   伪报头包含源和目的 IP 地址，以及来自 IP 数据报报头的协议值。IP 数据报在网络中传送时
   包含 UDP 数据报。
   伪报头并不会在网络中传送，校验和中所包含的伪报头内容可以避免目的端错误地接收错误
   路由的数据报。校验和值的计算方法和 IP 报头检验和的计算方法类似

5. 解释三次握手和四次挥手

   **第一次握手**：建立连接。客户端发送连接请求报文段，将SYN位置为1，Sequence Number为x；然后，客户端进入SYN_SEND状态，等待服务器的确认；

   **第二次握手**：服务器收到SYN报文段。服务器收到客户端的SYN报文段，需要对这个SYN报文段进行确认，设置Acknowledgment Number为x+1(Sequence Number+1)；同时，自己自己还要发送SYN请求信息，将SYN位置为1，Sequence Number为y；服务器端将上述所有信息放到一个报文段（即SYN+ACK报文段）中，一并发送给客户端，此时服务器进入SYN_RECV状态； 

   **第三次握手**：客户端收到服务器的SYN+ACK报文段。然后将Acknowledgment Number设置为y+1，向服务器发送ACK报文段，这个报文段发送完毕以后，客户端和服务器端都进入ESTABLISHED状态，完成TCP三次握手。

   > 为什么要三次握手？

   为了防止已失效的连接请求报文段突然又传送到了服务端，因而产生错误。

   具体例子：“已失效的连接请求报文段”的产生在这样一种情况下：client发出的第一个连接请求报文段并没有丢失，而是在某个网络结点长时间的滞留了，以致延误到连接释放以后的某个时间才到达server。本来这是一个早已失效的报文段。但server收到此失效的连接请求报文段后，就误认为是client再次发出的一个新的连接请求。

   于是就向client发出确认报文段，同意建立连接。假设不采用“三次握手”，那么只要server发出确认，新的连接就建立了。由于现在client并没有发出建立连接的请求，因此不会理睬server的确认，也不会向server发送数据。但server却以为新的运输连接已经建立，并一直等待client发来数据。这样，server的很多资源就白白浪费掉了。采用“三次握手”的办法可以防止上述现象发生。例如刚才那种情况，client不会向server的确认发出确认。server由于收不到确认，就知道client并没有要求建立连接。”

   **第一次分手**：主机1（可以使客户端，也可以是服务器端），设置Sequence Number，向主机2发送一个FIN报文段；此时，主机1进入FIN_WAIT_1状态；这表示主机1没有数据要发送给主机2了；

   **第二次分手**：主机2收到了主机1发送的FIN报文段，向主机1回一个ACK报文段，Acknowledgment Number为Sequence Number加1；主机1进入FIN_WAIT_2状态；主机2告诉主机1，我“同意”你的关闭请求；
   **第三次分手**：主机2向主机1发送FIN报文段，请求关闭连接，同时主机2进入LAST_ACK状态；

   **第四次分手**：主机1收到主机2发送的FIN报文段，向主机2发送ACK报文段，然后主机1进入TIME_WAIT状态；主机2收到主机1的ACK报文段以后，就关闭连接；此时，主机1等待2MSL后依然没有收到回复，则证明Server端已正常关闭，那好，主机1也可以关闭连接了。

   #### 为什么要四次分手？

   TCP协议是一种面向连接的、可靠的、基于字节流的运输层通信协议。TCP是全双工模式，这就意味着，当主机1发出FIN报文段时，只是表示主机1已经没有数据要发送了，主机1告诉主机2，它的数据已经全部发送完毕了；但是，这个时候主机1还是可以接受来自主机2的数据；当主机2返回ACK报文段时，表示它已经知道主机1没有数据发送了，但是主机2还是可以发送数据到主机1的；当主机2也发送了FIN报文段时，这个时候就表示主机2也没有数据要发送了，就会告诉主机1，我也没有数据要发送了，之后彼此就会愉快的中断这次TCP连接。

6. 为什么要 3 次握手，4 次挥手 

   1. 3 次握手：防止已过期的连接请求报文突然又传送到服务器，因而产生错误
   2. 4 次挥手：确保数据能够完成传输，但关闭连接时，当收到对方的 FIN 报文通知时，它
   仅仅表示对方没有数据发送给你了；但未必你所有的数据都全部发送给对方了，所以你可以
   未必会马上会关闭 SOCKET,也即你可能还需要发送一些数据给对方之后，再发送 FIN 报文
   给对方来表示你同意现在可以关闭连接了，所以它这里的 ACK 报文和 FIN 报文多数情况下
   都是分开发送的

7. TCP的流量控制机制

   主要是下面的四种机制：
   **慢启动（慢开始）：** 
   1. 慢开始不是指 cwnd 的增长速度慢（指数增长），而是指 TCP 开始发送设置 cwnd=1。
   2. 思路：不要一开始就发送大量的数据，先探测一下网络的拥塞程度，也就是说由小到大
       逐渐增加拥塞窗口的大小。这里用报文段的个数的拥塞窗口大小举例说明慢开始算法，实时
       拥塞窗口大小是以字节为单位的。
   3. 为了防止 cwnd 增长过大引起网络拥塞，设置一个慢开始门限（ssthresh 状态变量）
       当 cnwd＜ssthresh，使用慢开始算法
       当 cnwd=ssthresh，既可使用慢开始算法，也可以使用拥塞避免算法
       当 cnwd＞ssthresh，使用拥塞避免算法

   **拥塞避免：** 

   1. 拥塞避免并非完全能够避免拥塞，是说在拥塞避免阶段将拥塞窗口控制为按线性规律增
      长，使网络比较不容易出现拥塞。

   2. 思路：让拥塞窗口 cwnd 缓慢地增大，即每经过一个往返时间 RTT 就把发送方的拥塞控
      制窗口加一。

   无论是在慢开始阶段还是在拥塞避免阶段，只要发送方判断网络出现拥塞（其根据就是没有
   收到确认，虽然没有收到确认可能是其他原因的分组丢失，但是因为无法判定，所以都当做
   拥塞来处理），就把慢开始门限设置为出现拥塞时的发送窗口大小的一半。然后把拥塞窗口
   设置为 1，执行慢开始算法。

   **快速重传：** 

   1. 快重传要求接收方在收到一个失序的报文段后就立即发出重复确认（为的是使发送方及
       早知道有报文段没有到达对方）而不要等到自己发送数据时捎带确认。快重传算法规定，发
       送方只要一连收到三个重复确认就应当立即重传对方尚未收到的报文段，而不必继续等待设
       置的重传计时器时间到期。
   2. 由于不需要等待设置的重传计时器到期，能尽早重传未被确认的报文段，能提高整个网
       络的吞吐量。

   **快速恢复：** 

   1. 当发送方连续收到三个重复确认时，就执行“乘法减小”算法，把 ssthresh 门限减半。
      但是接下去并不执行慢开始算法。

   2. 考虑到如果网络出现拥塞的话就不会收到好几个重复的确认，所以发送方现在认为网络
      可能没有出现拥塞。所以此时不执行慢开始算法，而是将 cwnd 设置为 ssthresh 的大小，
      然后执行拥塞避免算法。

8. 

### DNS

1. DNS 的概念，用途，DNS 查询的实现算法
   1.  概念
      - 域名解析，ww w.xxx.com 转换成 ip，能够使用户更方便的访问互联网，而不用去记住能够被机器直接读取的 ip 地址
      - DNS 协议运行在 UDP 协议之上，使用端口号 53
   2. 主机解析域名的顺序
      - 浏览器缓存
      - 找本机的 hosts 文件
      - 路由缓存
      - 找 DNS 服务器(本地域名、顶级域名、根域名) 
        - 迭代查询、递归查询 

### CDN

### CORS

- CORS的过程



1. 进程和线程有什么区别 

   > 

   TCP 和 UDP 各自的特点和区别 

   DNS 协议工作流程 

   CDN 是什么（讲一下内容分发网络的定义， 负载均衡， 提高响应速度） 

    https 的加密过程 



### Geolocation

`**Geolocation**` 接口是一个用来获取设备地理位置的可编程的对象，它可以让Web内容访问到设备的地理位置，这将允许Web应用基于用户的地理位置提供定制的信息。说实话：其实`**Geolocation**` 就是用来获取到当前设备的经纬度（位置）

WebSocket使得客户端和服务器之间的数据交换变得更加简单，允许服务端主动向客户端推送数据。在WebSocket API中，浏览器和服务器只需要完成一次握手，两者之间就直接可以创建持久性的连接，并进行双向数据传输。

# 计算机网络

## TCP/TP

TCP/IP协议模型（Transmission Control Protocol/Internet Protocol），包含了一系列构成互联网基础的网络协议，是Internet的核心协议。

基于TCP/IP的参考模型将协议分成四个层次，它们分别是链路层、网络层、传输层和应用层。下图表示TCP/IP模型与OSI模型各层的对照关系。

### 数据链路层

物理层负责0、1比特流与物理设备电压高低、光的闪灭之间的互换。数据链路层负责将0、1序列划分为数据帧从一个节点传输到临近的另一个节点,这些节点是通过MAC来唯一标识的(MAC,物理地址，一个主机会有一个MAC地址)。



![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1ic1rRmG7HyT7y9PkF7h96LPGQFSiamEibjmpibNUYoOghpu5P2eYZAnZy5w/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

- 封装成帧: 把网络层数据报加头和尾，封装成帧,帧头中包括源MAC地址和目的MAC地址。
- 透明传输:零比特填充、转义字符。
- 可靠传输: 在出错率很低的链路上很少用，但是无线链路WLAN会保证可靠传输。
- 差错检测(CRC):接收者检测错误,如果发现差错，丢弃该帧。





### 1、IP协议

IP协议是TCP/IP协议的核心，所有的TCP，UDP，IMCP，IGMP的数据都以IP数据格式传输。要注意的是，IP不是可靠的协议，这是说，IP协议没有提供一种数据未传达以后的处理机制，这被认为是上层协议：TCP或UDP要做的事情。

#### 1.1 IP地址

在数据链路层中我们一般通过MAC地址来识别不同的节点，而在IP层我们也要有一个类似的地址标识，这就是IP地址。

32位IP地址分为网络位和地址位，这样做可以减少路由器中路由表记录的数目，有了网络地址，就可以限定拥有相同网络地址的终端都在同一个范围内，那么路由表只需要维护一条这个网络地址的方向，就可以找到相应的这些终端了。

A类IP地址: 0.0.0.0~127.0.0.0
B类IP地址:128.0.0.1~191.255.0.0
C类IP地址:192.168.0.0~239.255.255.0

#### 1.2 IP协议头

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icnG978hUKrh6s5hc89Nqg1nGD7EZPcsZ3371vyAia4yAtjSsqTibcSm4w/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

这里只介绍:八位的TTL字段。这个字段规定该数据包在穿过多少个路由之后才会被抛弃。某个IP数据包每穿过一个路由器，该数据包的TTL数值就会减少1，当该数据包的TTL成为零，它就会被自动抛弃。

这个字段的最大值也就是255，也就是说一个协议包也就在路由器里面穿行255次就会被抛弃了，根据系统的不同，这个数字也不一样，一般是32或者是64。

### 2、ARP及RARP协议

ARP 是根据IP地址获取MAC地址的一种协议。

ARP（地址解析）协议是一种解析协议，本来主机是完全不知道这个IP对应的是哪个主机的哪个接口，当主机要发送一个IP包的时候，会首先查一下自己的ARP高速缓存（就是一个IP-MAC地址对应表缓存）。

如果查询的IP－MAC值对不存在，那么主机就向网络发送一个ARP协议广播包，这个广播包里面就有待查询的IP地址，而直接收到这份广播的包的所有主机都会查询自己的IP地址，如果收到广播包的某一个主机发现自己符合条件，那么就准备好一个包含自己的MAC地址的ARP包传送给发送ARP广播的主机。

而广播主机拿到ARP包后会更新自己的ARP缓存（就是存放IP-MAC对应表的地方）。发送广播的主机就会用新的ARP缓存数据准备好数据链路层的的数据包发送工作。

RARP协议的工作与此相反，不做赘述。

### 3、ICMP协议

IP协议并不是一个可靠的协议，它不保证数据被送达，那么，自然的，保证数据送达的工作应该由其他的模块来完成。其中一个重要的模块就是ICMP(网络控制报文)协议。ICMP不是高层协议，而是IP层的协议。

当传送IP数据包发生错误。比如主机不可达，路由不可达等等，ICMP协议将会把错误信息封包，然后传送回给主机。给主机一个处理错误的机会，这 也就是为什么说建立在IP层以上的协议是可能做到安全的原因。

TCP/UDP都是是传输层协议，但是两者具有不同的特性，同时也具有不同的应用场景，下面以图表的形式对比分析。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1iciaLnCicT6qytE5CntCqoFmOQfMKE1UNZHoYYc0ibUXd2EPMRpv5lhGicKA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**面向报文**

面向报文的传输方式是应用层交给UDP多长的报文，UDP就照样发送，即一次发送一个报文。因此，应用程序必须选择合适大小的报文。若报文太长，则IP层需要分片，降低效率。若太短，会是IP太小。

**面向字节流**

面向字节流的话，虽然应用程序和TCP的交互是一次一个数据块（大小不等），但TCP把应用程序看成是一连串的无结构的字节流。TCP有一个缓冲，当应用程序传送的数据块太长，TCP就可以把它划分短一些再传送。

关于拥塞控制，流量控制，是TCP的重点，后面讲解。

TCP和UDP协议的一些应用

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icQ3o1iaIPUcwN0ocVwZrdgsLcc2VAKIqHEmVIIIia5OVppBkXOTHa0zmw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

##### 什么时候应该使用TCP？

当对网络通讯质量有要求的时候，比如：整个数据要准确无误的传递给对方，这往往用于一些要求可靠的应用，比如HTTP、HTTPS、FTP等传输文件的协议，POP、SMTP等邮件传输的协议。

##### 什么时候应该使用UDP？

当对网络通讯质量要求不高的时候，要求网络通讯速度能尽量的快，这时就可以使用UDP。

### 七、DNS

DNS（Domain Name System，域名系统），因特网上作为域名和IP地址相互映射的一个分布式数据库，能够使用户更方便的访问互联网，而不用去记住能够被机器直接读取的IP数串。通过主机名，最终得到该主机名对应的IP地址的过程叫做域名解析（或主机名解析）。DNS协议运行在UDP协议之上，使用端口号53。

### 八、TCP连接的建立与终止

#### 1、三次握手

TCP是面向连接的，无论哪一方向另一方发送数据之前，都必须先在双方之间建立一条连接。在TCP/IP协议中，TCP协议提供可靠的连接服务，连接是通过三次握手进行初始化的。三次握手的目的是同步连接双方的序列号和确认号并交换 TCP窗口大小信息。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icW5O1VCcwgHC7kLYG3zaypCExVneJkY3GHLkmQjFydy96CmCErbuaGA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**第一次握手**：建立连接。客户端发送连接请求报文段，将SYN位置为1，Sequence Number为x；然后，客户端进入SYN_SEND状态，等待服务器的确认；

**第二次握手**：服务器收到SYN报文段。服务器收到客户端的SYN报文段，需要对这个SYN报文段进行确认，设置Acknowledgment Number为x+1(Sequence Number+1)；同时，自己自己还要发送SYN请求信息，将SYN位置为1，Sequence Number为y；服务器端将上述所有信息放到一个报文段（即SYN+ACK报文段）中，一并发送给客户端，此时服务器进入SYN_RECV状态； 

**第三次握手**：客户端收到服务器的SYN+ACK报文段。然后将Acknowledgment Number设置为y+1，向服务器发送ACK报文段，这个报文段发送完毕以后，客户端和服务器端都进入ESTABLISHED状态，完成TCP三次握手。

> 为什么要三次握手？

为了防止已失效的连接请求报文段突然又传送到了服务端，因而产生错误。

具体例子：“已失效的连接请求报文段”的产生在这样一种情况下：client发出的第一个连接请求报文段并没有丢失，而是在某个网络结点长时间的滞留了，以致延误到连接释放以后的某个时间才到达server。本来这是一个早已失效的报文段。但server收到此失效的连接请求报文段后，就误认为是client再次发出的一个新的连接请求。

于是就向client发出确认报文段，同意建立连接。假设不采用“三次握手”，那么只要server发出确认，新的连接就建立了。由于现在client并没有发出建立连接的请求，因此不会理睬server的确认，也不会向server发送数据。但server却以为新的运输连接已经建立，并一直等待client发来数据。这样，server的很多资源就白白浪费掉了。采用“三次握手”的办法可以防止上述现象发生。例如刚才那种情况，client不会向server的确认发出确认。server由于收不到确认，就知道client并没有要求建立连接。”

#### 2、四次挥手

当客户端和服务器通过三次握手建立了TCP连接以后，当数据传送完毕，肯定是要断开TCP连接的啊。那对于TCP的断开连接，这里就有了神秘的“四次分手”。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icaK6BzTE10Z1oHwd7NAqTMG4iaOT1PiatHA37klzT1NBSibsMTSlDk6WAQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

**第一次分手**：主机1（可以使客户端，也可以是服务器端），设置Sequence Number，向主机2发送一个FIN报文段；此时，主机1进入FIN_WAIT_1状态；这表示主机1没有数据要发送给主机2了；

**第二次分手**：主机2收到了主机1发送的FIN报文段，向主机1回一个ACK报文段，Acknowledgment Number为Sequence Number加1；主机1进入FIN_WAIT_2状态；主机2告诉主机1，我“同意”你的关闭请求；
**第三次分手**：主机2向主机1发送FIN报文段，请求关闭连接，同时主机2进入LAST_ACK状态；

**第四次分手**：主机1收到主机2发送的FIN报文段，向主机2发送ACK报文段，然后主机1进入TIME_WAIT状态；主机2收到主机1的ACK报文段以后，就关闭连接；此时，主机1等待2MSL后依然没有收到回复，则证明Server端已正常关闭，那好，主机1也可以关闭连接了。

#### 为什么要四次分手？

TCP协议是一种面向连接的、可靠的、基于字节流的运输层通信协议。TCP是全双工模式，这就意味着，当主机1发出FIN报文段时，只是表示主机1已经没有数据要发送了，主机1告诉主机2，它的数据已经全部发送完毕了；但是，这个时候主机1还是可以接受来自主机2的数据；当主机2返回ACK报文段时，表示它已经知道主机1没有数据发送了，但是主机2还是可以发送数据到主机1的；当主机2也发送了FIN报文段时，这个时候就表示主机2也没有数据要发送了，就会告诉主机1，我也没有数据要发送了，之后彼此就会愉快的中断这次TCP连接。

#### 为什么要等待2MSL？

MSL：报文段最大生存时间，它是任何报文段被丢弃前在网络内的最长时间。原因有二：

- 保证TCP协议的全双工连接能够可靠关闭
- 保证这次连接的重复数据段从网络中消失

第一点：如果主机1直接CLOSED了，那么由于IP协议的不可靠性或者是其它网络原因，导致主机2没有收到主机1最后回复的ACK。那么主机2就会在超时之后继续发送FIN，此时由于主机1已经CLOSED了，就找不到与重发的FIN对应的连接。所以，主机1不是直接进入CLOSED，而是要保持TIME_WAIT，当再次收到FIN的时候，能够保证对方收到ACK，最后正确的关闭连接。

第二点：如果主机1直接CLOSED，然后又再向主机2发起一个新连接，我们不能保证这个新连接与刚关闭的连接的端口号是不同的。也就是说有可能新连接和老连接的端口号是相同的。一般来说不会发生什么问题，但是还是有特殊情况出现：假设新连接和已经关闭的老连接端口号是一样的，如果前一次连接的某些数据仍然滞留在网络中，这些延迟数据在建立新连接之后才到达主机2，由于新连接和老连接的端口号是一样的，TCP协议就认为那个延迟的数据是属于新连接的，这样就和真正的新连接的数据包发生混淆了。所以TCP连接还要在TIME_WAIT状态等待2倍MSL，这样可以保证本次连接的所有数据都从网络中消失。

### 九、TCP流量控制

如果发送方把数据发送得过快，接收方可能会来不及接收，这就会造成数据的丢失。所谓流量控制就是让发送方的发送速率不要太快，要让接收方来得及接收。

利用**滑动窗口机制**可以很方便地在TCP连接上实现对发送方的流量控制。

设A向B发送数据。在连接建立时，B告诉了A：“我的接收窗口是 rwnd = 400 ”(这里的 rwnd 表示 receiver window) 。因此，发送方的发送窗口不能超过接收方给出的接收窗口的数值。请注意，TCP的窗口单位是字节，不是报文段。假设每一个报文段为100字节长，而数据报文段序号的初始值设为1。大写ACK表示首部中的确认位ACK，小写ack表示确认字段的值ack。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icvniazgsSmDkS3e9wFZNErfMqmIlTicAafYOFheibs7ibyqTpUCeicegJoSg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

从图中可以看出，B进行了三次流量控制。第一次把窗口减少到 rwnd = 300 ，第二次又减到了 rwnd = 100 ，最后减到 rwnd = 0 ，即不允许发送方再发送数据了。这种使发送方暂停发送的状态将持续到主机B重新发出一个新的窗口值为止。B向A发送的三个报文段都设置了 ACK = 1 ，只有在ACK=1时确认号字段才有意义。

TCP为每一个连接设有一个持续计时器(persistence timer)。只要TCP连接的一方收到对方的零窗口通知，就启动持续计时器。若持续计时器设置的时间到期，就发送一个零窗口控测报文段（携1字节的数据），那么收到这个报文段的一方就重新设置持续计时器。

### 十、TCP拥塞控制

发送方维持一个拥塞窗口 cwnd ( congestion window )的状态变量。拥塞窗口的大小取决于网络的拥塞程度，并且动态地在变化。发送方让自己的发送窗口等于拥塞窗口。

发送方控制拥塞窗口的原则是：只要网络没有出现拥塞，拥塞窗口就再增大一些，以便把更多的分组发送出去。但只要网络出现拥塞，拥塞窗口就减小一些，以减少注入到网络中的分组数。

慢开始算法：

当主机开始发送数据时，如果立即所大量数据字节注入到网络，那么就有可能引起网络拥塞，因为现在并不清楚网络的负荷情况。因此，较好的方法是 先探测一下，即由小到大逐渐增大发送窗口，也就是说，由小到大逐渐增大拥塞窗口数值。

通常在刚刚开始发送报文段时，先把拥塞窗口 cwnd 设置为一个最大报文段MSS的数值。而在每收到一个对新的报文段的确认后，把拥塞窗口增加至多一个MSS的数值。用这样的方法逐步增大发送方的拥塞窗口 cwnd ，可以使分组注入到网络的速率更加合理。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1ic9dW4gMLAjvAYvlPicyP6Ws6iacAKz2xscqqSXQkljRxquBYRVVnxtlEA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

每经过一个传输轮次，拥塞窗口 cwnd 就加倍。一个传输轮次所经历的时间其实就是往返时间**RTT**。不过“传输轮次”更加强调：把拥塞窗口cwnd所允许发送的报文段都连续发送出去，并收到了对已发送的最后一个字节的确认。

另，慢开始的“慢”并不是指cwnd的增长速率慢，而是指在TCP开始发送报文段时先设置cwnd=1，使得发送方在开始时只发送一个报文段（目的是试探一下网络的拥塞情况），然后再逐渐增大cwnd。

为了防止拥塞窗口cwnd增长过大引起网络拥塞，还需要设置一个慢开始门限ssthresh状态变量。慢开始门限ssthresh的用法如下：

- 当 cwnd < ssthresh 时，使用上述的慢开始算法。
- 当 cwnd > ssthresh 时，停止使用慢开始算法而改用拥塞避免算法。
- 当 cwnd = ssthresh 时，既可使用慢开始算法，也可使用拥塞控制避免算法。拥塞避免

**拥塞避免**

让拥塞窗口cwnd缓慢地增大，即每经过一个往返时间RTT就把发送方的拥塞窗口cwnd加1，而不是加倍。这样拥塞窗口cwnd按线性规律缓慢增长，比慢开始算法的拥塞窗口增长速率缓慢得多。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icuk5H7XxwTsHHicdVr4ajmxWS8ZQAicv3f4vSMnpMvlw9sXuhbfY1ibJAQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

无论在慢开始阶段还是在拥塞避免阶段，只要发送方判断网络出现拥塞（其根据就是没有收到确认），就要把慢开始门限ssthresh设置为出现拥塞时的发送 方窗口值的一半（但不能小于2）。然后把拥塞窗口cwnd重新设置为1，执行慢开始算法。

这样做的目的就是要迅速减少主机发送到网络中的分组数，使得发生 拥塞的路由器有足够时间把队列中积压的分组处理完毕。

如下图，用具体数值说明了上述拥塞控制的过程。现在发送窗口的大小和拥塞窗口一样大。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1icPYWNJ7I6HGd8m4GfKR4asnxsOEHL5tSdlHpYK23tg43rgwe7uy02QQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

### 2、快重传和快恢复

#### 快重传

快重传算法首先要求接收方每收到一个失序的报文段后就立即发出重复确认（为的是使发送方及早知道有报文段没有到达对方）而不要等到自己发送数据时才进行捎带确认。

![图片](https://mmbiz.qpic.cn/mmbiz/yNKv1P4Q9eXxLvDTCzZNz2JwNsQx4x1ic6ibAd2L7Nkk77ethS8Vc436xiagR4sIUXVyC8R9icrP7cbYiboiaVd4vibGA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)

接收方收到了M1和M2后都分别发出了确认。现在假定接收方没有收到M3但接着收到了M4。

显然，接收方不能确认M4，因为M4是收到的失序报文段。根据 可靠传输原理，接收方可以什么都不做，也可以在适当时机发送一次对M2的确认。

但按照快重传算法的规定，接收方应及时发送对M2的重复确认，这样做可以让 发送方及早知道报文段M3没有到达接收方。发送方接着发送了M5和M6。接收方收到这两个报文后，也还要再次发出对M2的重复确认。这样，发送方共收到了 接收方的四个对M2的确认，其中后三个都是重复确认。

快重传算法还规定，发送方只要一连收到三个重复确认就应当立即重传对方尚未收到的报文段M3，而不必 继续等待M3设置的重传计时器到期。

由于发送方尽早重传未被确认的报文段，因此采用快重传后可以使整个网络吞吐量提高约20%。

#### 快恢复

与快重传配合使用的还有快恢复算法，其过程有以下两个要点：

- 当发送方连续收到三个重复确认，就执行“乘法减小”算法，把慢开始门限ssthresh减半。
- 与慢开始不同之处是现在不执行慢开始算法（即拥塞窗口cwnd现在不设置为1），而是把cwnd值设置为 慢开始门限ssthresh减半后的数值，然后开始执行拥塞避免算法（“加法增大”），使拥塞窗口缓慢地线性增大。



**https://juejin.im/post/6844903490595061767**

https://mp.weixin.qq.com/s/MzQ-h_y5rLam1PPGXKGrsw

### TEST



## HTTP 

https://mp.weixin.qq.com/s/RCwtQDwIFzDyOjw-L4l7Vw

### HTTP请求过程

- 对 www.abc.com 这个网址进行 DNS 域名解析，得到对应的 IP 地址
- 根据这个 IP ，找到对应的服务器，发起 TCP 的三次握手
- 建立 TCP 连接后发起 HTTP 请求
- 服务器响应 HTTP 请求，浏览器得到 html 代码
- 浏览器解析 html 代码，并请求 html 代码中的资源（如 js 、 css 、图片等）（先得到 html 代码，才能去找这些资源）
- 浏览器对页面进行渲染呈现给用户
- 服务器关闭关闭 TCP 连接

### HTTP 的请求方式场景 

> Get 方法：获取数据通常(查看数据)-查看
>
> POST 方法：向服务器提交数据通常(创建数据)-create
>
> PUT 方法：向服务器提交数据通常(更新数据)-update，与POST方法很像，也是提交数据，但PUT 制定了资源在服务器上的位置，常用在修改数据
>
> HEAD 方法：只请求页面的首部信息 DELETE 方法：删除服务器上的资源
>
> OPTIONS 方法：用于获取当前URL支持的请求方式
>
> TRACE方法：用于激活一个远程的应用层请求消息回路
>
> CONNECT 方法：把请求链接转换到透明的TCP/IP的通道

### 状态码

状态码一共分为5类。

> 1××：处于中间状态，还需后续操作
>
> 2××：成功收到报文并正确处理

"200 OK"

最常见的成功状态码，表示一切正常，客户端获得期许的处理结果。如果不是Head请求，那么在响应头中通常会有body数据。

"204 No Content"

这个的含义和"200"很相似，不同之处在于它的响应头中没有body数据。

"206 Partial Content"

是 HTTP 分块下载或断点续传的基础，在客户端发送“范围请求”、要求获取资源的部分数据时出现，它与 200 一样，也是服务器成功处理了请求，但 body 里的数据不是资源的全部，而是其中的一部分。状态码 206 通常还会伴随着头字段“Content-Range”，表示响应报文里 body 数据的具体范围，供客户端确认，例如“Content-Range: bytes 0-99/5000”，意思是此次获取的是总计 5000 个字节的前 100 个字节。

> 3××：重定向到其他资源位置

"301 Moved Permanently"

“永久重定向”，意思是本地请求的资源以及不存在，使用新的URI再次访问。

“302 Found”

“Moved Temporarily”，“临时重定向”，临时则所请求的资源暂时还在，但是目前需要用另一个URI访问。

301 和 302 通过在字段Location中表明需要跳转的URI。两者最大的不同在于一个是临时改变，一个是永久改变。举个例子，有时候需要将网站全部升级为HTTPS，这种永久性改变就需要配置永久的"301"。有时候晚上更新系统，系统暂时不可用，可以配置"302"临时访问，此时不会做缓存优化，第二天还会访问原来的地址。

“304 Not Modified”

运用于缓存控制。它用于 If-Modified-Since 等条件请求，表示资源未修改，可以理解成“重定向已到缓存的文件”（即“缓存重定向”）。

> 4××：请求报文有误，服务器无法处理

"400 Bad Request”

通用错误码，表示请求报文有错误，但是这个错误过于笼统。不知道是客户端还是哪里的错误，所以在实际应用中，通常会返回含有明确含义的状态码。

“403 Forbidden”

注意了，这一个是表示服务器禁止访问资源。原因比如涉及到敏感词汇、法律禁止等。当然，如果能让客户端有一个清晰的认识，可以考虑说明拒绝的原因并返回即可。

“404 Not Found”

这可能是我们都知道且都不想看到的状态码之一，它的本意是想要的资源在本地未找到从而无法提供给服务端，但是现在，只要服务器"耍脾气"就会给你返回 404，而我们也无从得知后面到底是真的未找到，还是有什么别的原因，

"405 Method Not Allowed"

获取资源的方法好几种，我们可以对某些方法进行限制。例如不允许 POST 只能 GET；

"406 Not Acceptable"

客户端资源无法满足客户端请求的条件，例如请求需要中文但只有英文；

"408 Request Timeout"

请求超时，服务器等待了过长的时间；

"409 Conflict"：

多个请求发生了冲突，可以理解为多线程并发时的竞态；

413 Request Entity Too Large：

请求报文里的 body 太大；

414 Request-URI Too Long：请求行里的 URI 太大；

429 Too Many Requests：客户端发送了太多的请求，
通常是由于服务器的限连策略；

431 Request Header Fields Too Large：请求头某个字
段或总体太大；

> 5××：服务器错误，服务器对请求出的时候发生内部错误。

“500 Internal Server Error”

和400 类似，属于一个通用的错误码，但是服务器到底是什么错误我们不得而知。其实这是好事，尽量少的将服务器资源暴露外网，尽量保证服务器的安全。

“502 Bad Gateway”

通常是服务器作为网关或者代理时返回的错误码，表示服务器自身工作正常，访问后端服务器时发生了错误，但具体的错误原因也是不知道的。

“503 Service Unavailable”

表示服务器当前很忙，暂时无法响应服务，我们上网时有时候遇到的“网络服务正忙，请稍后重试”的提示信息就是状态码 503。

503 是一个“临时”的状态，

暂时比较忙，稍后提供服务。在响应报文中的“Retry-After”字段，指示客户端可以在多久以后再次尝试发送请求。

### 从浏览器地址栏输入URL后发生了什么？ 

##### 基础版本

> 的浏览器根据请求的URL 交给 DNS域名解析，找到真实 IP，向服务器发起请求；
>
> 服务器交给后台处理完成后返回数据，浏览器接收文件（ HTML、JS、CSS 、图象等）；
>
> 浏览器对加载到的资源（ HTML、JS、CSS 等）进行语法解析，建立相应的内部数据结构（如
>
> HTML 的 DOM ）；
>
> 载入解析到的资源文件，渲染页面，完成。

##### 详细版

> 从浏览器接收 url 到开启网络请求线程（这一部分可以展开浏览器的机制以及进程与线程之间的关系）
>
> 开启网络线程到发出一个完整的 HTTP 请求（这一部分涉及到dns查询， TCP/IP请求，五层因特网协议栈等知识）从服务器接收到请求到对应后台接收到请求（这一部分可能涉及到负载均衡，安全拦截以及后台内部的处理等等）
>
> 后台和前台的 HTTP 交互（这一部分包括 HTTP头部、响应码、报文结构、 cookie 等知识，可以提下静态资源的 cookie优化，以及编码解码，如 gzip 压缩等）
>
> 单独拎出来的缓存问题， HTTP 的缓存（这部分包括http缓存头部， ETag ， catchcontrol 等）
>
> 浏览器接收到HTTP数据包后的解析流程（解析html -词法分析然后解析成dom树、解析 css 生成 css规则树、合并成 render 树，然后 layout 、 painting渲染、复合图层的合成、 GPU 绘
>
> 制、外链资源的处理、 loaded 和 DOMContentLoaded等）
>
> CSS 的可视化格式模型（元素的渲染规则，如包含块，控制框， BFC， IFC 等概念）
>
> JS 引擎解析过程（JS的解释阶段，预处理阶段，执行阶段生成执行上下文，VO，作用域链、回收机制等等）

其它（可以拓展不同的知识模块，如跨域，web安全， hybrid 模式等等内容）**详细升级版**

> 在浏览器地址栏输入URL
>
> 浏览器查看缓存，如果请求资源在缓存中并且新鲜，跳转到转码步骤
>
> 如果资源未缓存，发起新请求
>
> 如果已缓存，检验是否足够新鲜，足够新鲜直接提供给客户端，否则与服务器进行验证。
>
> 检验新鲜通常有两个HTTP头进行控制 Expires 和 Cache-Control ：

2.3.1 HTTP1.0提供Expires，值为一个绝对时间表示缓存新鲜日期

> 2.3.2 HTTP1.1增加了Cache-Control: max-age= ,值为以秒为单位的 大新鲜时间浏览器解析URL获取协议，主机，端口，path 浏览器组装一个HTTP（GET）请求报文浏览器获取主机ip地址，过程如下：
>
> 浏览器缓存
>
> 本机缓存 hosts文件路由器缓存
>
> ISP DNS缓存
>
> DNS递归查询（可能存在负载均衡导致每次IP不一致）打开一个socket与目标IP地址，端口建立TCP链接，三次握手如下：
>
> 客户端发送一个TCP的SYN=1，Seq=X的包到服务器端口服务器发回SYN=1，ACK=x+1,Seq=Y的相应包客户端发送ACK=Y+1，Seq=z
>
> TCP链接建立后发送HTTP请求
>
> 服务器接收请求后解析，将请求转发到服务器程序，如虚拟主机使用HTTP Host头部判断请求的服务程序
>
> 服务器检测HTTP请求头是否包含缓存验证信息，如果验证缓存新鲜，返回304等对应状态出合理程序读取完整请求并准备HTTP相应，可能需要查询数据库等操作服务器将相应报文通过TCP链接发送回浏览器
>
> 浏览器接收HTTP相应，然后根据情况选择关闭TCP链接或者保留重用，关闭TCP链接的四次握手如下：
>
> 主动方发送Fin=1,ACK=z,Seq=x报文被动方发送ACK=X+1,Seq=Y报文
>
> 被动方发送Fin=1,ACK=X,Seq=Y报文主动方发送ACK=Y,Seq=x报文浏览器检查相应状态码
>
> 如果资源可缓存，进行缓存对相应进行解码
>
> 根据资源类型决定如何处理
>
> 解析HTML文档，构建DOM树，下载资源，构建CSSOM树，执行js脚本，这些操作每月严格的先后顺序
>
> 构建DOM树：
>
> Tokenizing：根据HTML规范将字符流解析为标记
>
> Lexing：词法分析将标记转换为对象并定义属性和规则
>
> DOM construction：根据HTML标记关系将对象组成DOM树解析过程中遇到图片、样式表、js文件，启动下载构建CSSOM树：
>
> Tokenizing：字符流转换为标记流
>
> Node：根据标记创建节点
>
> CSSOM：节点创建CSSOM树根据DOM树和CSSOM树构建渲染树
>
> 从DOM树的根节点遍历所有可见节点，不可见节点包括：1） script , meta这样本身不可见的标签。2)被css隐藏的节点，如 display: none 对每一个可见节点，找到恰当的CSSOM规则并应用发布可视节点的内容和计算样式 js解析如下
>
> 浏览器创建Document对象并解析HTML，将解析到的元素和文本节点添加到文档中，此时
>
> document.readystate为loading
>
> HTML解析器遇到没有async和defer的script时，将他们添加到文档中，然后执行行内或外部脚本。这些脚本会同步执行，并且在脚本下载和执行时解析器会暂停。这样就可以用
>
> document.write()把文本插入到输入流中。同步脚本经常简单定义函数和注册事件处理程序，他们可以遍历和操作script和他们之前的文档内容
>
> 当解析器遇到设置了async属性的script时，开始下载脚本并继续解析文档。脚本会在它下载完成后尽快执行，但是解析器不会停下来等它下载。异步脚本禁止使用 document.write()，它们可以访问自己script和之前的文档元素
>
> 当文档完成解析，document.readState变成interactive
>
> 所有defer脚本会按照在文档出现的顺序执行，延迟脚本能访问完整文档树，禁止使用
>
> document.write()
>
> 浏览器在Document对象上触发DOMContentLoaded事件
>
> 此时文档完全解析完成，浏览器可能还在等待如图片等内容加载，等这些内容完成载入并且所
>
> 有异步脚本完成载入和执行，document.readState变为complete，window触发load事件 显示页面（HTML解析过程中会逐步显示页面）

## GET和POST的区别

GET 参数通过 url 传递，POST 放在 body 中。（http 协议规定，url 在请求头中，所以大小限制很小）

GET 请求在 url 中传递的参数是有长度限制的，而 POST 没有。原因见上↑↑↑

GET 在浏览器回退时是无害的，而 POST 会再次提交请求

GET 请求会被浏览器主动 cache，而 POST 不会，除非手动设置

GET 比 POST 更不安全，因为参数直接暴露在 url 中，所以不能用来传递敏感信息对参数的数据类型，GET 只接受 ASCII字符，而 POST 没有限制

GET 请求只能进行 url(x-www-form-urlencoded)编码，而 POST 支持多种编码方式

**GET 产生一个 TCP 数据包；POST 产生两个 TCP 数据包**。对于 GET 方式的请求，浏览器会把 http 的 header 和 data 一并发送出去，服务器响应200（返回数据）。而对于 POST，浏览器先发送 header，服务器响应100 continue，浏览器再发送 data，服务器响应200 ok（返回数据）

## reflow

浏览器为了重新渲染部分或整个页面，重新计算页面元素位置和几何结构的进程叫做 reflow . 通俗点说就是当开发人员定义好了样式后(也包括浏览器的默认样式),浏览器根据这些来计算并根据结果将元素放到它应该出现的位置上，这个过程叫做 reflow . 由于reflow是一种浏览器中的用户拦截操作，所以我们了解如何减少 reflow 次数，及DOM的层级，css 效率对 refolw 次数的影响是十分有必要的。 reflow

(回流)是导致DOM脚本执行效率低的关键因素之一，页面上任何一个节点触发了 reflow，会导致它的子节点及祖先节点重新渲染。 简单解释一下 Reflow：当元素改变的时候，将会影响文档内容或结构，或元素位置，此过程称为 Reflow。

当p节点上发生reflow时，hello和body也会重新渲染，甚至h5和ol都会收到影响。

#### 什么时候会导致reflow发生呢？ 

改变窗口大小改变文字大小添加/删除样式表

内容的改变，(用户在输入框中写入内容也会) 激活伪类，如:hover

操作class属性脚本操作DOM

计算offsetWidth和offsetHeight 设置style属性

#### 减少reflow对性能的影响 

- 不要一条一条地修改 DOM 的样式，预先定义好 class，然后修改 DOM 的 className

- 把 DOM 离线后修改，比如：先把 DOM 给 display:none (有一次 Reflow)，然后你修改100次，然后再把它显示出来

- 不要把 DOM 结点的属性值放在一个循环里当成循环里的变量尽可能不要修改影响范围比较大的 DOM

- 为动画的元素使用绝对定位 absolute / fixed 不要使用 table 布局，可能很小的一个小改动会造成整个 table 的重新布局尽可能限制reflow的影响范围，尽可能在低层级的DOM节点上，上述例子中，如果你要改变p的样式，class就不要加在div上，通过父元素去影响子元素不好。

- 避免设置大量的 style 属性，因为通过设置 style 属性改变结点样式的话，每一次设置都会触发一次 reflow，所以 好是使用 class 属性

- 实现元素的动画，它的position属性， 好是设为absoulte或fixed，这样不会影响其他元素的布局

- 动画实现的速度的选择。比如实现一个动画，以1个像素为单位移动这样 平滑，但是reflow就会过于频繁，大量消耗CPU资源，如果以3个像素为单位移动则会好很多。

- 不要使用 table 布局，因为table中某个元素旦触发了 reflow，那么整个 table 的元素都会触发reflow 。那么在不得已使用 table 的场合，可以设置 table-layout:auto; 或者是 table-layout:fixed 这样可以让table一行一行的渲染，这种做法也是为了限制reflow的影响范围

如果CSS里面有计算表达式，每次都会重新计算一遍，触发一次reflow。





### HTTP2的多路复用

HTTP2 采用**二进制格式传输**，取代了 HTTP1.x 的文本格式，二进制格式解析更 高效。 

多路复用代替了 HTTP1.x 的序列和阻塞机制，所**有的相同域名请求都通过同一 个 TCP 连接并发完成**。 

在 HTTP1.x 中，并发多个请求需要多个 TCP 连接，浏览器为了控制资源会有 6-8 个 TCP 连接都限制。

HTTP2 中 同域名下所有通信都在单个连接上完成，消除了因多个 TCP 连接而带来的延 时和内存消耗。 

单个连接上可以并行交错的请求和响应，之间互不干扰



### ***HTTPS***

> 好人占多数，坏人也不少。总有些要搞坏事，因为HTTP是明文，所以需要想办法保护明文，从而出现了https。

安全是什么

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpapmt3FrQcmuVOHTaOsp7tH0D6icwtib1tCBcDfezgUqqOiaY5HZsGrZX8Q/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)安全四要素

机密性

> 对信息进行保密，只能可信的人可以访问(让我想起时间管理者)。

完整性

> 数据在传输过程中内容不被"篡改"。虽然机密性对数据进行保密了，但是有上策也有下策(hack)

身份认证

> 证明自己的身份是本人，保证其消息发给可信的人

不可否认

> 君子一言驷马难追，说话算数，说过的话做过的事要有所保证

HTTPS

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaCkba38X1vyEKico3wb7ce5YeRWwGSCwdxyfLMdWciak6Kh1nZpCQ4ymw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)HTTP和HTTPS

从上图我们知道HTTPS无非是在传输层和应用层中间加了一层TLS，正是TLS紧跟当代密码学的步伐，尽全力的保障用户的安全。老规矩，我们用wireshark看看长什么样子。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaiad2T3qljudOiaygZdBf1ic2jMeuuNG8wARE4ydDcichfia31CAkib6DytZQ/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)TLS

可以看出在交互的过程中多了不少新东西，了解TLS,TLS由SSL握手协议，SSL修改密码规范协议，SSL警报协议，SSL记录协议组成。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaYGiareDAib1UAhqv0eY9mQug0ySa5c05PrKDjMQWnLDiafAVk5I6V0oaA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)TLS组成

SSL握手协议：

> 相对于三次握手

记录协议

> 记录为TLS发送接收数据的基本单位。它的自协议需要通过记录协议发出。如果多个纪录数据则可以一个TCP包一次性发出。

警报协议

> 类似HTTP状态码，通过反馈不同的消息进行不同的策略。

变更密码规范协议

> 告诉对方，从此刻开始，后续的数据将使用加密算法进行加密再传输。

对称加密与非对称加密

对称加密

> 对称加密，顾名思义，加密方与解密方使用同一钥匙(秘钥)。具体一些就是，发送方通过使用相应的加密算法和秘钥，对将要发送的信息进行加密；对于接收方而言，使用解密算法和相同的秘钥解锁信息，从而有能力阅读信息。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaQoSrn1r5IHNsiav1pXQHick2uOf2CbkWictlQFaYcNvxttwdZ8ialstSibA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)对称加密

*非对称加密*

> 在对称加密中，发送方与接收方使用相同的秘钥。那么在非对称加密中则是发送方与接收方使用的不同的秘钥。其主要解决的问题是防止在秘钥协商的过程中发生泄漏。比如在对称加密中，小蓝将需要发送的消息加密，然后告诉你密码是123balala,ok,对于其他人而言，很容易就能劫持到密码是123balala。那么在非对称的情况下，小蓝告诉所有人密码是123balala,对于中间人而言，拿到也没用，因为没有私钥。所以，非对称密钥其实主要解决了密钥分发的难题。如下图

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaoeU4ZpadacuuYaxsDwrjzFBrTTsue2LdVYbW69zdYV8lVKatibPYyew/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)非对称加密

> 其实我们经常都在使用非对称加密，比如使用多台服务器搭建大数据平台hadoop，为了方便多台机器设置免密登录，是不是就会涉及到秘钥分发。再比如搭建docker集群也会使用相关非对称加密算法。

*混合加密*

> 非对称加密算法，大多数是从数学问题演变而来，运算速度较慢。混合加密所谓取长补短。通信过程中使用RSA等解决密钥交换问题，然后使用随机数产生的在对称算法中的会话密钥，最后使用加密。对方使用私钥解密得到的密文取出会话秘钥，这样就实现了密钥交换。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpannAFZM7BkDylZkgrQXdMtDLLxn0fiaH0plBOAowxaqLBqkpFQicYiacvw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)混合加密

通过混淆加密等方式完成了机密性任务，作为Hack只需要伪造发布公钥或者作为之间人窃听密文。但是我们知道安全是四要素，还需要保证数据的完整性，身份认证等。

*摘要*

> 摘要算法可以理解为一种特殊的"单向"加密算法，无密钥，不可逆。在平时项目中，应该大家都是用过MD5，SHA-1。但是在TLS中使用SHA-2。

假设小A转账5000给小C，小A加上SHA-2摘要。网站计算摘要并对比，如果一致则完整可信。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaKwW8b5SusXuAeBIPZr203KJiacWB32Iich9icAh36OrricUHhZZic70rsuw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)摘要可信

此时小B想修改小A给的money，这个时候网站计算摘要就会发现不一样，不可信

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpassSXjYHKzfUzZcjkE5cOFOfLDVe9FWyC97N3U3YkUmJFBJANa76pGA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)摘要不可信

HTTPS请求建立连接过程

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpazwxDBTVR4J2Wxd54oWGrFxgKI9vl0lb15lojwfDMgmLovy56xXiag9Q/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)HTTP握手过程

注意：

1. 首先通过非对称加密建立通信过程
2. 在握手阶段，为什么使用3个随机数，一方面防止「随机数 C」被猜出，另一方增加Session key随机性
3. Client发出支持的「对称/非对称加密」算法
4. server返回选用的「对称/非对称加密」算法
5. Client对算法进行确认
6. Server对算法进行确认

根据wireshak结果，对TLS进一步剖析。TCP三次握手建立连接，作为礼貌，Client先打招呼"Client Hello"。里面包含了Client的版本号、所支持的密码套件和随机数，如下图所示

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpa6ssaqJialF2C9eCoqDvEPWzTvtol8lx5IWZKmwzCibFfFia3E6AO1EoibA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)Client Hello

Server端表示尊重，回复"Server Hello",同时进行版本校对，给出随机数(Server Random)，从Client算法列表中选择一个密码套件，在这里选择的"TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256"。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpacj0fCXXicrXwSU0SnwGcUutGa15saF7zZhRPv2OWCnQsicXdXGthicE6g/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)cipher Suite

这里的"TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256"什么意思呢

> 密码套件选择椭圆曲线加RSA、AES、SHA256

双方通过证书验证身份。因为本机服务器选用了ECDHE算法，为了实现密钥交换算法，它会发送证书后把椭圆曲线的公钥（Server Params）连带"Server Key Exchange"消息发送出去。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpaur9zLqGhl7dcqmlibByWKhE2Ld0kQicuEUPDV2hbKdia2EmOnQ66KTE8g/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)Server Key Exchange

意思是，刚才混合加密套件比较复杂，给你个算法参数，好好记住，别弄丢了。

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpagHxO3KvZEC3NK13RG3ViciaLADOBXm5vGWej2J2d7CMBVQtEvLTDcFQw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)ServerHelloDone

随后服务端回复"hello done"告知打招呼完毕

打完招呼完毕后，客户端对证书进行核实。然后根据密码套件也生成椭圆曲线的公钥，用"Client Key Exchange"消息发给服务器

![图片](https://mmbiz.qpic.cn/mmbiz_png/NdsdouZwicacugPgPuxCgLUTf9ErM0xpar7orILcibrplzxHibNLicecD3XDEfvtJZpyW6tpVF6BrI6JibiczqY3koPw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1)Client Key Exchange

此时客户端和服务端都有了密钥交换的两个参数(Client Params、ServerParams），然后通过 ECDHE 算法算出了一个新的值，叫“Pre-Master”

有了主密钥和会话密钥，客户端发送“Change Cipher Spec”和“Finished”消息，最后将所有消息加上摘要发送给服务器验证。

服务器同样发送“Change Cipher Spec”和“Finished”消息，握手结束，开始进行HTTP请求与响应

4 初探域名

> 我们知道域名的出现让我们更容易记忆，按照"."分割，越靠近右边级别越高。域名本质是一个名字空间系统，采用多级域名的方式区分不同的国家，公司等，作为一种身份的标识。

根域名服务器（Root DNS Server）：管理顶级域名服务器，返回“com”“net”“cn”等顶级域名服务器的 IP 地址；

顶级域名服务器（Top-level DNS Server）：管理各自域名下的权威域名服务器，比如
com 顶级域名服务器可以返回 apple.com 域名服务器的 IP 地址；

权威域名服务器（Authoritative DNS Server）：管理自己域名下主机的 IP 地址，比如apple.com 权威域名服务器可以返回 www.apple.com 的 IP 地址



###  HTTPS中间人攻击

 https 协议由 http + ssl 协议构成，具体的链接过程可参考 SSL 或 TLS 握手的概述

中间人攻击过程如下： 

1. 服务器向客户端发送公钥。 
2. 攻击者截获公钥，保留在自己手上。
3. 然后攻击者自己生成一个【伪造的】公钥，发给客户端。
4. 客户端收到伪造的公钥后，生成加密 hash 值发给服务器
5. 攻击者获得加密 hash 值，用自己的私钥解密获得真秘钥。 
6. 同时生成假的加密 hash 值，发给服务器。
7. 服务器用私钥解密获得假秘钥。
8. 服务器用加秘钥加密传输信息 

防范方法： 服务端在发送浏览器的公钥中加入 CA 证书，浏览器可以验证 CA 证书的有效性

## COOKIE

### Cookie的优缺点 

**优点：**极高的扩展性和可用性

1)  数据持久性。

2)  不需要任何服务器资源。 Cookie 存储在客户端并在发送后由服务器读取。

3)  可配置到期规则。 控制 cookie 的生命期，使之不会永远有效。偷盗者很可能拿到一个过期的 cookie

4)  简单性。 基于文本的轻量结构。

5)  通过良好的编程，控制保存在 cookie 中的 session 对象的大小。

6)  通过加密和安全传输技术（ SSL ），减少 cookie 被破解的可能性。

7)  只在 cookie 中存放不敏感数据，即使被盗也不会有重大损失。

缺点：

1\) Cookie 数量和长度的限制 。

数量：每个域的 cookie 总数有限。 a) IE6 或更低版本 多 20 个 cookie

b)  IE7 和之后的版本 后可以有 50 个 cookie

c)  Firefox 多 50 个 cookie

d)  chrome 和 Safari 没有做硬性限制

长度：每个 cookie 长度不超过 4KB （ 4096B ），否则会被截掉。

2)  潜在的安全风险 。 Cookie 可能被拦截、篡改。如果 cookie 被拦截，就有可能取得所有的 session 信息。

3)  用户配置为禁用 。有些用户禁用了浏览器或客户端设备接受 cookie 的能力，因此限制了这一功能。

4)  有些状态不可能保存在客户端 。例如，为了防止重复提交表单，我们需要在服务器端保存一个计数器。如果我们把这个计数器保存在客户端，那么它起不到任何作用。

### cookies ， sessionStorage 和 localStorage 的区别 

cookie 是网站为了标示用户身份而储存在用户本地终端上的数据（通常经过加密）

cookie数据始终在同源的http请求中携带（即使不需要），记会在浏览器和服务器间来回传递

（优化点）

sessionStorage 和 localStorage 不会自动把数据发给服务器，仅在本地保存存储大小：

cookie 数据大小不能超过4k

sessionStorage 和 localStorage虽然也有存储大小的限制，但比 cookie 大得多，可以达到5M或更大有期时间：

localStorage 存储持久数据，浏览器关闭后数据不丢失除非主动删除数据

sessionStorage 数据在当前浏览器窗口关闭后自动删除

cookie 设置的 cookie 过期时间之前一直有效，即使窗口或浏览器关闭

区别：

1.  Cookie

> 每个域名存储量比较小（各浏览器不同，大致 4K ）所有域名的存储量有限制（各浏览器不同，大致 4K ）有个数限制（各浏览器不同）会随请求发送到服务器

2.  LocalStorage 永久存储

> 单个域名存储量比较大（推荐 5MB ，各浏览器不同）总体数量无限制

3.  SessionStorage

> 只在 Session 内有效
>
> 存储量更大（推荐没有限制，但是实际上各浏览器也不同）

## cookie 和 token 都存放在 header 中，为什么不会 劫持 token？ 

1、攻击者通过 xss 拿到用户的 cookie 然后就可以伪造 cookie 了。 2、或者通过 csrf 在同个浏览器下面通过浏览器会自动带上 cookie 的特性 在通过 用户网站-攻击者网站-攻击者请求用户网站的方式 浏览器会自动带上 cookie 但是 token 1、不会被浏览器带上 问题 2 解决 2、token 是放在 jwt 里面下发给客户端的 而且不一定存储在哪里 不能通过 document.cookie 直接拿到，通过 jwt+ip 的方式 可以防止 被劫持 即使被劫持 也是无效的 jwt

### test

- Get和Post区别
- HTTP与HTTPS区别
- HTTP通信过程
- 游览器输入一个地址。到页面展示中间经历了哪些步骤？
- cookies机制和session机制的区别：
- HTTP请求报文与响应报文格式
- 一次完整的HTTP请求所经历的7个步骤
- HTTP优化方案
- 不同版本的HTTP区别
- HTTP优点缺点
- URI和URL的区别
- 如何判断是否为http
- HTTP 1.1引入分块传输编码提供了以下几点好处
- 长连接与短连接的区别，以及应用场景
- 常见web攻击
- 站内跳转和外部重定向有何区别
- HTTP的keep-alive是干什么的？
- 关于Http 2.0 你知道多少？
- 讲讲304缓存的原理
- HTTP与RPC异同
- 从传输协议来说

> RPC既可以基于TCP也可以基于HTTP协议，但是HTTP通常都是基于HTTP

- 从性能消耗来说

> RPC可以基于thrift实现高效二进制传输。HTTP大部分通过json实现，无论从字节大小还是序列化耗时都比t'hrift耗时

- 从负载均衡来说

> RPC基本上自带负载均衡策略，而HTTP需要配置Nginx实现。

## Vue



1. vue怎么实现对数组的监听，vue数组变异方法有哪些，是怎么实现的，以push为例，说说算法

   > 

2. vue全家桶各自的原理

   > 

3. 组件间的通讯

   > 

4. vue的生命周期

   > 

5. 如何构建一个vue项目

6. vue的基本原理

7. vue-router实现的原理

8. vue双向绑定

   > **Vue 的双向数据绑定，Model 如何改变 View，** **View 又是如何改变 Model 的** 
   >
   > 1、从 M 到 V 的映射（Data Binding），这样可以大量节省你人肉来 update View 的代码 
   >
   > 2、从 V 到 M 的事件监听（DOM Listeners），这样你的 Model 会随着 View 触发事件而改变 

9. 虚拟dom

10. data 为什么是函数 

    > 与JavaScript的作用域有关。为防止组件间的data相互修改

11. 父子组件如何通信 :prop 

12. 双向绑定和响应式数据原理

    > 双向绑定：v-model
    >
    > 响应式：v-bind

13. **Vue 的父组件和子组件生命周期钩子执行顺序是什么** 

    > 1. 父组建： beforeCreate -> created -> beforeMount 
    > 2. 子组件： -> beforeCreate -> created -> beforeMount -> mounted 
    > 3. 父组件： -> mounted
    > 4. 总结：从外到内，再从内到外 

    

14. 







## webpack





## react



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

- 要关联一个远程库，使用命令git remote add origin git@server-name:path/repo-name.git；

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

  

- 忽略某些文件时，需要编写.gitignore；

- .gitignore文件本身要放到版本库里，并且可以对.gitignore做版本管理！

- 

- 来自 <https://www.liaoxuefeng.com/wiki/896043488029600/900004590234208> 

- 

## 手写编程题

1. 防抖和节流★

2. 深拷贝★★★

3. 数组扁平化★★★

4. 单例模式★★

5. 数组去重★★★

6. 手写promise.all和promise.race★★

7. 模拟实现new ★

8. 实现call/apply/bind ★

9. 模拟Object.create()的实现

10. 千分位分隔符★

11. 实现三角形★★

12. 实现三栏布局/双栏布局★★★

13. flatten数组

14. 实现repeat函数，每隔一段时间执行一次函数，重复n次。

    ```javascript
    //每隔2s输出一次"helloworld"，共输出4次const 
    repeatFunc = repeat(console.log, 4, 2000);
    repeatFunc("helloworld");
    
    ANS:
    
    const repeatFunc = repeat(console.log, 4, 2000);
    repeatFunc("helloworld");
    function repeat(fn, n, time) {
    return function (args) {
    for (let i = 1; i <= n; i++) {
          setTimeout(fn, i * time, args)
        }
      }
    }
    ```

    

15. 编程题：将数组转成树形结构的对象

16. 实现一个正方形，拖拽窗口，正方形等比例缩放

17. 编程题：判断一个字符串是否完全由某个子串重复组成

18. Diff算法

19. 冒泡排序  快速排序

20. 给一段HTML，写出它的VDOM；写一个函数去解析这个VDOM，把元素添加到DOM上。

21. 一个div块，设置其为两个效果，一个为渐隐效果，一个为点击空白处显示和隐藏

22. ajax封装成promise

23. 写一个 vue 组件，实现类[百度](https://www.nowcoder.com/jump/super-jump/word?word=百度)的搜索框，可以出现自动的下拉列表，里面出现可能的和文字相关的信息（自动补全）

24. LeetCode 打家劫舍

25. 斐波那契第50项

    ```js
    function fibonacci(s){
                var prev = 0;
                var curr  =1;
                var ans = 0;
                if (s == 1)return prev;
                if (s == 2)return curr;
    
                for(var i =3;i<=s;i++){
                    ans = prev+curr;
                    prev = curr;
                    curr = ans;
                }
                return ans;
            }
            console.log(fibonacci(5))
    ```

    

26. 函数高频调用时只执行最后一次

    防抖函数

    https://blog.csdn.net/Kindergarten_Sir/article/details/109137418

27. 深拷贝

    https://www.w3cschool.cn/article/8b3a1e469cd340.html

28. CSS布局（水平竖直）

    ```css
    //水平
    .center {
        margin: auto;
        width: 50%;
        border: 3px solid green;
        padding: 10px;
    }
    //or
    .center{
    	text-alien:center
    }
    //竖直
    .center {
        padding: 70px 0;
    }
    ```

    https://www.runoob.com/css/css-align.html

29. 图片缩放居中

    ```css 
    img {
        display: block;
        margin: auto;
        width: 40%;
    }
    ```

    

30. 卷

    ```javascript
    题目一：
    请完成“空白处”代码，使得以下组件在选择时能够将合适的值打印出来
    class Counter extends React.Component {
    	select(val) {
    		console.log('you have select' + val);
    	}
    	render() {
    		return (<ul>
               { 
                   ['a','b','c'].map((item, index) => {
                       return <li onClick={___空白处___}>{item}</li>
                   })
               }
           </ul>)
    	}
    }
    
    
    题目二：
    请实现find函数，使下列的代码调用正确。
    约定：
    title数据类型为String
    userId为主键，数据类型为Number
    var data = [
    	{userId: 8, title: 'title1'},
    	{userId: 11, title: 'other'},
    	{userId: 15, title: null},
    	{userId: 19, title: 'title2'}
    ];
    
    var find = function(origin) {
    	//your code are here...
    }
    
    //查找data中，符合条件的数据，并进行排序
    var result = find(data).where({
    	"title": /\d$/
    }).orderBy('userId', 'desc');
    
    console.log(result); // [{ userId: 19, title: 'title2'}, { userId: 8, title: 'title1' }];
    
    
    
    
    题目三：
    下面是一个redux中间件，补充“空白处”代码，使得dispatch支持action为函数作为返回值
      export default function() {
        return ({ dispatch, getState }) => next => action => {
          if (___空白处___) {
            return ___空白处___;
          }
          return next(action);
        };
      };
    
    
    
    题目四：
    为 Function 扩展一个通用的方法 bindX，可以实现如下功能
      function add(num1, num2) {
          return this.value + num1 + num2;
      }
    
      var data = {
          value: 1
      };
    
      var addEx = add.bindX(data, 2);
    
      addEx(3);    // 6
    
    
    
    
    
    
    题目五：
    有一个数组，里面只存在 * 和 字母，比如 [‘*’, ‘d’, ‘c’, ‘*’, ‘e’, ‘*’, ‘a’, ‘*‘]。现在需要把这个数组中的所有星号移动到左边，所有的字母移动到右边，所有字母的顺序不能改变。
    var arr = ['*', 'd', 'c', '*', 'e', '*', 'a', '*'];
    
     function parse(arr){
    
     }
    
     console.log(parse(arr));
    
    ```

    https://www.nowcoder.com/discuss/454033?type=all&order=time&pos=&page=1&channel=-1&source_id=search_all_nctrack

31. （1）给定一个整数数组和一个目标值，找出数组中和为目标值的两个数。 [算法]()要求 o(n)
    (一个值只能用一次，匹配多个值，需要都返回 ，( [1，1，1，2，2，5，55] => [1,2] , [1,2] )

32. （2）给定两个版本号，比较两个版本号的大小。.号作为分割符使用，版本号中只有数和.号。  （0.1 < 1.1.1 < 1.2 < 13.37  ）
    例如：给定一个function输入两个参数 targetVersion , currentVersion，比较后返回 1， 0 ，-1 ( 大 ，等于 ，小于 )

33. （3）编写一个 getJsonp function(args , callback ), 其中 args 为参数， callback 为回调

34. 用reduce写一个map方法

35. new的过程

36. CSS3写一个环形进度条

37. 浏览器 缓存机制

38. BFC

39. 编程题：n维数组转换成1维数组，比如:[1,[2,3],[[4],[5,6]]]变成[1,2,3,4,5,6]

40. 手写数组拍平写了三个方法，不过面试官表示直接 return arr.flatten(Infinity) 是不可以的，因为本来就要去实现它。上一次写数组拍平有些时日了，以为自己已经了然于心，实则不然，最后写出来还是不太优雅，这里给大家分享一个优雅的： 

    [复制代码](#)

    ```
    Array.prototype.flatten = ``function``() {`` ``return` `this``.reduce((a, b) => {``  ``return` `a.concat(Array.isArray(b) ? b.flatten() : b);`` ``}, []);``}
    ```

41. 括号匹配

42. 数组的扁平化

    ```javascript
    var data =  [1, [2, [ [3, 4], 5], 6]];
    
        function flat(data, result) {
            var i, d, len;
            for (i = 0, len = data.length; i < len; ++i) {
                d = data[i];
                if (typeof d === 'number') {
                    result.push(d);
                } else {
                    flat(d, result);
                }
            }
        }
    
        var result = [];
        flat(data, result);
    
        console.log(result);
    ```

    

43. 斐波那契第50项

    ```js
    function fibonacci(s){
                var prev = 0;
                var curr  =1;
                var ans = 0;
                if (s == 1)return prev;
                if (s == 2)return curr;
    
                for(var i =3;i<=s;i++){
                    ans = prev+curr;
                    prev = curr;
                    curr = ans;
                }
                return ans;
            }
            console.log(fibonacci(5))
    ```

    

44. 函数高频调用时只执行最后一次

    防抖函数

    https://blog.csdn.net/Kindergarten_Sir/article/details/109137418

45. 深拷贝

    https://www.w3cschool.cn/article/8b3a1e469cd340.html

46. CSS布局（水平竖直）

    ```css
    //水平
    .center {
        margin: auto;
        width: 50%;
        border: 3px solid green;
        padding: 10px;
    }
    //or
    .center{
    	text-alien:center
    }
    //竖直
    .center {
        padding: 70px 0;
    }
    ```

    https://www.runoob.com/css/css-align.html

47. 图片缩放居中

    ```css 
    img {
        display: block;
        margin: auto;
        width: 40%;
    }
    ```

    

48. 卷

    ```javascript
    题目一：
    请完成“空白处”代码，使得以下组件在选择时能够将合适的值打印出来
    class Counter extends React.Component {
    	select(val) {
    		console.log('you have select' + val);
    	}
    	render() {
    		return (<ul>
               { 
                   ['a','b','c'].map((item, index) => {
                       return <li onClick={___空白处___}>{item}</li>
                   })
               }
           </ul>)
    	}
    }
    
    
    题目二：
    请实现find函数，使下列的代码调用正确。
    约定：
    title数据类型为String
    userId为主键，数据类型为Number
    var data = [
    	{userId: 8, title: 'title1'},
    	{userId: 11, title: 'other'},
    	{userId: 15, title: null},
    	{userId: 19, title: 'title2'}
    ];
    
    var find = function(origin) {
    	//your code are here...
    }
    
    //查找data中，符合条件的数据，并进行排序
    var result = find(data).where({
    	"title": /\d$/
    }).orderBy('userId', 'desc');
    
    console.log(result); // [{ userId: 19, title: 'title2'}, { userId: 8, title: 'title1' }];
    
    
    
    
    题目三：
    下面是一个redux中间件，补充“空白处”代码，使得dispatch支持action为函数作为返回值
      export default function() {
        return ({ dispatch, getState }) => next => action => {
          if (___空白处___) {
            return ___空白处___;
          }
          return next(action);
        };
      };
    
    
    
    题目四：
    为 Function 扩展一个通用的方法 bindX，可以实现如下功能
      function add(num1, num2) {
          return this.value + num1 + num2;
      }
    
      var data = {
          value: 1
      };
    
      var addEx = add.bindX(data, 2);
    
      addEx(3);    // 6
    
    
    
    
    
    
    题目五：
    有一个数组，里面只存在 * 和 字母，比如 [‘*’, ‘d’, ‘c’, ‘*’, ‘e’, ‘*’, ‘a’, ‘*‘]。现在需要把这个数组中的所有星号移动到左边，所有的字母移动到右边，所有字母的顺序不能改变。
    var arr = ['*', 'd', 'c', '*', 'e', '*', 'a', '*'];
    
     function parse(arr){
    
     }
    
     console.log(parse(arr));
    
    ```

    https://www.nowcoder.com/discuss/454033?type=all&order=time&pos=&page=1&channel=-1&source_id=search_all_nctrack

49. 手写代码：输入一个数字n，输出从1到n的所有排列，比如输入3，输出123、132、213、231、312、321

50. 字符串反转

    ```javascript
    var str="asdfghjkl";
    str = str.split('').reverse().join("");
    
    ```

51. 10进制转指定7进制字符（用额外的7个字符代替原先七进制的0123456）

    ```javascript
    var str = 17;
           str = str.toString(7).split("");
           var alaph = "QWERTYUIOP".split('');
            for (let i = 0; i < str.length; i++) {
                str[i] = alaph[i];
    
                
            }
            str = str.join("");
            console.log(str)
    ```

    

52. 节流函数和浏览器窗体大小变动结合，每250毫秒只显示一次窗口大小变动

    





## reviewLink

https://www.runoob.com/

[现代JavaScript教程](https://zh.javascript.info/)

[ES6入门文档](http://caibaojian.com/es6/)

[ECMAScript 6 入门-阮一峰](https://www.bookstack.cn/read/es6-3rd/sidebar.md)

[Vue.js](https://cn.vuejs.org/v2/guide/)

《JavaScript高级程序设计》

《你不知道的JavaScript》

《算法（第4版）》