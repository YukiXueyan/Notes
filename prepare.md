# menu

[TOC]



# HTML

## 浏览器页面有哪三层构成，分别是什么，作用是什么?

构成：结构层、表示层、行为层

分别是：HTML、CSS、JavaScript

作用：HTML实现页面结构，CSS完成页面的表现与风格，JavaScript实现一些客户端的功能与业务。

## HTML5的优点与缺点？

优点：

a.  网络标准统一、HTML5本身是由W3C推荐出来的。

b.  多设备、跨平台 

c、即时更新。

d、提高可用性和改进用户的友好体验； 

e、有几个新的标签，这将有助于开发人员定义重要的内容；

f、可以给站点带来更多的多媒体元素(视频和音频)；

g、可以很好的替代Flash和Silverlight；

h、涉及到网站的抓取和索引的时候，对于SEO很友好； 

i、被大量应用于移动应用程序和游戏。

缺点：

a.  安全：像之前Firefox4的web socket和透明代理的实现存在严重的安全问题，同时web storage、web socket 这样的功能很容易被黑客利用，来盗取用户的信息和资料。

b.  完善性：许多特性各浏览器的支持程度也不一样。

c.  技术门槛：HTML5简化开发者工作的同时代表了有许多新的属性和API需要开发者学习，像web worker、web socket、web storage 等新特性，后台甚至浏览器原理的知识，机遇的同时也是巨大的挑战

d.  性能：某些平台上的引擎问题导致HTML5性能低下。

e.  **浏览器兼容性：最大缺点**，IE9以下浏览器几乎全军覆没。

## Doctype作用? 严格模式与混杂模式如何区分？它们有何意义?

ans1

1. 声明位于文档中的最前面，处于标签之前。告知浏览器的解析器，用什么文档类型规范来解析这个文档。
2. 严格模式的排版和JS 运作模式是以该浏览器支持的最高标准运行。
3. 在混杂模式中，页面以宽松的向后兼容的方式显示。模拟老式浏览器的行为以防止站点无法工作。
4. DOCTYPE不存在或格式不正确会导致文档以混杂模式呈现。

回答2：

doctype声明指出阅读程序应该用什么规则集来解释文档中的标记。在Web文档的情况下，"阅读程序"通常是浏览器或者校验器这样的一个程序，"规则"则是W3C所发布的一个文档类型定义（DTD）中包含的规则。

1. 声明位于文档中的最前面的位置，处于标签之前。此标签可告知浏览器文档使用哪种 HTML 或 XHTML 规范。该标签可声明三种 DTD 类型，分别表示严格版本、过渡版本以及基于框架的HTML 文档。
2. 所谓的标准模式是指，浏览器按 W3C 标准解析执行代码；怪异模式则是使用浏览器自己的方式解析执行代码，因为不同浏览器解析执行的方式不一样，所以我们称之为怪异模式。 严格模式是浏览器根据web标准去解析页面，是一种要求严格的DTD，不允许使用任何表现层的语法，如。严格模式的排版和JS 运作模式是以该浏览器支持的最高标准运行混杂模式则是一种向后兼容的解析方法，说的透明点就是可以实现IE5.5以下版本浏览器的渲染模式。
3. 浏览器解析时到底使用标准模式还是怪异模式，与你网页中的 DTD 声明直接相关， DTD 声明定义了标准文档的类型（标准模式解析）文档类型，会使浏览器使用相应的方式加载网页并显示，忽略 DTD 声明 ,将使网页进入怪异模式。

## HTML5有哪些新特性、移除了哪些元素？

 

Html5新增了27个元素，废弃了16个元素，根据现有的标准规范，把 HTML5 的元素按优先级定义为结构性属性、级块性元素、行内语义性元素和交互性元素

4大类。

结构性元素主要负责web上下文结构的定义：

section：在 web 页面应用中，该元素也可以用于区域的章节描述。 header：页面主体上的头部， header 元素往往在一对 body 元素中。

footer：页面的底部（页脚），通常会标出网站的相关信息。

nav：专门用于菜单导航、链接导航的元素，是 navigator 的缩写。 article：用于表现一篇文章的主体内容，一般为文字集中显示的区域。

级块性元素主要完成web页面区域的划分，确保内容的有效分割。

aside：用于表达注记、贴士、侧栏、摘要、插入的引用等作为补充主体的内容。 figure：是对多个元素进行组合并展示的元素，通常与 ficaption 联合使用。

code：表示一段代码块。

dialog：用于表达人与人之间的对话，该元素包含 dt 和 dd 这两个组合元素， dt 用于表示说话者，而 dd 用来表示说话内容。

行内语义性元素主要完成web页面具体内容的引用和描述，是丰富内容展示的基础。

meter：表示特定范围内的数值，可用于工资、数量、百分比等。

time：表示时间值。

progress：用来表示进度条，可通过对其 max 、 min 、 step 等属性进行控制，完成对进度的表示和监事。

video：视频元素，用于支持和实现视频文件的直接播放，支持缓冲预载和多种视频媒体格式。

audio：音频元素，用于支持和实现音频文件的直接播放，支持缓冲预载和多种音频媒体格式。

交互性元素主要用于功能性的内容表达，会有一定的内容和数据的关联，是各种事件的基础。

details：用来表示一段具体的内容，但是内容默认可能不显示，通过某种手段

（如单击）与 legend 交互才会显示出来。

datagrid：用来控制客户端数据与显示，可以由动态脚本及时更新。 menu：主要用于交互菜单（曾被废弃又被重新启用的元素）。

command：用来处理命令按钮。

- 新特性
  - 新元素
    - canvas
    - article 、footer、header、nav、section 表单控件 ，calendar 、 date 、 time 、 email 、 url 、 search 
  - 新属性
  - 完全支持 CSS3
  - Video 和 Audio
  - 2D/3D 制图
  - 本地存储
    - 本地离线存储localStorage长期存储数据，浏览器关闭后数据不丢失 sessionStorage的数据在浏览器关闭后自动删除
  - 本地 SQL 数据
  - Web 应用
  - 新技术
    -  webworker 、 websocket 、 Geolocation
- 移除元素
  - 纯表现的元素： basefont 、 big 、 center 、 font 、 s 、 strike 、 tt 、 u 
  - 对可用性产生负面影响的元素： frame 、 frameset 、 noframes
  - `<acronym>`
  - `<applet>`
  - `<basefont>`
  - `<big>`
  - `<center>`
  - `<dir>`
  - `<font>`
  - `<frame>`
  - `<frameset>`
  - `<noframes>`
  - `<strike>`

## 你做的网页在哪些浏览器测试过,这些浏览器的内核分别是什么?

- IE: trident内核
- Firefox：gecko内核
- Safari: webkit内核
- Opera: 以前是presto内核，Opera现已改用Google Chrome的Blink内核 
- Chrome:Blink(基于webkit，Google与Opera Software共同开发 )

## 每个HTML文件里开头都有个很重要的东西，Doctype，知道这是干什么的吗？

声明位于文档中的最前面的位置，处于标签之前。此标签可告知浏览器文档使用哪种HTML或XHTML规范。（重点：告诉浏览器按照何种规范解析页面）

## 说说你对HTML5认识?（是什么,为什么）

是什么：

HTML5指的是包括HTML、CSS和JavaScript在内的一套技术组合。它希望能够

减少网页浏览器对于需要插件的丰富性网络应用服务（Plug-in-Based Rich InternetApplication，RIA），例如：AdobeFlash 、MicrosoftSilverlight 与Oracle JavaFX的需求，并且提供更多能有效加强网络应用的标准集。HTML5 是HTML最新版本，2014年10月由万维网联盟（W3C）完成标准制定。目标是替换1999年所制定的HTML4.01和XHTML1.0标准，以期能在互联网应用迅速发展的时候，使网络标准达到匹配当代的网络需求。

为什么：

HTML4陈旧不能满足日益发展的互联网需要，特别是移动互联网。为了增强浏览器功能Flash被广泛使用，但安全与稳定堪忧，不适合在移动端使用（耗电、触摸、不开放）。

HTML5增强了浏览器的原生功能，符合HTML5规范的浏览器功能将更加强大，减少了Web应用对插件的依赖，让用户体验更好，让开发更加方便，另外W3C从推出HTML4.0到5.0之间共经历了17年，HTML的变化很小，这并不符合一个好产品的演进规则。

## 对WEB标准以及W3C的理解与认识?

标签闭合、标签小写、不乱嵌套、提高搜索机器人搜索几率、使用外链css和 js脚本、结构行为表现的分离、文件下载与页面速度更快、内容能被更多的用户所访问、内容能被更广泛的设备所访问、更少的代码和组件，容易维护、改版方便，不需要变动页面内容、提供打印版本而不需要复制内容、提高网站易用性。

## HTML5行内元素有哪些,块级元素有哪些, 空元素有哪些?

(1)行内元素 

- a - 锚点
- abbr - 缩写
- acronym - 首字
- b - 粗体 ( 不推荐 )
- bdo - bidi override
- big - 大字体 
- br - 换行
- cite - 引用
- code - 计算机代码 ( 在引用源码的时候需要 ) 
- dfn - 定义字段 
- em - 强调 
- font - 字体设定 ( 不推荐 ) 
- i - 斜体
- img - 图片 
- input - 输入框
- kbd - 定义键盘文本 
- label - 表格标签
- q - 短引用 s - 中划线 ( 不推荐 )
- samp - 定义范例计算机代码
- select - 项目选择 small - 小字体文本 span - 常用内联容器，定义文本内区块
- strike - 中划线 strong - 粗体强调 sub - 下标 sup - 上标
- textarea - 多行文本输入框
- tt - 电传文本 u - 下划线
- var - 定义变量

(2)块元素 (block element)

- address - 地址
- blockquote - 块引用
- center - 居中对齐块
- dir - 目录列表
- div - 常用块级容易，也是 css layout 的主要标签
- dl - 定义列表
- fieldset - form控制组
- form - 交互表单
- h1 - 大标题
- h2 - 副标题
- h3 - 3级标题
- h4 - 4级标题
- h5 - 5级标题
- h6 - 6级标题
- hr - 水平分隔线
- isindex - input prompt
- menu - 菜单列表
- noframes - frames可选内容，（对于不支持 frame 的浏览器显示此区块内容

- noscript - ）可选脚本内容（对于不支持 script 的浏览器显示此内容）
- ol - 排序表单
- p - 段落
- pre - 格式化文本 * table - 表格

- ul - 非排序列表

(3)可变元素

可变元素为根据上下文语境决定该元素为块元素或者内联元素。

- applet - java applet
- button - 按钮
- del - 删除文本
- iframe - inline frame
- ins - 插入的文本
- map - 图片区块 (map)
- object - object对象
- script - 客户端脚本

(4)空元素 ( 在 HTML[1] 元素中，没有内容的 HTML 元素被称为空元

素 )

`<br/>` //换行

`<hr>` //分隔线

`<input>` //文本框等

`<link> <meta>`

## 什么是WebGL,它有什么优点?

 

WebGL（全写 WebGraphicsLibrary ）是一种3D绘图标准，这种绘图技术标准允许把JavaScript和OpenGL ES 2.0结合在一起，通过增加OpenGL ES 2.0的一个JavaScript绑定，WebGL可以为HTML5 Canvas提供硬件3D加速渲染，这样Web开发人员就可以借助系统显卡来在浏览器里更流畅地展示3D场景和模型了，还能创建复杂的导航和数据视觉化。显然，WebGL技术标准免去了开发网页专用渲染插件的麻烦，可被用于创建具有复杂3D结构的网站页面，甚至可以用来设计3D网页游戏等等。

WebGL完美地解决了现有的Web交互式三维动画的两个问题：

第一，它通过HTML脚本本身实现Web交互式三维动画的制作，无需任何浏览器插件支持 ;

第二，它利用底层的图形硬件加速功能进行的图形渲染，是通过统一的、标准的、跨平台的OpenGL接口实现的。

通俗说WebGL中canvas绘图中的3D版本。因为原生的WebGL很复杂，我们经常会使用一些三方的库，如three.js等，这些库多数用于HTML5游戏开发。

## 请你描述一下 cookies，sessionStorage 和 localStorage 的区别?

 

sessionStorage 和 localStorage 是 HTML5 Web Storage API 提供的，可以方便的在 web 请求之间保存数据。有了本地数据，就可以避免数据在浏览器和服务器间不必要地来回传递。sessionStorage、 localStorage 、 cookie 都是在浏览器端存储的数据，其中 sessionStorage 的概念很特别，引入了一个"浏览器窗口"的概念。sessionStorage 是在同源的同窗口（或 tab ）中，始终存在的数据。也就是说只要这个浏览器窗口没有关闭，即使刷新页面或进入同源另一页面，数据仍然存在。关闭窗口后， sessionStorage 即被销毁。同时"独立" 打开的不同窗口，即使是同一页面， sessionStorage 对象也是不同的cookies 会发送到服务器端。其余两个不会。

Microsoft指出InternetExplorer8增加cookie限制为每个域名50个，但IE7 似乎也允许每个域名50个cookie。Firefox每个域名cookie限制为50个。Opera 每个域名cookie限制为30个。 Firefox和Safari允许cookie多达4097个字节，包括名（name）、值（value）和等号。Opera许cookie多达4096个字节，包括：名（name）、值（value）和等号。Internet Explorer允许cookie多达4095个字节，包括：名（name）、值（value）和等号。

区别：

1. Cookie

   每个域名存储量比较小（各浏览器不同，大致 4K ）所有域名的存储量有限制（各浏览器不同，大致 4K ）有个数限制（各浏览器不同）会随请求发送到服务器

2. LocalStorage 永久存储

   单个域名存储量比较大（推荐 5MB ，各浏览器不同）总体数量无限制

3. SessionStorage

   只在 Session 内有效.存储量更大（推荐没有限制，但是实际上各浏览器也不同）

## 说说你对HTML语义化的理解?



(1)什么是 HTML 语义化？

基本上都是围绕着几个主要的标签，像标题（ H1~H6 ）、列表（ li ）、强调（ strong em ）等等 > 根据内容的结构化（内容语义化），选择合适的标签（代码语义化）便于开发者阅读和写出更优雅的代码的同时让浏览器的爬虫和机器很好地解析。

(2)为什么要语义化？

为了在没有CSS的情况下，页面也能呈现出很好地内容结构、代码结构 : 为了裸奔时好看；

用户体验：例如title、 alt 用于解释名词或解释图片信息、 label 标签的活用；

有利于SEO：和搜索引擎建立良好沟通，有助于爬虫抓取更多的有效信息：爬虫依赖于标签来确定上下文和各个关键字的权重；

方便其他设备解析（如屏幕阅读器、盲人阅读器、移动设备）以意义的方式来渲染网页；

便于团队开发和维护，语义化更具可读性，是下一步网页的重要动向，遵循W3C 标准的团队都遵循这个标准，可以减少差异化。

(3) 语义化标签

```html
<header></header> <footer></footer>

<nav></nav>

<section></section>

<article></article>
```
SM:用来在页面中表示一套结构完整且独立的内容部分

`<aslde></aside>`

SM:主题的附属信息(用途很广，主要就是一个附属内容)，如果article里面为

一篇文章的话，那么文章的作者以及信息内容就是这篇文章的附属内容了

SM:媒体元素，比如一些视频，图片啊等等

`<datalist></datalist>`

SM:选项列表，与 input 元素配合使用，来定义 input 可能的值

SM:用于描述文档或者文档某个部分的细节，默认属性为open~

ps:配合summary一起使用 13.link和\@import的区别?



XML/HTML代码

`<link rel='stylesheet' rev='stylesheet' href='CSS文件 ' type='text/css' media='all' />`

XML/HTML代码
```
\@import url('CSS文件 ');

</style>
```
两者都是外部引用CSS的方式，但是存在一定的区别：

区别1： link 是 XHTML 标签，除了加载 CSS 外，还可以定义 RSS 等其他事务；` \@import` 属于 CSS 范畴，只能加载 CSS 。

区别2： link 引用 CSS 时，在页面载入时同时加载； \@import 需要页面网页完全载入以后加载。

区别3： link 是 XHTML 标签，无兼容问题； \@import 是在 CSS2.1 提出的，低版本的浏览器不支持。

区别4： link 支持使用 Javascript 控制 DOM 去改变样式；而 \@import 不支持。

## 说说你对SVG理解?

SVG可缩放矢量图形（ScalableVectorGraphics）**是基于可扩展标记语言（XML），用于描述二维矢量图形的一种图形格式。**SVG是W3C('World Wide Web ConSortium'即'国际互联网标准织')在2000年8月制定的一种新的二维矢量图形格式，也是规范中的网络矢量图形标准。SVG严格遵从XML语法，并用文本格式的描述性语言来描述图像内容，因此是一种和图像分辨率无关的矢量图形格式。SVG于2003年1月14日成为W3C推荐标准。

特点：

(1)任意放缩

​	用户可以任意缩放图像显示，而不会破坏图像的清晰度、细节等。

(2)文本独立

​	SVG图像中的文字独立于图像，文字保留可编辑和可搜寻的状态。也不会再有字体的限制，用户系统即使没有安装某一字体，也会看到和他们制作时完全相同的画面。

(3)较小文件

​	总体来讲，SVG文件比那些GIF和JPEG格式的文件要小很多，因而下载也很快。

(4)超强显示效果

​	SVG图像在屏幕上总是边缘清晰，它的清晰度适合任何屏幕分辨率和打印分辨率。

(5)超级颜色控制

​	SVG图像提供一个1600万种颜色的调色板，支持ICC颜色描述文件标准、RGB、线X填充、渐变和蒙版。

(6)交互X和智能化。

​	SVG面临的主要问题一个是如何和已经占有重要市场份额的矢量图形格式Flash竞争的问题，另一个问题就是SVG的本地运行环境下的厂家支持程度。

浏览器支持：

Internet Explorer9，火狐，谷歌Chrome，Opera和Safari都支持SVG。 IE8和早期版本都需要一个插件-如Adobe SVG浏览器，这是免费提供的。

## HTML全局属性(global attribute)有哪些?



MDN: html global attribute或者W3C HTML global-attributes

accesskey:设置快捷键，提供快速访问元素如aaa在windows下的firefox中按 alt + shift + a可激活元素;

class:为元素设置类标识，多个类名用空格分开，CSS和javascript可通过class 属性获取元素;

contenteditable: 指定元素内容是否可编辑;

contextmenu: 自定义鼠标右键弹出菜单内容 data-*: 为元素增加自定义属性; dir: 设置元素文本方向;

draggable: 设置元素是否可拖拽;

dropzone: 设置元素拖放类型： copy, move, link hidden: 表示一个元素是否与文档。样式上会导致元素不显示，但是不能用这个属性实现样式效果 id: 元素id，文档内唯一;

lang: 元素内容的的语言 spellcheck: 是否启动拼写和语法检查 style: 行内css样式

tabindex: 设置元素可以获得焦点，通过tab可以导航;

title: 元素相关的建议信息; translate: 元素和子孙节点内容是否需要本地化;

## 说说超链接target属性的取值和作用？


target这个属性指定所链接的页面在**浏览器窗口中的打开方式。**

它的参数值主要有：

a.  _blank：在新浏览器窗口中打开链接文件；

b.  _parent ：将链接的文件载入含有该链接框架的父框架集或父窗口中。如果含有该链接的框架不是嵌套的，则在浏览器全屏窗口中载入链接的文件；

c.  _self：在同一框架或窗口中打开所链接的文档。此参数为默认值，通常不用指定。但是我不太理解； d、_top：在当前的整个浏览器窗口中打开所链接的文档，因而会删除所有框架；

## `data-`属性的作用是什么？

\`data-\`为H5新增的为前端开发者提供自定义的属性，这些属性集可以通过对象的\`dataset\`属性获取，不支持该属性的浏览器可以通过\`getAttribute\`方法获取，需要注意的是：\`data-\`之后的以连字符分割的多个单词组成的属性，获取的时候使用驼峰风格。所有主流浏览器都支持 data-* 属性。

即：当没有合适的属性和元素时，自定义的data属性是能够存储页面或App的私有的自定义数据。

## 介绍一下你对浏览器内核的理解？

主要分成两部分：渲染引擎(layout engineer或 Rendering Engine)和JS引擎。

渲染引擎：负责取得网页的内容（HTML、XML、图像等等）、整理讯息（例如加入CSS等），以及计算网页的显示方式，然后会输出至显示器或打印机。浏览器的内核的不同对于网页的语法解释会有不同，所以渲染的效果也不相同。所有网页浏览器、电子邮件客户端以及其它需要编辑、显示网络内容的应用程序都需要内核。

JS引擎：解析和执行javascript来实现网页的动态效果。

最开始渲染引擎和JS引擎并没有区分的很明确，后来JS引擎越来越独立，内核就倾向于只指渲染引擎。

## 常见的浏览器内核有哪些？

Trident内核：IE,MaxThon,TT,TheWorld,360, 搜狗浏览器等。[又称MSHTML]

Gecko内核：Netscape6及以上版本，FF,MozillaSuite/SeaMonkey等

Presto内核：Opera7及以上。[Opera内核原为：Presto，现为：Blink;]

Webkit内核：Safari,Chrome等。 [ Chrome的：Blink（WebKit的分支）]

## iframe有那些缺点？

(1)iframe会阻塞主页面的Onload事件；

(2)搜索引擎的检索程序无法解读这种页面，不利于SEO;

(3)iframe和主页面共享连接池，而浏览器对相同域的连接有限制，所以会影响页面的并行加载。使用iframe之前需要考虑这两个缺点。如果需要使用iframe，最好是通过 javascript动态给iframe添加 src 属性值，这样可以绕开以上两个问题。 

## Label的作用是什么，是怎么用的？

label标签来定义表单控制间的关系 , 当用户选择该标签时，浏览器会自动将焦点转到和标签相关的表单控件上。

```html
<label for='Name'>Number:</label>

<input type=" text " name='Name' id='Name'/> <label>Date:<input type='text' name='B'/></label>
```



注意:label的for属性值要与后面对应的input标签id属性值相同

```html
<label for='Name'>Number:</label>

<input type=" text " name='Name' id='Name'/>
```

## 如何实现浏览器内多个标签页之间的通信?

WebSocket、SharedWorker；

也可以调用localstorage、cookies等本地存储方式；

localstorage另一个浏览上下文里被添加、修改或删除时，它都会触发一个事件，我们通过监听事件，控制它的值来进行页面信息通信；

注意quirks：Safari在无痕模式下设置localstorge值时会抛出QuotaExceededError的异常；

## 如何在页面上实现一个圆形的可点击区域？ 

a、map+area或者svg 

b、border-radius

c、纯js实现 需要求一个点在不在圆上简单算法、获取鼠标坐标等等

## title与h3的区别、b与strong的区别、i与em的区别？

(1)title属性没有明确意义只表示是个标题，H1则表示层次明确的标题，对页面信息的抓取也有很大的影响；

(2)strong是标明重点内容，有语气加强的含义，使用阅读设备阅读网时：

`<strong>`会重读，而`<B>`是展示强调内容。

(3)i内容展示为斜体，em表示强调的文本；

Physical Style Elements -- 自然样式标签 b, i, u, s, pre

Semantic Style Elements -- 语义样式标签 strong, em, ins, del, code

应该准确使用语义样式标签,但不能滥用,如果不能确定时首选使用自然样式标签。

## 实现不使用 border 画出1px高的线，在不同浏览器的标准模式与怪异模式下都能保持一致的效果？

> `<div style="width:100%;height:1px;background-color:black"></div>`

## HTML5标签的作用?(用途)



a.  使Web页面的内容更加有序和规范；

b.  使搜索引擎更加容易按照HTML5规则识别出有效的内容；

 c、使Web页面更接近于一种数据字段和表；

## 简述一下src与href的区别？



src用于替换当前元素，href用于在当前文档和引用资源之间确立联系。

src是source的缩写，指向外部资源的位置，指向的内容将会嵌入到文档中当前标签所在位置；

在请求src资源时会将其指向的资源下载并应用到文档内，例如js脚本，img 图片和frame等元素。

当浏览器解析到该元素时，会暂停其他资源的下载和处理，直到将该资源加载、编译、执行完毕，图片和框架等元素也如此，类似于将所指向资源嵌入当前标签内。这也是为什么将js脚本放在底部而不是头部。

href是Hypertext Reference的缩写，指向网络资源所在位置，建立和当前元素（锚点）或当前文档（链接）之间的链接，如果我们在文档中添加`<link href='common.css' rel='stylesheet'/>`

那么浏览器会识别该文档为css文件，就会并行下载资源并且不会停止对当前文档的处理。这也是为什么建议使用link方式来加载css，而不是使用`\@import` 方式。

## 谈谈你对canvas的理解？

canvas是HTML5中新增一个HTML5标签与操作canvas的javascriptAPI，它可以实现在网页中完成动态的2D与3D图像技术。标记和 SVG以及 VML 之间的一个重要的不同是，有一个基于 JavaScript 的绘图 API，而 SVG 和 VML 使用一个 XML 文档来描述绘图。SVG 绘图很容易编辑与生成，但功能明显要弱一些。 canvas可以完成动画、游戏、图表、图像处理等原来需要Flash完成的一些功能。

## WebSocket与消息推送？

B/S架构的系统多使用HTTP协议，

HTTP协议的特点：

1)无状态协议

2)用于通过 Internet 发送请求消息和响应消息

3)使用端口接收和发送消息，默认为80端口 底层通信还是使用Socket完成。

HTTP协议决定了服务器与客户端之间的连接方式，无法直接实现消息推送（F5 已坏）,一些变相的解决办法：双向通信与消息推送

轮询：客户端定时向服务器发送Ajax请求，服务器接到请求后马上返回响应信息并关闭连接。

优点：后端程序编写比较容易。

缺点：请求中有大半是无用，浪费带宽和服务器资源。

实例：适于小型应用。长轮询：客户端向服务器发送Ajax请求，服务器接到请求后 hold 住连接，直到有新消息才返回响应信息并关闭连接，客户端处理完响应信息后再向服务器发送新的请求。

优点：在无消息的情况下不会频繁的请求，耗费资小。

缺点：服务器hold连接会消耗资源，返回数据顺序无保证，难于管理维护。Comet 异步的ashx，

实例：WebQQ、Hi网页版、Facebook IM。

长连接：在页面里嵌入一个隐蔵iframe，将这个隐蔵iframe的src属性设为对一个长连接的请求或是采用xhr请求，服务器端就能源源不断地往客户端输入数据。

优点：消息即时到达，不发无用请求；管理起来也相对便。

缺点：服务器维护一个长连接会增加开销。

实例：Gmail聊天

FlashSocket：在页面中内嵌入一个使用了Socket类的Flash程序JavaScript 通过调用此Flash程序提供的Socket接口与服务器端的Socket接口进行通信，

JavaScript在收到服务器端传送的信息后控制页面的显示。

优点：实现真正的即时通信，而不是伪即时。

缺点：客户端必须安装Flash插件；非HTTP协议，无法自动穿越防火墙。

实例：网络互动游戏。

Websocket:

WebSocket是HTML5开始提供的一种浏览器与服务器间进行全双工通讯的网络技

术。依靠这种技术可以实现客户端和服务器端的长连接，双向实时通信。

特点:

a、事件驱动 

b、异步

c、使用ws或者wss协议的客户端socket 

d、能够实现真正意义上的推送功能缺点：少部分浏览器不支持，浏览器支持的程度与方式有区别。

## img的title和alt有什么区别？

Alt 用于图片无法加载时显示Title为该属性提供信息，通常当鼠标滑动到元素上的时候显示。

## 表单的基本组成部分有哪些，表单的主要用途是什么？

组成：表单标签、表单域、表单按钮

a.  表单标签：这里面包含了处理表单数据所用CGI程序的URL,以及数据提交到服务器的方法。

b.  表单域：包含了文本框、密码框、隐藏域、多行文本框、复选框、单选框、下拉选择框、和文件上传框等。

c.  表单按钮：包括提交按钮，复位按钮和一般按钮；用于将数据传送到服务器上的CGI脚本或者取消输入，还可以用表单按钮来控制其他定义了处理脚本的处理工作。

主要用途：表单在网页中主要负责数据采集的功能，和向服务器传送数据。

## 表单提交中Get和Post方式的区别？



(1)、get是从服务器上获取数据，post是向服务器传送数据。

(2)、get是把参数数据队列加到提交表单的ACTION属性所指的URL中，值和表单内各个字段一一对应，在URL中可以看到。post是通过HTTP post机制，将表单内各个字段与其内容放置在HTML HEADER内一起传送到ACTION属性所指的 URL地址,用户看不到这个过程。

(3)、对于get方式，服务器端用Request.QueryString获取变量的值，对于post

方式，服务器端用Request.Form获取提交的数据。

(4)、get传送的数据量较小，不能大于2KB。post传送的数据量较大，一般被默认为不受限制。但理论上，IIS4中最大量为80KB，IIS5中为100KB 。

(5)、get安全性低，post安全性较高。

## HTML5 有哪些新增的表单元素?

HTML5新增了很多表单元素让开发者构建更优秀的Web应用程序，主要有：

datalist keygen output



## HTML5 标准提供了哪些新的 API？

HTML5提供的应用程序API主要有：

· Media API

· Text Track API

· Application Cache API

· User Interaction

· Data Transfer API

· Command API

· Constraint Validation API

· History API

## HTML5 存储类型有什么区别？



HTML5能够本地存储数据，在之前都是使用cookies使用的。HTML5提供了下面两种本地存储方案：

· localStorage 用于持久化的本地存储，数据永远不会过期，关闭浏览器也不会丢失。

·sessionStorage 同一个会话中的页面才能访问并且当会话结束后数据也随之销毁。因此sessionStorage不是一种持久化的本地存储，仅仅是会话级别的存

储

## HTML5 应用程序缓存和浏览器缓存有什么区别？

应用程序缓存是 HTML5的重要特性之一，提供了离线使用的功能，让应用程序

可以获取本地的网站内容，例如 HTML 、CSS 、图片以及JavaScript。这个特性可以提高网站性能，它的实现借助于manifest文件，如下：

```html
<!doctype html>
<html manifest="example.appcache">

.....

</html>
```

与传统浏览器缓存相比，它不强制用户访问的网站内容被缓存。

##  HTML5 Canvas 元素有什么用？

 Canvas元素用于在网页上绘制图形，该元素标签强大之处在于可以直接在HTML 上进行图形操作

`<canvas id="canvas1" width="300" height="100">   </canvas>` 

## 除了 audio 和 video，HTML5 还有哪些媒体标签？

 HTML5对于多媒体提供了强有力的支持，除了audio和video标签外，还支持以下标签：

```html
<source>对于定义多个数据源很有用。

<source src="jamshed.mp4" type="video/mp4">

<source src="jamshed.ogg" type= "video/ogg">

</video>

<track>标签为诸如video元素之类的媒介规定外部文本轨道。用于规定字幕文

件或其他包含文本的文件，当媒介播放时，这些文件是可见的。

<source src="jamshed.mp4" type="video/mp4">

<source src="jamshed.ogg" type= "video/ogg">

<track kind="subtitles" label="English" src=

"jamshed_en.vtt" srclang="en" default></track>

<track kind="subtitles" label="Arabic" src=

"jamshed_ar.vtt" srclang="ar"></track>

</video>
```



## HTML5 中如何嵌入视频？

和音频类似，HTML5支持MP4、WebM和Ogg格式的视频，

简单示例：

```html
<source src="jamshed.mp4" type="video/mp4">

Your browser does' nt support video embedding feature.

</video>
```

## HTML5 中如何嵌入音频？

HTML5支持MP3、Wav和Ogg格式的音频，下面是在网页中嵌入音频的简单示例：

```html
<source src="jamshed.mp3" type="audio/mpeg">

Your browser does' nt support audio embedding feature.

</audio>
```

## 新的 HTML5 文档类型和字符集是？

HTML5文档类型很简单：

`<!doctype html>`


HTML5使用UTF-8编码示例：

`<meta charset="UTF-8">`

## viewport的content属性作用 

\<meta name=\"viewport\" content=\"\" /\>

width viewport的宽度\[device-width \| pixel\_value\]width如果直接设置pixel\_value数值，大部分的安卓手机不支持，但是ios支持；

height -- viewport 的高度 （范围从 223 到 10,000 ）

user-scalable \[yes \| no\]是否允许缩放

initial-scale \[数值\] 初始化比例（范围从 \> 0 到 10）

minimum-scale \[数值\] 允许缩放的最小比例

maximum-scale \[数值\] 允许缩放的最大比例

target-densitydpi 值有以下（一般推荐设置中等响度密度或者低像素密度，后者设置具体的值 dpi\_value，另外webkit内核已不准备再支持此属性）

\-- dpi\_value 一般是70-400//没英寸像素点的个数

\-- device-dpi设备默认像素密度

\-- high-dpi 高像素密度

\-- medium-dpi 中等像素密度

\-- low-dpi 低像素密度附带问题：怎样处理 移动端 1px 被 渲染成 2px 问题?

局部处理：

mate 标签中的 viewport 属性 ， initial-scale 设置为 1 rem 按照设计稿标准走，外加利用transfrome 的 scale(0.5)缩小一倍即可；

全局处理：

mate标签中的 viewport 属性 ， initial-scale 设置为 0.5 rem 按照设计稿标准走即可

## meta 相关 

> \<!DOCTYPE html\> \<!\--H5标准声明，使用 HTML5 doctype，不区分大小写\--\>
>
> \<head lang="en"\> \<!\--标准的 lang 属性写法\--\>
>
> \<meta charset='utf-8ʹ\> \<!\--声明文档使用的字符编码\--\>
>
> \<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1″/\> \<!\--优先使用指定浏览器使用特定的文档模式\--\>
>
> \<meta name="description" content="不超过150个字符"/\> \<!\--页面描述\--\>
>
> \<meta name="keywords" content=""/\> \<!\-- 页面关键词\--\>
>
> \<meta name="author" content="name, email\@gmail.com"/\> \<!\--网页作者\--\>
>
> \<meta name="robots" content="index,follow"/\> \<!\--搜索引擎抓取\--\>
>
> \<meta name="viewport" content="initial-scale=1, maximum-scale=3, minimum-sc
>
> \<meta name="apple-mobile-web-app-title" content="标题"\> \<!\--iOS 设备 begin\--\>
>
> \<meta name="apple-mobile-web-app-capable" content="yes"/\> \<!\--添加到主屏后的标是否启用 WebApp 全屏模式，删除苹果默认的工具栏和菜单栏\--\>
>
> \<meta name="apple-mobile-web-app-status-bar-style" content="black"/\>
>
> \<meta name="renderer" content="webkit"\> \<!\-- 启用360浏览器的极速模式(webkit)\--\>
>
> \<meta http-equiv="X-UA-Compatible" content="IE=edge"\> \<!\--避免IE使用兼容模式\--\>
>
> \<meta http-equiv="Cache-Control" content="no-siteapp" /\> \<!\--不让百度转码\--\> \<meta name="HandheldFriendly" content="true"\> \<!\--针对手持设备优化，主要是针对一些老的不识别viewport的浏览器\--\>
>
> \<meta name="MobileOptimized" content="320″\> \<!\--微软的老式浏览器\--\>
>
> \<meta name="screen-orientation" content="portrait"\> \<!\--uc强制竖屏\--\>
>
> \<meta name="x5-orientation" content="portrait"\> \<!\--QQ强制竖屏\--\>
>
> \<meta name="full-screen" content="yes"\> \<!\--UC强制全屏\--\>
>
> \<meta name="x5-fullscreen" content="true"\> \<!\--QQ强制全屏\--\>
>
> \<meta name="browsermode" content="application"\> \<!\--UC应用模式\--\>
>
> \<meta name="x5-page-mode" content="app"\> \<!\-- QQ应用模式\--\>
>
> \<meta name="msapplication-tap-highlight" content="no"\> \<!\--windows phone 设置页面不缓存\--\>
>
> \<meta http-equiv="pragma" content="no-cache"\>
>
> \<meta http-equiv="cache-control" content="no-cache"\>
>
> \<meta http-equiv="expires" content="0″\>

## 说一下HTML5 drag api

 

dragstart：事件主体是被拖放元素，在开始拖放被拖放元素时触发

darg：事件主体是被拖放元素，在正在拖放被拖放元素时触发。 

dragenter：事件主体是目标元素，在被拖放元素进入某元素时触发。 

dragover：事件主体是目标元素，在被拖放在某元素内移动时触发。 

dragleave：事件主体是目标元素，在被拖放元素移出目标元素是触发。 

drop：事件主体是目标元素，在目标元素完全接受被拖放元素时触发。

dragend：事件主体是被拖放元素，在整个拖放操作结束时触发



## 对HTML语义化标签的理解

HTML5语义化标签是指正确的标签包含了正确的内容，结构良好，便于阅读，比如nav表示导航条，类似的还有article、header、footer等等标签。

## iframe是什么？有什么缺点？

定义：iframe元素会创建包含另一个文档的内联框架

提示：可以将提示文字放在`<iframe></iframe>`之间，来提示某些不支持iframe 的浏览器缺点：

a.会阻塞主页面的onload事件

b.搜索引擎无法解读这种页面，不利于SEO

c.iframe和主页面共享连接池，而浏览器对相同区域有限制所以会影响性能。

## Doctype作用?严格模式与混杂模式如何区分？它们有何意义?

\<!DOCTYPE\> 声明位于文档中的最前面的位置，处于 \<html\> 标签之前。此标签可告知浏览器文档使用哪种 HTML 或 XHTML 规范。（重点：告诉浏览器按照何种规范解析页面）

1.  严格模式的排版和 JS 运作模式是 以该浏览器支持的最高标准运行。

2.  、在混杂模式中，页面以宽松的向后兼容的方式显示。模拟老式浏览器的行为以防止站点无法工作。

3.  、DOCTYPE不存在或格式不正确会导致文档以混杂模式呈现。

# CSS

## 解释一下CSS的盒子模型？

a、标准的css盒子模型：宽度=内容的宽度+边框的宽度+加上内边框的宽度 

b、网页设计中常听的属性名：内容(content)、填充(padding)、边框(border)、边界(margin)， CSS盒子模式都具备这些属性。

c、这些属性我们可以把它转移到我们日常生活中的盒子（箱子）上来理解，日常生活中所见的盒子也就是能装东西的一种箱子，也具有这些属性，所以叫它盒子模式。CSS盒子模型就是在网页设计中经常用到的CSS技术所使用的一种思维模型。

标准的盒模型：width = content

IE盒模型：width = content+padding+border

## 请你说说CSS选择器的类型有哪些，并举几个例子说明其用法？

类型：基础的选择器、组合选择器、属性选择器、伪类、伪元素

- 选择符：相邻（+）、后代（ 空格）、子类（<）

1. id 选择器（ # myid） 
2. 类选择器（.myclassname） 

3. 标签选择器（div, h1, p） 

4. 相邻选择器（h1 + p） 

5. 子选择器（ul < li） 

6. 后代选择器（li a） 

7. 通配符选择器（ * ） 

8. 属性选择器（a[rel = "external"]） 

9. 伪类选择器（a: hover, li: nth - child） 

- **可继承： font-size font-family color, UL LI DL DD DT; **

- **不可继承 ：border padding margin width height ;** 

优先级就近原则，样式定义最近者为准; * 载入样式以最后载入的定位为准; 

优先级为: !important > id > class > tag 

important 比 内联优先级高 

权重：从0开始，一个行内样式+1000，一个id选择器+100，一个属性选择器、class或者伪类+10，一个

元素选择器，或者伪元素+1，通配符+0

- CSS3 新增伪类举例： 

p:first-of-type选择属于其父元素的首个 元素的每个 元素。

p:last-of-type选择属于其父元素的 后 元素的每个元素。

p:only-of-type选择属于其父元素唯一的 元素的每个 元素。

p:only-child选择属于其父元素的唯一子元素的每个 元素。

p:nth-child(2)选择属于其父元素的第二个子元素的每个 元素。

:enabled已启用的表单元素。

:disabled已禁用的表单元素。

:checked单选框或复选框被选中。

::before在元素之前添加内容。

::after在元素之后添加内容,也可以用来做清除浮动。

::first-line添加一行特殊样式到首行。

::first-letter添加一个特殊的样式到文本的首字母。伪类语法一个：，它是为了弥补css常规类选择器的不足

伪元素语法两个：，它是凭空创建的一个虚拟容器生成的元素

## 请你说说CSS有什么特殊性?（优先级、计算特殊值）

优先级：

(1)、同类型，同级别的样式后者先于前者

(2))、ID > 类样式 > 标签 > *

(3)、内联>ID选择器>伪类>属性选择器>类选择器>标签选择器>通用选择器(*)> 继承的样式

(4)、具体 > 泛化的，特殊性即css优先级

(5)、近的 > 远的 (内嵌样式 > 内部样式表 > 外联样式表)

  内嵌样式：内嵌在元素中，`<span style="color:red">span</span>`

  内部样式表：在页面中的样式，写在`<style></style>`中的样式外联样式表：单独存在一个css文件中，通过link引入或import导入的样式

(6)、!important 权重最高，比 inline style 还要高

**计算特殊性值**

important > 内嵌 > ID > 类 > 标签 | 伪类 | 属性选择 > 元素|伪元素 > 继承 > 通配符

权重、特殊性计算法：

CSS样式选择器分为4个等级，a、b、c、d

(1)、如果样式是行内样式（通过Style=""定义），那么a=1，1,0,0,0

(2)、b为ID选择器的总数 0,1,0,0

(3)、c为属性选择器，伪类选择器和class类选择器的数量。0,0,1,0

(4)、d为标签、伪元素选择器的数量 0,0,0,1

(5)、!important 权重最高，比 inline style 还要高

比如结果为：1093比1100，按位比较，从左到右，只要一位高于则立即胜出，否则继续比较。

| -选择器             | -特殊性(a,b,c,d) |
| ------------------- | ---------------- |
| style=""            | 1000             |
| #wrapper #content{} | 0200             |
| #content .data{}    | 0110             |
| div#content{}       | 0101             |
| #content p{}        | 0101             |
| #content{}          | 0100             |
| p.comment .data{}   | 0021             |
| div.comment p{}     | 0012             |
| .comment p{}        | 0011             |
| p.comment{}         | 0011             |
| .comment{}          | 0010             |
| div p{}             | 0002             |
| p{}                 | 0001             |

## CSS3有哪些新特性？

边框、圆角、背景、渐变、文本效果、字体、2D/3D转换、过渡、动画、多列、弹性盒子、多媒体查询

- 边框、圆角

  - border-radius
  - box-shadow
  - border-image

- 背景

  - background-image  添加背景图片。
  - background-size  指定背景图像的大小。
  - background-origin  指定了背景图像的位置区域。值有  content-box, padding-box,和 border-box
  - background-clip背景剪裁属性是从指定位置开始绘制。

- 渐变

  - **线性渐变（Linear Gradients）- 向下/向上/向左/向右/对角方向**
  - **径向渐变（Radial Gradients）- 由它们的中心定义**

- 文本效果

  - text-shadow适用于文本阴影。
  - box-shadow适用于盒子阴影
  - text-overflow  指定应向用户如何显示溢出内容
  - word-wrap自动换行属性允许您强制文本换行 - 即使这意味着分裂它中间的一个字
  - word-break  单词拆分换行

- 字体

- 2D/3D转换

  - 、缩放、转动、拉长或拉伸
  - translate()移动
  - rotate()旋转
  - scale()该元素增加或减少的大小，取决于宽度（X轴）和高度（Y轴）的参数
  - skew()
    - 包含两个参数值，分别表示X轴和Y轴倾斜的角度，如果第二个参数为空，则默认为0，参数为负表示向相反方向倾斜。
    - skewX(`<angle>`);表示只在X轴(水平方向)倾斜。
    - skewY(`<angle>`);表示只在Y轴(垂直方向)倾斜。
  - matrix()   matrix 方法有六个参数，包含旋转，缩放，移动（平移）和倾斜功能。
  - rotateX()方法，围绕其在一个给定度数X轴旋转的元素。
  - rotateY()方法，围绕其在一个给定度数Y轴旋转的元素。

- 过渡

  - | [transition](https://www.runoob.com/cssref/css3-pr-transition.html) | 简写属性，用于在一个属性中设置四个过渡属性。 |
    | ------------------------------------------------------------ | -------------------------------------------- |
    | [transition-property](https://www.runoob.com/cssref/css3-pr-transition-property.html) | 规定应用过渡的 CSS 属性的名称。              |
    | [transition-duration](https://www.runoob.com/cssref/css3-pr-transition-duration.html) | 定义过渡效果花费的时间。默认是 0。           |
    | [transition-timing-function](https://www.runoob.com/cssref/css3-pr-transition-timing-function.html) | 规定过渡效果的时间曲线。默认是 "ease"。      |
    | [transition-delay](https://www.runoob.com/cssref/css3-pr-transition-delay.html) | 规定过渡效果何时开始。默认是 0。             |

- 动画

  - @keyframes 规则内指定一个 CSS 样式和动画将逐步从目前的样式更改为新的样式。

- 多列

  - `column-count`指定了需要分割的列数。
  - `column-gap`指定了列与列间的间隙。
  - `column-rule-style`指定了列与列间的边框样式
  - `column-rule-width`指定了两列的边框厚度
  - `column-rule-color`指定了两列的边框颜色
  - `column-rule`
  - `column-span`指定元素跨越多少列
  - `column-width`指定列的宽度

- 弹性盒子

  - 弹性盒子由弹性容器(Flex container)和弹性子元素(Flex item)组成。

  - 弹性容器通过设置 display 属性的值为 flex 或 inline-flex将其定义为弹性容器。

  - 弹性容器内包含了一个或多个弹性子元素。

  - 弹性盒子只定义了弹性子元素如何在弹性容器内布局。

  - 修改排列方式：  direction

    - flex-direction 属性指定了弹性子元素在父容器中的位置
      - flex-direction: row | row-reverse | column | column-reverse

    - justify-content 属性  把弹性项沿着弹性容器的主轴线（main axis）对齐

      - flex-start

      - flex-end

      - center

      - space-between

      - space-around

      - flex-start：弹性项目向行头紧挨着填充。这个是默认值。第一个弹性项的main-start外边距边线被放置在该行的main-start边线，而后续弹性项依次平齐摆放。flex-end：弹性项目向行尾紧挨着填充。第一个弹性项的main-end外边距边线被放置在该行的main-end边线，而后续弹性项依次平齐摆放。center：弹性项目居中紧挨着填充。（如果剩余的自由空间是负的，则弹性项目将在两个方向上同时溢出）。space-between：弹性项目平均分布在该行上。如果剩余空间为负或者只有一个弹性项，则该值等同于flex-start。否则，第1个弹性项的外边距和行的main-start边线对齐，而最后1个弹性项的外边距和行的main-end边线对齐，然后剩余的弹性项分布在该行上，相邻项目的间隔相等。space-around：弹性项目平均分布在该行上，两边留有一半的间隔空间。如果剩余空间为负或者只有一个弹性项，则该值等同于center。否则，弹性项目沿该行分布，且彼此间隔相等（比如是20px），同时首尾两边和弹性容器之间留有一半的间隔（1/2*20px=10px）。

    - align-items 设置或检索弹性盒子元素在侧轴（纵轴）方向上的对齐方式

      - flex-start

      - flex-end

      - center

      - baseline

      - stretch

    - flex-wrap 属性用于指定弹性盒子的子元素换行方式。

      - nowrap

      - wrap

      - wrap-reverse

    - align-content 属性用于修改 flex-wrap 属性的行为,设置各个行的对齐

      - flex-start

      - flex-end

      - center

      - space-between

      - space-around

      - stretch

    - align-self 属性用于设置弹性元素自身在侧轴（纵轴）方向上的对齐方式。

    - flex 如何分配空间

- 多媒体查询

- 响应式设计

  - viewport

    - viewport 是用户网页的可视区域。

    - 手机浏览器是把页面放在一个虚拟的"窗口"（viewport）中，通常这个虚拟的"窗口"（viewport）比屏幕宽，这样就不用把每个网页挤到很小的窗口中（这样会破坏没有针对手机浏览器优化的网页的布局），用户可以通过平移和缩放来看网页的不同部分。

  - 网格视图

    - 按列布局

    - 创建

      - 确保所有的 HTML 元素都有 box-sizing 属性且设置为 border-box。

      - 确保边距和边框包含在元素的宽度和高度间。

      - 12列的网格布局  每列的百分比: 100% / 12 列 = 8.33%。

        - 每列中指定 class， class="col-" 用于定义每列有几个 span 

        - 所有的列向左浮动

        - 每一行使用 &lt;div&gt; 包裹。所有列数加起来应为 12：

        - 列中行为左浮动，并添加清除浮动

- 网格Grid布局

  - 将容器分为行和列，产生单元格。

  - 使用Grid布局的区域——container；内部元素：item

  - 水平区域是行row；垂直区域是列

  - display：grid

    - 指定容器采用网格布局

      - display：grid

      - display：inline-grid

  - grid-template-columns

    - 定义列宽

    - grid-template-columns: 33.33% 33.33% 33.33%;  三列

    - grid-template-columns属性对于网页布局非常有用。两栏式布局只需要一行代码。
      - grid-template-columns: 70% 30%;

  - grid-template-rows

    - 定义行高

    - grid-template-rows: 33.33% 33.33% 33.33%;

  - repeat（）

    - 重复

    - 重复次数和所要重复的值

    - grid-template-columns: repeat(3, 33.33%);

  - auto-fill 关键字

    - 如果希望每一行（或每一列）容纳尽可能多的单元格，这时可以使用auto-fill关键字表示自动填充。

  - fr 关键字

    - 表示比例关系

    - 如果两列的宽度分别为1fr和2fr，就表示后者是前者的两倍。

    - grid-template-columns: 150px 1fr 2fr;
      - 表示，第一列的宽度为150像素，第二列的宽度是第三列的一半。

  - minmax()

    - minmax()函数产生一个长度范围，表示长度就在这个范围之中。它接受两个参数，分别为最小值和最大值。

  - auto 关键字

    - auto关键字表示由浏览器自己决定长度。

  - 行间距与列间距

    - grid-row-gap属性设置行与行的间隔（行间距），grid-column-gap属性设置列与列的间隔（列间距）。

    - grid-gap属性是grid-column-gap和grid-row-gap的合并简写形式
      -  grid-gap: 20px 20px;

  - grid-template-areas 属性

    - 网格布局允许指定"区域"（area），一个区域由单个或多个单元格组成。grid-template-areas属性用于定义区域。

  - grid-auto-flow 属性

    - grid-auto-flow: row;先行后列

    - grid-auto-flow: column;先列后行

    - row dense

    - column dense

  - justify-items 属性

    - start | end | center | stretch;
      - start：对齐单元格的起始边缘。end：对齐单元格的结束边缘。center：单元格内部居中。stretch：拉伸，占满单元格的整个宽度（默认值）。

  - align-items属性

    - start | end | center | stretch;

  - justify-content属性是整个内容区域在容器里面的水平位置（左中右），

  - align-content属性是整个内容区域的垂直位置（上中下）

  - 项目属性

    - grid-column-start 属性，grid-column-end 属性，grid-row-start 属性，grid-row-end 属性

    - grid-column 属性，grid-row 属性

    - grid-area

      - grid-area属性指定项目放在哪一个区域。
        - （grid-template-areas属性定义区域名）

      - grid-area属性还可用作grid-row-start、grid-column-start、grid-row-end、grid-column-end的合并简写形式，直接指定项目的位置。

    - justify-self 属性，align-self 属性，place-self 属性

## 要动态改变层中内容可以使用的方法？

innerHTML，innerText

## 常见浏览器兼容性问题与解决方案？ 

- 浏览器兼容问题一：不同浏览器的标签默认的外补丁和内补丁不同

> 问题症状：随便写几个标签，不加样式控制的情况下，各自的margin 和padding 差异较大。
>
> 碰到频率:100%
>
> 解决方案：CSS里 *{margin:0;padding:0;}
>
> 备注：这个是最常见的也是最易解决的一个浏览器兼容性问题，几乎所有的CSS 文件开头都会用通配符*来设置各个标签的内外补丁是0。

- 浏览器兼容问题二：块属性标签float后，又有横行的margin情况下，在IE6显示margin比设置的大

> 问题症状:常见症状是IE6中后面的一块被顶到下一行
>
> 碰到频率：90%（稍微复杂点的页面都会碰到，float布局最常见的浏览器兼容问题）
>
> 解决方案：在float的标签样式控制中加入 display:inline;将其转化为行内属性
>
> 备注：我们最常用的就是div+CSS布局了，而div就是一个典型的块属性标签，横向布局的时候我们通常都是用div float实现的，横向的间距设置如果用 margin实现，这就是一个必然会碰到的兼容性问题。

- 浏览器兼容问题三：设置较小高度标签（一般小于10px），在IE6，IE7，遨游中高度超出自己设置高度

> 问题症状：IE6、7和遨游里这个标签的高度不受控制，超出自己设置的高度碰到频率：60%
>
> 解决方案：给超出高度的标签设置overflow:hidden;或者设置行高line-height 小于你设置的高度。
>
> 备注：这种情况一般出现在我们设置小圆角背景的标签里。出现这个问题的原因是IE8之前的浏览器都会给标签一个最小默认的行高的高度。即使你的标签是空的，这个标签的高度还是会达到默认的行高。

- 浏览器兼容问题四：行内属性标签，设置display:block后采用float布局，又有横行的margin的情况，IE6间距bug

> 问题症状：IE6里的间距比超过设置的间距碰到几率：20%
>
> 解决方案 ： 在display:block;后面加入display:inline;display:table;
>
> 备注：行内属性标签，为了设置宽高，我们需要设置display:block;(除了input 标签比较特殊)。在用float布局并有横向的margin后，在IE6下，他就具有了块属性float后的横向margin的bug。不过因为它本身就是行内属性标签，所以我们再加上display:inline的话，它的高宽就不可设了。这时候我们还需要在display:inline后面加入display:talbe。

- 浏览器兼容问题五：图片默认有间距

> 问题症状：几个img标签放在一起的时候，有些浏览器会有默认的间距，加了问题一中提到的通配符也不起作用。
>
> 碰到几率：20%
>
> 解决方案：使用float属性为img布局
>
> 备注：因为img标签是行内属性标签，所以只要不超出容器宽度，img标签都会排在一行里，但是部分浏览器的img标签之间会有个间距。去掉这个间距使用 float是正道。（我的一个学生使用负margin，虽然能解决，但负margin本身就是容易引起浏览器兼容问题的用法，所以我禁止他们使用）

- 浏览器兼容问题六：标签最低高度设置min-height不兼容

> 问题症状：因为min-height本身就是一个不兼容的CSS属性，所以设置 min-height时不能很好的被各个浏览器兼容碰到几率：5%
>
> 解决方案：如果我们要设置一个标签的最小高度200px，需要进行的设置为：
>
> {min-height:200px; height:auto !important; height:200px; overflow:visible;}
>
> 备注：在B/S系统前端开时，有很多情况下我们又这种需求。当内容小于一个值（如300px）时。容器的高度为300px；当内容高度大于这个值时，容器高度被撑高，而不是出现滚动条。这时候我们就会面临这个兼容性问题。
>
> (7)浏览器兼容问题七：透明度的兼容CSS设置
>
> 一般在ie中用的是filter:alpha(opacity=0);这个属性来设置div或者是块级元素的透明度，而在firefox中，一般就是直接使用opacity:0,对于兼容的，一般的做法就是在书写css样式的将2个都写上就行，就能实现兼容

## 列出display的值并说明他们的作用？

display： none | inline | block | list-item| inline-block | table | inline-table | table-caption | table-cell | table-row | table-row-group | table-column | table-column-group | table-footer-group | table-header-group | run-in | box | inline-box | flexbox | inline-flexbox | flex | inline-flex

默认值：inline

- none： 隐藏对象。与visibility属性的hidden值不同，其不为被隐藏的对象保留其物理空间

- inline： 指定对象为内联元素。 block： 指定对象为块元素。 list-item： 指定对象为列表项目。

- inline-block： 指定对象为内联块元素。（CSS2） table： 指定对象作为块元素级的表格。类同于html标签<table>（CSS2） inline-table： 指定对象作为内联元素级的表格。类同于html标签`<table>`（CSS2） table-caption：指定对象作为表格标题。类同于html标签`<caption>`（CSS2） table-cell： 指定对象作为表格单元格。类同于html标签`<td>`（CSS2） table-row： 指定对象作为表格行。类同于html标签`<tr>`（CSS2） table-row-group：指定对象作为表格行组。类同于html标签`<tbody>`（CSS2） table-column： 指定对象作为表格列。类同于html标签`<col>`（CSS2） table-column-group： 指定对象作为表格列组显示。类同于html标签`<colgroup>`（CSS2）

- table-header-group： 指定对象作为表格标题组。类同于html标签`<thead>`（CSS2） table-footer-group： 指定对象作为表格脚注组。类同于html标签`<tfoot>` （CSS2）

- run-in： 根据上下文决定对象是内联对象还是块级对象。（CSS3） box： 将对象作为弹性伸缩盒显示。（伸缩盒最老版本）（CSS3）

- inline-box：将对象作为内联块级弹性伸缩盒显示。（伸缩盒最老版本）（CSS3） 
- flexbox： 将对象作为弹性伸缩盒显示。（伸缩盒过渡版本）（CSS3）

- inline-flexbox： 将对象作为内联块级弹性伸缩盒显示。（伸缩盒过渡版本）（CSS3）

- flex： 将对象作为弹性伸缩盒显示。（伸缩盒最新版本）（CSS3） 
- inline-flex：将对象作为内联块级弹性伸缩盒显示。（伸缩盒最新版本）（CSS3）

## 如何居中div, 如何居中一个浮动元素? 

(1) 非浮动元素居中：可以设置 margin:0 auto 令其居中, 定位 ,父级元素 text-align:center等等

(2) 浮动元素居中:

方法一:设置当前div的宽度，然后设置margin-left:50%;position:relative; left:-250px;其中的left是宽度的一半。

方法二:父元素和子元素同时左浮动，然后父元素相对左移动50%，再然后子元素相对左移动-50%。

方法三:position定位等等。

## CSS中 link 和@import 的区别是？

1. link属于HTML标签，而\@import是CSS提供的;
2. 页面被加载的时，link会同时被加载，而\@import引用的CSS会等到页面被加载完再加载; 
3. import只在IE5以上才能识别，而link是HTML标签，无兼容问题;
4. link方式的样式的权重 高于\@import的权重.

## 请列举几种清除浮动的方法(至少两种)?

1. 父级div定义 height

   原理：父级div手动定义height，就解决了父级div无法自动获取到高度的问题。

   优点：简单、代码少、容易掌握

   缺点：只适合高度固定的布局，要给出精确的高度，如果高度和父级div不一样时，会产生问题

   建议：不推荐使用，只建议高度固定的布局时使用

2. 结尾处加空div标签 clear:both

   原理：添加一个空div，利用css提高的clear:both清除浮动，让父级div能自动获取到高度

   优点：简单、代码少、浏览器支持好、不容易出现怪问题

   缺点：不少初学者不理解原理；如果页面浮动布局多，就要增加很多空div，让人感觉很不好

   建议：不推荐使用，但此方法是以前主要使用的一种清除浮动方法

3. 父级div定义 伪类:after 和 zoom

   原理：IE8以上和非IE浏览器才支持:after，原理和方法2有点类似，zoom(IE 转有属性)可解决ie6,ie7浮动问题

   优点：浏览器支持好、不容易出现怪问题（目前：大型网站都有使用，如：腾迅，网易，新浪等等）

   缺点：代码多、不少初学者不理解原理，要两句代码结合使用才能让主流浏览器都支持。

   建议：推荐使用，建议定义公共类，以减少CSS代码。

4. 父级div定义 overflow:hidden

   原理：必须定义width或zoom:1，同时不能定义height，使用overflow:hidden 时，浏览器会自动检查浮动区域的高度优点：简单、代码少、浏览器支持好

   缺点：不能和position配合使用，因为超出的尺寸的会被隐藏。

   建议：只推荐没有使用position或对overflow:hidden理解比较深的朋友使用。

5. 父级div定义 overflow:auto

   原理：必须定义width或zoom:1，同时不能定义height，使用overflow:auto 时，浏览器会自动检查浮动区域的高度优点：简单、代码少、浏览器支持好

   缺点：内部宽高超过父级div时，会出现滚动条。

   建议：不推荐使用，如果你需要出现滚动条或者确保你的代码不会出现滚动条就使用吧。

## **CSS** 怎么画一个大小为父元素宽度一半的正方形？

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .outer {
            width: 400px;
            height: 600px;
            background: red;
        }

        .inner {
            width: 50%;
            padding-bottom: 50%;
            background: blue;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner"></div>
    </div>
</body>

</html>
```



## CSS实现自适应正方形、等宽高比矩形 

双重嵌套，外层 relative，内层 absolute padding 撑高

如果只是要相对于 body 而言的话，还可以使用 vw 和 vh 伪元素设置 margin-top: 100%撑高

**双重嵌套，外层 relative，内层 absolute**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .outer {
            padding-top: 50%;
            height: 0;
            background: #ccc;
            width: 50%;
            position: relative;
        }

        .inner {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            background: blue;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner">hello</div>
    </div>
</body>

</html>
```



**padding 撑高画正方形**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .outer {
            width: 400px;
            height: 600px;
            background: blue;
        }

        .inner {
            width: 100%;
            height: 0;
            padding-bottom: 100%;
            background: red;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner"></div>
    </div>
</body>

</html>
```

**相对于视口 VW VH**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .inner {
            width: 1vw;
            height: 1vw;
            background: blue;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner"></div>
    </div>
</body>

</html>
```

**伪元素设置 margin-top**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .inner {
            width: 100px;
            overflow: hidden;
        }

        .inner::after {
            content: "";
            margin-top: 100%;
            display: block;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner"></div>
    </div>
</body>

</html>
```



## 实现两栏布局的方式 

### 左float，右边自适应（margin-left）

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    div{
      height: 100px;
    }
    .left{
      float: left;
      width:100px;
      background-color:aqua
    }
    .right{
      /* margin-left: 100px; */
      background-color:aquamarine
    }
  </style>
</head>
<body>
  <div class="outer">
    <div class="left"></div>
    <div class="right"></div>
  </div>
</body>
</html>
```

### 右边固定，左边自适应（右边：float：right，左边margin-right）

```css
div{
    height: 100px;
}
.left{
    width: 300px; 
    float: right; 
    background: yellow;
}
.right{
    margin-right: 100px;
    background-color:aquamarine
}
```

### bfc+float

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document</title>
  <style>
    div {
      height: 500px;
    }

    .aside {
      width: 300px;
      float: left;
      background: yellow;
    }

    .main {
      overflow: hidden;
      background: aqua;
    }
  </style>
</head>

<body>
  <div class="aside"></div>
  <div class="main"></div>
</body>

</html>
```



###  float + 负margin

```html
<head>
  <style>
    .left {
      width: 100%;
      float: left;
      background: #f00;
      margin-right: -200px;
    }

    .right {
      float: left;
      width: 200px;
      background: #0f0;
    }
  </style>
</head>
<body>
<div class="left">
  <p>hello</p>
</div>
<div class="right">
  <p>world</p>
</div>
</body>
```



### flex 两栏布局

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    div{
      height:100%;
    }
    .main{
      display:flex;
    }
    .left{
      flex: 0 0 200px;
      background-color:chocolate
    }
    .right{
      flex: 1 1;
      background-color:aliceblue
    }
  </style>
</head>
<body>
  <div class="main">
    <div class="left">hi</div>
    <div class="right">yuki</div>
  </div>
</body>
</html>
```

## 实现三列布局的方式 

### position + margin-left + margin-right

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document</title>
  <style>
    div {
      height: 500px;
    }

    .box {
      position: relative;
    }

    .left {
      position: absolute;
      left: 0;
      top: 0;
      width: 200px;
      background: green;
    }

    .right {
      position: absolute;
      right: 0;
      top: 0;
      width: 200px;
      background: red;
    }

    .middle {
      margin-left: 200px;
      margin-right: 200px;
      background: black;
    }
  </style>
</head>

<body>
  <div class="box">
    <div class="left"></div>
    <div class="middle"></div>
    <div class="right"></div>
  </div>
</body>

</html
```

### 通过 float + margin

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document</title>
  <style>
    div {
      height: 500px;
    }

    .left {
      float: left;
      width: 200px;
      height: 200px;
      background: green;
    }

    .right {
      float: right;
      width: 200px;
      height: 200px;
      background: red;
    }

    .middle {
      margin-left: 210px;
      margin-right: 210px;
      background: black;
      height: 200px;
    }
  </style>
</head>

<body>
  <div class="box">
    <div class="left"></div>
    <div class="right"></div>
    <div class="middle"></div>
  </div>
</body>

</html>
```

### 两列定宽一列自适应：

1、使用float+margin：

给div设置float：left，left的div添加属性margin-right：left和center的间隔px,right的div添加属性margin-left：left和center的宽度之和加上间隔

2、使用float+overflow：

给div设置float：left，再给right的div设置overflow:hidden。这样子两个盒子浮动，另一个盒子触发bfc达到自适应

3、使用position：

父级div设置position：relative，三个子级div设置position：absolute，这个要计算好盒子的宽度和间隔去设置位置，兼容性比较好，

4、使用table实现：

父级div设置display：table，设置border-spacing：10px//设置间距，取值随意,子级div设置display:table-cell，这种方法兼容性好，适用于高度宽度未知的情况，但是margin失效，设计间隔比较麻烦，

5、flex实现：

parent的div设置display：flex；left和center的div设置margin-right；然后right 的div设置flex：1；这样子right自适应，但是flex的兼容性不好

6、grid实现：

parent的div设置display：grid，设置grid-template-columns属性，固定第一列第二列宽度，第三列auto，

对于两侧定宽中间自适应的布局，对于这种布局需要把center放在前面，可以采用双飞翼布局：圣杯布局，来实现，也可以使用上述方法中的grid，table，flex，position实现

### 圣杯布局

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Document</title>
  <style>
    .container {
      padding: 0 300px 0 200px;
      border: 1px solid black;
    }

    .content {
      float: left;
      width: 100%;
      background: #f00;
    }

    .left {
      width: 200px;
      background: #0f0;
      float: left;
      margin-left: -100%;
      position: relative;
      left: -200px;
    }

    .right {
      width: 300px;
      background: #00f;
      float: left;
      margin-left: -300px;
      position: relative;
      right: -300px;
    }
  </style>
</head>

<body>
  <div class="container">
    <div class="content">中间内容</div>
    <div class="left">左侧区域</div>
    <div class="right">右侧区域</div>
  </div>
</body>

</html>

```

### flex布局

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        html,
        body {
            height: 100%;
        }

        div {
            height: 100%;
        }

        .container {
            display: flex;
        }

        .content {
            flex: 1 1;
            order: 2;
            background: #f00;
        }

        .left {
            flex: 0 0 200px;
            order: 1;
            background: #0f0;
        }

        .right {
            flex: 0 0 300px;
            order: 3;
            background: #00f;
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="content">hello world</div>
        <div class="left">你好</div>
        <div class="right">我好</div>
    </div>
</body>

</html>
```

## 三栏布局的实现方式

三列布局又分为两种，两列定宽一列自适应，以及两侧定宽中间自适应两列定宽一列自适应：

- 使用float+margin：给div设置float：left，left的div添加属性margin-right：left和center 的间隔px,right的div添加属性margin-left：left和center的宽度之和加上间隔

- 使用float+overflow：给div设置float：left，再给right的div设置overflow:hidden。这样子两个盒子浮动，另一个盒子触发bfc达到自适应

- 使用position：父级div设置position：relative，三个子级div设置position：absolute，这个要计算好盒子的宽度和间隔去设置位置，兼容性比较好。

- 使用table实现：
  - 父级div设置display：table，设置border-spacing：10px//设置间距，取值随意,子级div设置display:table-cell，这种方法兼容性好，适用于高度宽度未知的情况，但是margin失效，设计间隔比较麻烦，

- flex实现：
  - parent的div设置display：flex；left和center的div设置margin-right；然后right 的div设置flex：1；这样子right自适应，但是flex的兼容性不好

- grid实现：
  - parent的div设置display：grid，设置grid-template-columns属性，固定第一列第二列宽度，第三列auto，对于两侧定宽中间自适应的布局，对于这种布局需要把center放在前面，可以采用双飞翼布局：圣杯布局，来实现，也可以使用上述方法中的grid，table， flex，position实现



## 水平居中

- `div + margin: auto;`
- `margin:0 auto`
- `span + text-align`
- 使用 flex-box 布局，指定 justify-content 属性为center
- display 设置为 tabel-ceil



## 垂直居中

- 使用 position 然后 left/top 和 margin 的方式垂直居中（已知宽高和未知宽高）

- 使用 position + margin

- 使用 display: table-cell;



## 水平垂直居中

- 已知宽高

  - 父元素用`position:relative`
  - 子元素 `position: absolute`，`left: 50%; top: 50%; margin: -150px 0 0 -100px;`

  ```html
  <!DOCTYPE html> <html lang="en"> <head> <meta charset="UTF-8" /> <meta name="viewport" content="width=device-width, initial-scale=1.0" /> <title>Document</title> <style>
  .outer { position: relative; width: 400px; height: 600px; background: blue; }
      
      .inner { position: absolute; width: 200px; height: 300px; background: red; left: 50%; top: 50%; margin: -150px 0 0 -100px; } </style> </head> <body> <div class="outer"> <div class="inner"></div> </div> </body> </html>
  ```

  

- 未知宽高

  - 父元素`position: relative; `
  - 子元素`left: 50%; top: 50%; transform: translate(-50%, -50%)`

- 图片和其他元素使用 display: table-cell; 进行垂直居中

### 外层元素用position：relative+内层元素用position:absolute+left:50%，top:50%,margin-left:-width/2,margin-top:-height/2

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .outer {
            position: relative;
            width: 400px;
            height: 600px;
            background: blue;
        }

        .inner {
            position: absolute;
            width: 200px;
            height: 300px;
            background: red;
            left: 50%;
            top: 50%;
            margin: -150px 0 0 -100px;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner"></div>
    </div>
</body>

</html>
```

### 未知宽高：在position的基础上加入transform: translate(-50%, -50%);

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .outer {
            width: 400px;
            height: 600px;
            /* background: blue; */
            border: 1px solid red;
            background-color: transparent;
            position: relative;
        }

        .inner {
            position: absolute;
            background: red;
            left: 50%;
            top: 50%;
            transform: translate(-50%, -50%);
        }
    </style>
</head>

<body>
    <div class="outer"> <span class="inner">我想居中显示</span>
    </div>
</body>

</html>
```

###  使用绝对定位，top,left,right,bottom:0,margin: auto;

### flex 水平垂直居中

```html
<html lang="en">

<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
        .outer {
            width: 400px;
            height: 600px;
            display: flex;
            /* 垂直居中 */
            align-items: center;
            /* 水平居中 */
            justify-content: center;
            border: 1px solid red;
            background-color: transparent;
        }

        .inner {
            background: red;
            width: 200px;
            height: 300px;
            border: 1px solid blue;
        }
    </style>
</head>

<body>
    <div class="outer">
        <div class="inner">我想居中显示</div>
    </div>
</body>

</html>
```



## visibility 和 display 的差别（还有opacity) 

> visibility：设置 hidden 会隐藏元素，但是其位置还存在与页面文档流中，不会被删除，所以会触发浏览器渲染引擎的重绘
>
> display：设置了 none 属性会隐藏元素，且其位置也不会被保留下来，所以会触发浏览器渲染引擎的回流和重绘。
>
> opacity：会将元素设置为透明，但是其位置也在页面文档流中，不会被删除，所以会触发浏览器渲染引擎的重绘
>
> opacity 可以有过渡效果

##  了解box-sizing吗？ 

box-sizing 属性可以被用来调整这些表现:

content-box 是默认值。如果你设置一个元素的宽为100px，那么这个元素的内容区会有100px 宽，并且任何边框和内边距的宽度都会被增加到 后绘制出来的元素宽度中。

border-box 告诉浏览器：你想要设置的边框和内边距的值是包含在width内的。也就是说，如果你将一个元素的width设为100px，那么这100px会包含它的border和padding，内容区的实际宽度是width减去(border + padding)的值。大多数情况下，这使得我们更容易地设定一个元素的宽高。

## 什么是 BFC 

BFC（Block Formatting Context）格式化上下文，是 Web 页面中盒模型布局的 CSS 渲染模式，指一个独立的渲染区域或者说是一个隔离的独立容器。

**形成 BFC 的条件**五种：

浮动元素，float 除 none 以外的值

定位元素，position（absolute，fixed） display 为以下其中之一的值 inline-block，table-cell，table-caption overflow 除了 visible 以外的值（hidden，auto，scroll）

HTML 就是一个 BFC

**BFC 的特性：**

内部的 Box 会在垂直方向上一个接一个的放置。

垂直方向上的距离由 margin 决定

bfc 的区域不会与 float 的元素区域重叠。计算 bfc 的高度时，浮动元素也参与计算

bfc 就是页面上的一个独立容器，容器里面的子元素不会影响外面元素。





## 两个div上下排列，都设margin，有什么现象？ 

都正取大

一正一负相加

问：为什么会有这种现象？你能解释一下吗

是由块级格式上下文决定的，BFC，元素在 BFC 中会进行上下排列，然后垂直距离由 margin 决定，并且会发生重叠，具体表现为同正取 大的，同负取绝对值 大的，一正一负，相加

BFC 是页面中一个独立的隔离容器，内部的子元素不会影响到外部的元素。



## block，inline和inlinke-block细节对比？

• display:block

​	a.  block元素会独占一行，多个block元素会各自新起一行。默认情况下，block 元素宽度自动填满其父元素宽度。

​	b.  block元素可以设置width,height属性。块级元素即使设置了宽度,仍然是独占一行。

​	c.  block元素可以设置margin和padding属性。

• display:inline

​	a、inline元素不会独占一行，多个相邻的行内元素会排列在同一行里，直到一行排列不下，才会新换一行，其宽度随元素的内容而变化。 b、inline元素设置width,height属性无效。

​	c、inline元素的margin和padding属性，水平方向的padding-left,padding-right, margin-left, margin-right都产生边距效果；但竖直方向的 padding-top, padding-bottom, margin-top, margin-bottom不会产生边距效果。

• display:inline-block

​	a、简单来说就是将对象呈现为inline对象，但是对象的内容作为block对象呈现。之后的内联对象会被排列在同一行内。比如我们可以给一个link（a元素） inline-block属性值，使其既具有block的宽度高度特性又具有inline的同行特性。

补充说明

​	a.  一般我们会用display:block，display:inline或者display:inline-block 来调整元素的布局级别，其实display的参数远远不止这三种，仅仅是比较常用而已。

​	b.  IE（低版本IE）本来是不支持inline-block的，所以在IE中对内联元素使用display:inline-block，理论上IE是不识别的，但使用display:inline-block 在IE下会触发layout，从而使内联元素拥有了display:inline-block属性的表象。

## 什么叫优雅降级和渐进增强？



渐进增强 progressive enhancement：针对低版本浏览器进行构建页面，保证最基本的功能，然后再针对高级浏览器进行效果、交互等改进和追加功能达到更好的用户体验。

优雅降级 graceful degradation：一开始就构建完整的功能，然后再针对低版本浏览器进行兼容。

区别：优雅降级是从复杂的现状开始，并试图减少用户体验的供给，而渐进增强则是从一个非常基础的，能够起作用的版本开始，并不断扩充，以适应未来环境的需要。降级（功能衰减）意味着往回看；而渐进增强则意味着朝前看，同时保证其根基处于安全地带。 ["优雅降级"观点](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

"优雅降级"观点认为应该针对那些最高级、最完善的浏览器来设计网站。而将那些被认为 "过时"或有功能缺失的浏览器下的测试工作安排在开发周期的最后阶段，并把测试对象限定为主流浏览器（如 IE、Mozilla 等）的前一个版本。

在这种设计范例下，旧版的浏览器被认为仅能提供"简陋却无妨 (poor, but passable)" 的浏览体验。你可以做一些小的调整来适应某个特定的浏览器。但由于它们并非我们所关注的焦点，因此除了修复较大的错误之外，其它的差异将被直接忽略。

"渐进增强"观点

"渐进增强"观点则认为应关注于内容本身。

内容是我们建立网站的诱因。有的网站展示它，有的则收集它，有的寻求，有的操作，还有的网站甚至会包含以上的种种，但相同点是它们全都涉及到内容。这使得"渐进增强"成为一种更为合理的设计范例。这也是它立即被 Yahoo! 所采纳并用以构建其"分级式浏览器支持 (Graded Browser Support)"策略的原因所在。



## 说说浮动元素会引起的问题和你的解决办法

 问题：

1. 父元素的高度无法被撑开，影响与父元素同级的元素
2. 与浮动元素同级的非浮动元素会跟随其后
3. 若非第一个元素浮动，则该元素之前的元素也需要浮动，否则会影响页面显示的结构

解决方法：

使用CSS中的clear:both;属性来清除元素的浮动可解决问题(2)、(3)，对于问题(1)，添加如下样式，给父元素添加clearfix样式：

```css
.clearfix:after{ content: ".";

display: block; height: 0;

clear: both;

visibility: hidden;

}

.clearfix{

display: inline-block;

} /* for IE/Mac */
```





清除浮动的几种方法：（1）额外标签法，`<divstyle="clear:both;"></div>`（缺点：不过这个办法会增加额外的标签使HTML结构看起来不够简洁。）

1. 使用after伪类

   ```css
   #parent:after{
   
     content:" ";
   
     height:0;
   
     visibility:hidden;
   
     display:block;
   
     clear:both;
   
   }
   ```

   

2. 浮动外部元素

3. 设置`overflow`为`hidden`或者auto

## 你有哪些性能优化的方法？

1. 减少http请求次数：CSSSprites,JS、CSS源码压缩、图片大小控制合适；网页Gzip，CDN托管，data缓存，图片服务器。
2. 前端模板 JS+数据，减少由于HTML标签导致的带宽浪费，前端用变量保存AJAX请求结果，每次操作本地变量，不用请求，减少请求次数

1. 用innerHTML代替DOM操作，减少DOM操作次数，优化javascript性能。
2. 当需要设置的样式很多时设置className而不是直接操作style。
3. 少用全局变量、缓存DOM节点查找的结果。减少IO读取操作。
4. 避免使用CSS Expression（css表达式)又称Dynamic properties(动态属性)。
5. 图片预加载，将样式表放在顶部，将脚本放在底部 加上时间戳。



(1) 减少HTTP请求次数

(2) 使用CDN

(3) 避免空的src和href

(4) 为文件头指定Expires

(5) 使用gzip压缩内容

(6) 把CSS放到顶部

(7) 把JS放到底部

(8) 避免使用CSS表达式

(9) 将CSS和JS放到外部文件中

(10) 避免跳转

(11) 可缓存的AJAX

(12) 使用GET来完成AJAX请求

## 为什么要初始化CSS样式？

 

因为浏览器的兼容问题，不同浏览器对有些标签的默认值是不同的，如果没对CSS初始化往往会出现浏览器之间的页面显示差异。

当然，初始化样式会对SEO有一定的影响，但鱼和熊掌不可兼得，但力求影响最小的情况下初始化。

最简单的初始化方法就是：

```css
\* {

padding: 0;

margin: 0;

} （不建议）
```





## 解释下浮动和它的工作原理？清除浮动的技巧？

**浮动元素脱离文档流，不占据空间。浮动元素碰到包含它的边框或者浮动元素的边框停留。**

(1) 使用空标签清除浮动。

> 这种方法是在所有浮动标签后面添加一个空标签定义css clear:both.弊端就是增加了无意义标签。

(2) 使用overflow。

> 给包含浮动元素的父标签添加css属性overflow:auto;zoom:1;zoom:1用于兼容IE6。

(3) 使用after伪对象清除浮动。

> 该方法只适用于非IE浏览器。具体写法可参照以下示例。使用中需注意以下几点。该方法中必须为需要清除浮动元素的伪对象中设置 height:0，否则该元素会比实际高出若干像素；

## CSS样式表根据所在网页的位置，可分为哪几种样式表？

>  行内样式表，内嵌样式表，外部样式表

## 谈谈你对CSS中刻度的认识？

 在CSS中刻度是用于设置元素尺寸的单位。

a.  特殊值0可以省略单位。例如：margin:0px可以写成margin:0

b.  一些属性可能允许有负长度值，或者有一定的范围限制。如果不支持负长度值，那应该变换到能够被支持的最近的一个长度值。 c、长度单位包括：相对单位和绝对单位。

相对长度单位有：em,ex,ch,rem,vw,vh,vmax,vmin 绝对长度单位有：cm,mm,q,in,pt,pc,px 绝对长度单位：1in = 2.54cm = 25.4 mm = 72pt = 6pc = 96px

文本相对长度单位：em 相对长度单位是相对于当前对象内文本的字体尺寸，如当前对行内文本的字体尺寸未被人为设置，则相对于浏览器的默认字体尺寸。(相对父元素的字体大小倍

数)

body { font-size: 14px; } h1 { font-size: 16px; }

.size1 p { font-size: 1em; }

.size2 p { font-size: 2em; }

.size3 p { font-size: 3em; }

文本相对长度单位：rem rem是CSS3新增的一个相对单位（root em，根em），相对于根元素(即html 元素)font-size计算值的倍数

只相对于根元素的大小

浏览器的默认字体大小为16像素，浏览器默认样式也称为user agent stylesheet，就是所有浏览器内置的默认样式，多数是可以被修改的，但chrome

不能直接修改，可以被用户样式覆盖。

## 请你说说em与rem的区别？

rem ： rem是CSS3新增的一个相对单位（root em，根em），相对于根元素(即html 元素)font-size计算值的倍数

只相对于根元素的大小

rem（font size of the root element）是指相对于根元素的字体大小的单位。

简单的说它就是一个相对单位。

作用：利用rem可以实现简单的响应式布局，可以利用html元素中字体的大小与屏幕间的比值设置font-size的值实现当屏幕分辨率变化时让元素也变化，以前的天猫tmall就使用这种办法。

em ：

文本相对长度单位。相对于当前对象内文本的字体尺寸。如当前对行内文本的字体尺寸未被人为设置，则相对于浏览器的默认字体尺寸(默认16px)。(相对父元素的字体大小倍数)

em（font size of the element）是指相对于父元素的字体大小的单位。它与 rem之间其实很相似，区别在。（相对是的HTML元素的字体大，默认16px） em与rem的重要区别： 它们计算的规则一个是依赖父元素另一个是依赖根元素计算。

## 请你说说box-sizing属性的的用法？

 设置或检索对象的盒模型组成模式

a.  box-sizing:content-box：padding和border不被包含在定义的width和 height之内。对象的实际宽度等于设置的width值和border、padding之和，即 ( Element width = width + border + padding，但占有页面位置还要加上 margin ) 此属性表现为标准模式下的盒模型。

b.  box-sizing:border-box：padding和border被包含在定义的width和height 之内。对象的实际宽度就等于设置的width值，即使定义有border和padding 也不会改变对象的实际宽度，即 ( Element width = width ) 此属性表现为怪异模式下的盒模型。

## 浏览器标准模式和怪异模式之间的区别是什么？ 

**所谓的标准模式是指，浏览器按W3C标准解析执行代码；怪异模式则是使用浏览器自己的方式解析执行代码**，因为不同浏览器解析执行的方式不一样，所以我们称之为怪异模式。浏览器解析时到底使用标准模式还是怪异模式，与你网页中的DTD声明直接相关，DTD声明定义了标准文档的类型（标准模式解析）文档类型，会使浏览器使用相应的方式加载网页并显示，忽略DTD声明,将使网页进入怪异模式(quirks mode)。

## 怪异Quirks模式是什么，它和标准Standards模式有什么区别？

从IE6开始，引入了Standards模式，标准模式中，浏览器尝试给符合标准的文档在规范上的正确处理达到在指定浏览器中的程度。

在IE6之前CSS还不够成熟，所以IE5等之前的浏览器对CSS的支持很差，IE6 将对CSS提供更好的支持，然而这时的问题就来了，因为有很多页面是基于旧的布局方式写的，而如果IE6 支持CSS则将令这些页面显示不正常，如何在即保证不破坏现有页面，又提供新的渲染机制呢？

在写程序时我们也会经常遇到这样的问题，如何保证原来的接口不变，又提供更强大的功能，尤其是新功能不兼容旧功能时。遇到这种问题时的一个常见做法是增加参数和分支，即当某个参数为真时，我们就使用新功能，而如果这个参数 不为真时，就使用旧功能，这样就能不破坏原有的程序，又提供新功能。IE6也是类似这样做的，它将DTD当成了这个"参数"，因为以前的页面大家都不会去写 DTD，所以IE6就假定 如果写了DTD，就意味着这个页面将采用对CSS支持更好的布局，而如果没有，则采用兼容之前的布局方式。这就是Quirks模式（怪癖模式，诡异模式，怪异模式）。

区别：总体会有布局、样式解析和脚本执行三个方面的区别。

盒模型： 在W3C标准中，如果设置一个元素的宽度和高度，指的是元素内容的

宽度和高度，而在Quirks 模式下，IE的宽度和高度还包含了padding和border。

设置行内元素的高宽： 在Standards模式下，给<span>等行内元素设置wdith 和height都不会生效，而在quirks模式下，则会生效。

设置百分比的高度： 在standards模式下，一个元素的高度是由其包含的内容来决定的，如果父元素没有设置百分比的高度，子元素设置一个百分比的高度是无效的用margin:0auto设置水平居中：使用margin:0auto在standards模式下可以使元素水平居中，但在quirks模式下却会失效。

（还有很多，答出什么不重要，关键是看他答出的这些是不是自己经验遇到的，还是说都是看文章看的，甚至完全不知道。）

## 说说你对边距折叠的理解?

外边距折叠：相邻的两个或多个外边距(margin)在垂直方向会合并成一个外边距（margin）

相邻：没有被非空内容、padding、border或clear分隔开的margin特性. 非空内容就是说这元素之间要么是兄弟关系或者父子关系垂直方向外边距合并计算:

a、参加折叠的margin都是正值：取其中margin较大的值为最终margin值。

 b、参与折叠的margin都是负值：取的是其中绝对值较大的，然后，从0位置，负向位移。

c、参与折叠的margin中有正值，有负值：先取出负 margin 中绝对值中最大的，然后，和正margin值中最大的margin相加。

## 内联与块级标签有何区别？

Html中的标签默认主要分为两大类型，一类为块级元素，另一类是行内元素，许多人也把行内称为内联，所以叫内联元素，其实就是一个意思。为了很好的布局，必须理解它们间的区别。

## 说说隐藏元素的方式有哪些？

a.  使用CSS的display:none，不会占有原来的位置

b.  使用CSS的visibility:hidden，会占有原来的位置 

c、使用HTML5中的新增属性hidden="hidden"，不会占有原来的位置

## 为什么重置浏览器默认样式，如何重置默浏览器认样式？ 

每种浏览器都有一套默认的样式表，即user agent stylesheet，网页在没有指定的样式时，按浏览器内置的样式表来渲染。这是合理的，像word中也有一些预留样式，可以让我们的排版更美观整齐。不同浏览器甚至同一浏览器不同版本的默认样式是不同的。但这样会有很多兼容问题。 

a、最简单的办法：（不推荐使用）`*{margin: 0;padding: 0;}`。

 b、使用CSSReset可以将所有浏览器默认样式设置成一样。

c、normalize：也许有些cssreset过于简单粗暴，有点伤及无辜，normalize是另一个选择。bootstrap已经引用该css来重置浏览器默认样式，比普通的 cssreset要精细一些，保留浏览器有用的默认样式，支持包括手机浏览器在内的超多浏览器，同时对HTML5元素、排版、列表、嵌入的内容、表单和表格都进行了一般化。天猫 使用的css reset重置浏览器默认样式：

```css
@charset "gb2312"; body, h1, h2, h3, h4, h5, h6, hr, p, blockquote, dl, dt, dd, ul, ol, li, pre, form, fieldset, legend, button, input, textarea, th, td { margin: 0; padding: 0 } body, button, input, select, textarea { font: 12px "microsoft yahei"; line-height: 1.5;

-ms-overflow-style: scrollbar

}

h1, h2, h3, h4, h5, h6 { font-size: 100%

}

ul, ol {

list-style: none

}

a {

text-decoration: none; cursor:pointer

} a:hover { text-decoration: underline

} img { border: 0 } button, input, select, textarea { font-size: 100%

} table { border-collapse: collapse; border-spacing: 0

}

.clear { clear:both }

.fr {

float:right }

.fl {

float:left }

.block { display:block; text-indent:-999em }
```





## 谈谈你对BFC与IFC的理解？(是什么，如何产生，作用)

 

(1)、什么是BFC与IFC

a.  BFC（Block Formatting Context）即"块级格式化上下文"，IFC（Inline FormattingContext）即行内格式化上下文。常规流（也称标准流、普通流）是一个文档在被显示时最常见的布局形态。一个框在常规流中必须属于一个格式化上下文，你可以把BFC想象成一个大箱子，箱子外边的元素将不与箱子内的元素产生作用。

b.  BFC是W3C CSS 2.1 规范中的一个概念，它决定了元素如何对其内容进行定位，以及与其他元素的关系和相互作用。当涉及到可视化布局的时候，Block Formatting Context提供了一个环境，HTML元素在这个环境中按照一定规则进行布局。一个环境中的元素不会影响到其它环境中的布局。比如浮动元素会形成 BFC，浮动元素内部子元素的主要受该浮动元素影响，两个浮动元素之间是互不影响的。也可以说BFC就是一个作用范围。

c.  在普通流中的 Box(框) 属于一种 formattingcontext(格式化上下文) ，类型可以是block，或者是inline，但不能同时属于这两者。并且，Blockboxes(块框) 在 block formatting context(块格式化上下文) 里格式化，Inline

boxes(块内框) 则在Inline Formatting Context(行内格式化上下文) 里格式化。

(2)、如何产生BFC

当一个HTML元素满足下面条件的任何一点，都可以产生Block Formatting

Context：

a.  float的值不为none

b.  overflow的值不为visible

c.  display的值为table-cell, table-caption, inline-block中的任何一个 d、position的值不为relative和static

CSS3触发BFC方式则可以简单描述为：在元素定位非static，relative的情况下触发，float也是一种定位方式。

(3)、BFC的作用与特点

a、不和浮动元素重叠，清除外部浮动，阻止浮动元素覆盖；

如果一个浮动元素后面跟着一个非浮动的元素，那么就会产生一个重叠的现象。

常规流（也称标准流、普通流）是一个文档在被显示时最常见的布局形态，当 float不为none时，position为absolute、fixed时元素将脱离标准流。

## BFC会与float元素相互覆盖吗？为什么？举例说明

不会，因为 BFC 是页面中一个独立的隔离容器，其内部的元素不会与外部的元素相互影响，比如两个div，上面的 div 设置了 float，那么如果下面的元素不是 BFC，也没有设置 float，会形成对上面的元素进行包裹内容的情况，如果设置了下面元素为 overflow：hidden；属性那么就能够实现经典的两列布局，左边内容固定宽度，右边因为是 BFC 所以会进行自适应。

## 超链接样式顺序

L-V-H-A（link,visited,hover,active）

## 说说你对页面中使用定位(position)的理解？

 

使用css布局position非常重要，语法如下：

position：static | relative | absolute | fixed | center | page | sticky 默认值：static，center、page、sticky是CSS3中新增加的值。

- static
  - 可以认为静态的，默认元素都是静态的定位，对象遵循常规流。此时4个定位偏移属性不会被应用，也就是使用left，right，bottom，top将不会生效。

- relative
  - 相对定位，**对象遵循常规流**，并且参照自身在常规流中的位置通过top，right， bottom，left这4个定位偏移属性进行偏移时不会影响常规流中的任何元素。

- absolute
  - 绝对定位，对象脱离常规流，此时偏移属性参照的是离自身最近的定位祖先元素，如果没有定位的祖先元素，则一直回溯到body元素。盒子的偏移位置不影响常规流中的任何元素，其margin不与其他任何margin折叠。
  - 元素定位参考的是离自身最近的定位祖先元素，要满足两个条件，第一个是自己的祖先元素，可以是父元素也可以是父元素的父元素，一直找，如果没有则选择body为对照对象。第二个条件是要求祖先元素必须定位，通俗说就是 position的属性值为非static都行。

- fixed 固定定位，
  - 与absolute一致，但偏移定位是以窗口为参考。当出现滚动条时，对象不会随着滚动。

- center
  - 与absolute一致，但偏移定位是以定位祖先元素的中心点为参考。盒子在其包含容器垂直水平居中。（CSS3）
- page
  - 与absolute一致。元素在分页媒体或者区域块内，元素的包含块始终是初始包含块，否则取决于每个absolute模式。（CSS3）

- sticky
  - 对象在常态时遵循常规流。它就像是relative和fixed的合体，当在屏幕中时按常规流排版，当卷动到屏幕外时则表现如fixed。该属性的表现是现实中你见到的吸附效果。（CSS3）

## 如何解决多个元素重叠问题？ 

使用z-index属性可以设置元素的层叠顺序 z-index属性

语法：z-index: auto |` <integer>` 默认值：auto

适用于：定位元素。即定义了position为非static的元素取值：

auto： 元素在当前层叠上下文中的层叠级别是0。元素不会创建新的局部层叠上下文，除非它是根元素。

整数： 用整数值来定义堆叠级别。可以为负值。 说明：检索或设置对象的层叠顺序。 z-index用于确定元素在当前层叠上下文中的层叠级别，并确定该元素是否创建新的局部层叠上下文。

当多个元素层叠在一起时，数字大者将显示在上面。

## 页面布局的方式有哪些？

方式：双飞翼、多栏、弹性、流式、瀑布流、响应式布局

（1）、双飞翼布局

经典三列布局，也叫做圣杯布局【Holy Grail of Layouts】是Kevin Cornell 在2006年提出的一个布局模型概念，在国内最早是由淘宝UED的工程师传播开来，在中国也有叫法是双飞翼布局，它的布局要求有几点： a、三列布局，中间宽度自适应，两边定宽； b、中间栏要在浏览器中优先展示渲染； c、允许任意列的高度最高；

d.  要求只用一个额外的DIV标签；

e.  要求用最简单的CSS、最少的HACK语句；

在不增加额外标签的情况下，圣杯布局已经非常完美，圣杯布局使用了相对定位，

以后布局是有局限性的，而且宽度控制要改的地方也多。在淘宝UED（User Experience Design）探讨下，增加多一个div就可以不用相对布局了，只用到了浮动和负边距，这就是我们所说的双飞翼布局。

(2)、多栏布局

a、栏栅格系统：就是利用浮动实现的多栏布局，在bootstrap中用的非常多。 b、多列布局：栅格系统并没有真正实现分栏效果（如word中的分栏），CSS3 为了满足这个要求增加了多列布局模块

(3)、弹性布局（Flexbox）

CSS3引入了一种新的布局模式------Flexbox布局，即伸缩布局盒模型（Flexible Box），用来提供一个更加有效的方式制定、调整和分布一个容器里项目布局，即使它们的大小是未知或者动态的，这里简称为Flex。

Flexbox布局常用于设计比较复杂的页面，可以轻松的实现屏幕和浏览器窗口大小发生变化时保持元素的相对位置和大小不变，同时减少了依赖于浮动布局实现元素位置的定义以及重置元素的大小。

Flexbox布局在定义伸缩项目大小时伸缩容器会预留一些可用空间，让你可以调节伸缩项目的相对大小和位置。例如，你可以确保伸缩容器中的多余空间平均分配多个伸缩项目，当然，如果你的伸缩容器没有足够大的空间放置伸缩项目时，

浏览器会根据一定的比例减少伸缩项目的大小，使其不溢出伸缩容器。

综合而言，Flexbox布局功能主要具有以下几点：

a.  屏幕和浏览器窗口大小发生改变也可以灵活调整布局；

b.  可以指定伸缩项目沿着主轴或侧轴按比例分配额外空间（伸缩容器额外空间），从而调整伸缩项目的大小；

c.  可以指定伸缩项目沿着主轴或侧轴将伸缩容器额外空间，分配到伸缩项目之前、之后或之间；

d.  可以指定如何将垂直于元素布局轴的额外空间分布到该元素的周围； e、可以控制元素在页面上的布局方向；

f、可以按照不同于文档对象模型（DOM）所指定排序方式对屏幕上的元素重新排序。也就是说可以在浏览器渲染中不按照文档流先后顺序重排伸缩项目顺序。

(4)、瀑布流布局

瀑布流布局是流式布局的一种。是当下比较流行的一种网站页面布局，视觉表现为参差不齐的多栏布局，随着页面滚动条向下滚动，这种布局还会不断加载数据块并附加至当前尾部。最早采用此布局的网站是Pinterest，逐渐在国内流行开来。

优点：

a.  有效的降低了界面复杂度，节省了空间：我们不再需要臃肿复杂的页码导航链接或按钮了。

b.  对触屏设备来说，交互方式更符合直觉：在移动应用的交互环境当中，通过向上滑动进行滚屏的操作已经成为最基本的用户习惯，而且所需要的操作精准程度远远低于点击链接或按钮。

c.  更高的参与度：以上两点所带来的交互便捷性可以使用户将注意力更多的集中在内容而不是操作上，从而让他们更乐于沉浸在探索与浏览当中。

缺点：

a、有限的用例：

无限滚动的方式只适用于某些特定类型产品当中一部分特定类型的内容。

例如，在电商网站当中，用户时常需要在商品列表与详情页面之间切换，这种情况下，传统的、带有页码导航的方式可以帮助用户更稳妥和准确的回到某个特定的列表页面当中。 b、额外的复杂度：

那些用来打造无限滚动的JS库虽然都自称很容易使用，但你总会需要在自己的产品中进行不同程度的定制化处理，以满足你们自己的需求;另外这些JS库在浏览器和设备兼容性等方面的表现也参差不齐，你必须做好充分的测试与调整工作。

c.  再见了，页脚：

如果使用了比较典型的无限滚动加载模式，这就意味着你可以和页脚说拜拜了。最好考虑一下页脚对于你的网站，特别是用户的重要性;如果其中确实有比较重要的内容或链接，那么最好换一种更传统和稳妥的方式。千万不要耍弄你的用户，当他们一次次的浏览到页面底部，看到页脚，却因为自动加载的内容突然出现而无论如何都无法点击页脚中的链接时，他们会变的越发愤怒。

d.  集中在一页当中动态加载数据，与一页一页的输出相比，究竟那种方式更利于SEO，这是你必须考虑的问题。对于某些以类型网站来说，在这方面进行冒险是很不划算的。

e.  关于页面数量的印象：

其实站在用户的角度来看，这一点并非负面;不过，如果对于你的网站来说，通过更多的内容页面展示更多的相关信息(包括广告)是很重要的策略，那么单页无限滚动的方式对你并不适用。

(5)、流式布局（Fluid）

固定布局和流式布局在网页设计中最常用的两种布局方式。固定布局能呈现网页的原始设计效果，流式布局则不受窗口宽度影响，流式布局使用百分比宽度来限定布局元素，这样可以根据客户端分辨率的大小来进行合理的显示。

(6)、响应式布局

响应式布局是EthanMarcotte在2010年5月份提出的一个概念，简而言之，就是一个网站能够兼容多个终端------而不是为每个终端做一个特定的版本。这个概念是为解决移动互联网浏览而诞生的。

响应式布局可以为不同终端的用户提供更加舒适的界面和更好的用户体验，而且随着目前大屏幕移动设备的普及，用"大势所趋"来形容也不为过。随着越来越多的设计师采用这个技术，我们不仅看到很多的创新，还看到了一些成形的模式。

优点：

a.  面对不同分辨率设备灵活性强

b.  能够快捷解决多设备显示适应问题缺点： a、兼容各种设备工作量大，效率低下

b.  代码累赘，会出现隐藏无用的元素，加载时间加长

c.  其实这是一种折中性质的设计解决方案，多方面因素影响而达不到最佳效果 d、一定程度上改变了网站原有的布局结构，会出现用户混淆的情况

## overflow :hidden是否形成新的块级格式化上下文？

 

会形成，触发BFC的条件有：

- float的值不为none。
- overflow的值不为visible。
- display的值为table-cell, table-caption, inline-block 中的任何一个。
- position的值不为relative 和static。

## div+css的布局较table布局有什么优点？

改版的时候更方便 只要改css文件。

页面加载速度更快、结构化清晰、页面显示简洁。

表现与结构相分离。

易于优化（seo）搜索引擎更友好，排名更容易靠前。

## 为什么利用多个域名来存储网站资源会更有效？

CDN 缓存更方便

突破浏览器并发限制节约cookie带宽

节约主域名的连接数，优化页面响应速度防止不必要的安全问题

## 请谈一下你对网页标准和标准制定机构重要性的理解。

网页标准和标准制定机构都是为了能让web发展的更'健康'，开发者遵循统一的标准，降低开发难度，开发成本，SEO也会更好做，也不会因为滥用代码导致各种BUG、安全问题，最终提高网站易用性。

## 简述一下src与href的区别。

src用于替换当前元素，href用于在当前文档和引用资源之间确立联系。

src是source的缩写，指向外部资源的位置，指向的内容将会嵌入到文档中当前标签所在位置；在请求src资源时会将其指向的资源下载并应用到文档内，例如js脚本，img图片和frame等元素。

`\<script src ="js.js"\>\</script\>`

当浏览器解析到该元素时，会暂停其他资源的下载和处理，直到将该资源加载、编译、执行完毕，图片和框架等元素也如此，类似于将所指向资源嵌入当前标签内。这也是为什么将 js脚本放在底部而不是头部。

href是Hypertext Reference的缩写，指向网络资源所在位置，建立和当前元素（锚点）或当前文档（链接）之间的链接，如果我们在文档中添加

\`<link href="common.css" rel="stylesheet"/\>`

那么浏览器会识别该文档为css文件，就会并行下载资源并且不会停止对当前文档的处理。

这也是为什么建议使用link方式来加载css，而不是使用\`@import`方式。

## 知道什么是微格式吗？谈谈理解。在前端构建中应该考虑微格式吗？

微格式（Microformats）是一种让机器可读的语义化XHTML词汇的集合，是结构化数据的开放标准。是为特殊应用而制定的特殊格式。

优点：将智能数据添加到网页上，让网站内容在搜索引擎结果界面可以显示额外的提示。（应用范例：豆瓣，有兴趣自行google）

## 在css/js代码上线之后开发人员经常会优化性能，从用户刷新网页开始，一次js请求一般情况下有哪些地方会有缓存处理？

dns缓存，cdn缓存，浏览器缓存，服务器缓存。

## 一个页面上有大量的图片（大型电商网站），加载很慢，你有哪些方法优化这些图片的加载，给用户更好的体验。

图片懒加载，在页面上的未可视区域可以添加一个滚动条事件，判断图片位置与浏览器顶端的距离与页面的距离，如果前者小于后者，优先加载。

如果为幻灯片、相册等，可以使用图片预加载技术，将当前展示图片的前一张和后一张优先下载。

如果图片为css图片，可以使用CSSsprite，SVGsprite，Iconfont、Base64等技术。

如果图片过大，可以使用特殊编码的图片，加载时会先加载一张压缩的特别厉害的缩略图，以提高用户体验。

如果图片展示区域小于图片的真实大小，则因在服务器端根据业务需要先行进行图片压缩，图片压缩后大小与展示一致。

## 谈谈以前端角度出发做好SEO需要考虑什么？

了解搜索引擎如何抓取网页和如何索引网页

你需要知道一些搜索引擎的基本工作原理，各个搜索引擎之间的区别，搜索机器人

（SE robot 或叫 web crawler）如何进行工作，搜索引擎如何对搜索结果进行排序等等。

Meta标签优化[主要包括主题（Title)，网站描述(Description)，和](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)关键词（Keywords）。还有一些其它的隐藏文字比如Author（作者），Category（目录），Language（编码语种）等。

如何选取关键词并在网页中放置关键词

搜索就得用关键词。关键词分析和选择是SEO最重要的工作之一。首先要给网站确定主关键词（一般在5个上下），然后针对这些关键词进行优化，包括关键词密度（Density），相关度（Relavancy），突出性（Prominency）等等。

了解主要的搜索引擎

虽然搜索引擎有很多，但是对网站流量起决定作用的就那么几个。比如英文的主要有

Google，Yahoo，Bing等；中文的有百度，搜狗，有道等。不同的搜索引擎对页面的抓取和索引、排序的规则都不一样。还要了解各搜索门户和搜索引擎之间的关系，比如AOL网页搜索用的是Google的搜索技术，MSN用的是Bing的技术。

主要的互联网目录

Open Directory自身不是搜索引擎，而是一个大型的网站目录，他和搜索引擎的主要区别是网站内容的收集方式不同。目录是人工编辑的，主要收录网站主页；搜索引擎是自动收集的，除了主页外还抓取大量的内容页面。

按点击付费的搜索引擎

搜索引擎也需要生存，随着互联网商务的越来越成熟，收费的搜索引擎也开始大行其道。最典型的有Overture和百度，当然也包括Google的广告项目Google Adwords。越来越多的人通过搜索引擎的点击广告来定位商业网站，这里面也大有优化和排名的学问，你得学会用最少的广告投入获得最多的点击。

搜索引擎登录

网站做完了以后，别躺在那里等着客人从天而降。要让别人找到你，最简单的办法就是将网站提交（submit）到搜索引擎。如果你的是商业网站，主要的搜索引擎和目录都会要求你付费来获得收录（比如Yahoo要299美元），但是好消息是（至少到目前为止）最大的搜索引擎Google目前还是免费，而且它主宰着60％以上的搜索市场。

链接交换和链接广泛度（Link Popularity）

网页内容都是以超文本（Hypertext）的方式来互相链接的，网站之间也是如此。除了搜索引擎以外，人们也每天通过不同网站之间的链接来Surfing（"冲浪"）。其它网站到你的网站的链接越多，你也就会获得更多的访问量。更重要的是，你的网站的外部链接数越多，会被搜索引擎认为它的重要性越大，从而给你更高的排名。

合理的标签使用

## 超链接访问过后hover样式就不出现的问题是什么？如何解决？

被点击访问过的超链接样式不在具有hover和active了,解决方法是改变CSS属性的排列顺序: L-V-H-A（link,visited,hover,active）

## 什么是Css Hack？ie6,7,8的hack分别是什么？

针对不同的浏览器写不同的CSS code的过程，就是CSS hack。

## 什么是外边距重叠？重叠的结果是什么？

外边距重叠就是margin-collapse。

在CSS当中，相邻的两个盒子（可能是兄弟关系也可能是祖先关系）的外边距可以结合成一个单独的外边距。这种合并外边距的方式被称为折叠，并且因而所结合成的外边距称为折叠外边距。

折叠结果遵循下列计算规则：

两个相邻的外边距都是正数时，折叠结果是它们两者之间较大的值。

两个相邻的外边距都是负数时，折叠结果是两者绝对值的较大值。

两个外边距一正一负时，折叠结果是两者的相加的和。

## rgba()和opacity的透明效果有什么不同？

rgba()和opacity都能实现透明效果，但最大的不同是opacity作用于元素，以及元素内的所有内容的透明度，[而rgba()只作用于元素的颜色或其背景色。（设置rg](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)ba透明的元素的子元素不会继承透明效果！）

## 描述一个"reset"的CSS文件并如何使用它。知道normalize.css吗？你了解他们的不同之处？

重置样式非常多，凡是一个前端开发人员肯定有一个常用的重置CSS文件并知道如何使用它们。他们是盲目的在做还是知道为什么这么做呢？原因是不同的浏览器对一些元素有不同的默认样式，如果你不处理，在不同的浏览器下会存在必要的风险，或者更有戏剧性的性发生。

你可能会用[[Normalize]{.underline}](http://necolas.github.io/normalize.css/)来代替你的重置样式文件。它没有重置所有的样式风格，但仅提供了一套合理的默认样式值。既能让众多浏览器达到一致和合理，但又不扰乱其他的东西（如粗体的标题）。

在这一方面，无法做每一个复位重置。它也确实有些超过一个重置，它处理了你永远都不用考虑的怪癖，像HTML的audio元素不一致或line-height不一致。

## Sass、LESS是什么？大家为什么要使用他们？

他们是CSS预处理器。他是CSS上的一种抽象层。他们是一种特殊的语法/语言编译成CSS。

例如[[Less]{.underline}](http://www.lesscss.org/)是一种动态样式语言. 将CSS赋予了动态语言的特性，如变量，继承，运算， 函数. LESS 既可以在客户端上运行 (支持IE 6+, Webkit, Firefox)，也可一在服务端运行

(借助 Node.js)。

为什么要使用它们？

- [结构清晰，便于扩展。](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

- 可以方便地屏蔽浏览器私有语法差异。这个不用多说，封装对浏览器语法差异的重复处理，减少无意义的机械劳动。可以轻松实现多重继承。

- 完全兼容 CSS 代码，可以方便地应用到老项目中。LESS 只是在 CSS 语法上做了扩展，所以老的 CSS 代码也可以与 LESS 代码一同编译。

## html常见兼容性问题？

1. 双边距BUG float引起的 使用display

2. 3像素问题 使用float引起的 使用dislpay:inline -3px

3. 超链接hover 点击后失效 使用正确的书写顺序 link visited hover active

4. Ie z-index问题 给父级添加position:relative

5. Png 透明 使用js代码 改

6. Min-height 最小高度 ！Important 解决'

7. select 在ie6下遮盖 使用iframe嵌套

8. 为什么没有办法定义 1px 左右的宽度容器（IE6 默认的行高造成的，使用 over:hidden,zoom:0.08 line-height:1px）

9. IE5-8不支持opacity，解决办法：

   ```css
.opacity { opacity: 0.4
   
   ```

filter: alpha(opacity=60); /\* for IE5-7 \*/

-ms-filter: \"progid:DXImageTransform.Microsoft.Alpha(Opacity=60)\"; /\* for IE

8\*/

   }
   ```
   
   



## 对WEB标准以及W3C的理解与认识

标签闭合、标签小写、不乱嵌套、提高搜索机器人搜索几率、使用外 链css和js脚本、结构行为表现的分离、文件下载与页面速度更快、内容能被更多的用户所访问、内容能被更广泛的设备所访问、更少的代码和组件，容易维 护、改版方便，不需要变动页面内容、提供打印版本而不需要复制内容、提高网站易用性。

## 哪些css属性可以继承？

可继承： font-size font-family color, ul li dl dd dt; 不可继承 ：border padding margin width height ;

## b标签和strong标签,i标签和em标签的区别？

后者有语义，前者则无。

## text-align:center和line-height有什么区别？

text-align是水平对齐，line-height是行间。





## HTML5 存储类型有什么区别？

MediaAPI、TextTrackAPI、ApplicationCacheAPI、UserInteraction、DataTransfer

API、Command API、Constraint Validation API、History API

## 你怎么来实现页面设计图，你认为前端应该如何高质量完成工作? 一个满屏 品 字布局 如何设计?

-   首先划分成头部、body、脚部；。。。。。

-   实现效果图是最基本的工作，精确到2px；与设计师，产品经理的沟通和项目的参与做好的页面结构，页面重构和用户体验处理hack，兼容、写出优美的代码格式针对服务器的优化、拥抱 HTML5。

## 为什么利用多个域名来存储网站资源会更有效？

CDN 缓存更方便突破浏览器并发限制节约cookie带宽

节约主域名的连接数，优化页面响应速度防止不必要的安全问题

## 请谈一下你对网页标准和标准制定机构重要性的理解。

（无标准答案）网页标准和标准制定机构都是为了能让web发展的更'健康'，开发者遵循统一的标准，降低开发难度，开发成本，SEO也会更好做，也不会因为滥用代码导致各种BUG、安全问题，最终提高网站易用性。

## 请描述一下cookies，sessionStorage和localStorage的区别？

sessionStorage用于本地存储一个会话（session）中的数据，这些数据只有在同一个会话中的页面才能访问并且当会话结束后数据也随之销毁。因此sessionStorage不是一种[持久化的本地存储，仅仅是会话级别的存储。而loca](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)lStorage用于持久化的本地存储，除非主动删除数据，否则数据是永远不会过期的。

web storage和cookie的区别

Web Storage的概念和cookie相似，区别是它是为了更大容量存储设计的。Cookie 的大小是受限的，并且每次你请求一个新的页面的时候Cookie都会被发送过去，这样无形中浪费了带宽，另外cookie还需要指定作用域，不可以跨域调用。

除此之外，Web Storage 拥有 setItem,getItem,removeItem,clear 等方法，不像 cookie需要前端开发者自己封装setCookie，getCookie。但是Cookie也是不可以或缺的：Cookie的作用是与服务器进行交互，作为HTTP规范的一部分而存在 ，而 Web Storage仅仅是为了在本地"存储"数据而生。

## 知道css有个content属性吗？有什么作用？有什么应用？

知道。css的content属性专门应用在 before/after 伪元素上，用来插入生成内容。最常见的应用是利用伪类清除浮动。

after伪元素通过 content 在元素的后面生成了内容为一个点的块级素，再利用 clear:both清除浮动。

那么问题继续还有，知道css计数器（序列数字字符自动递增）吗？如何通过

css content属性实现css计数器？

css计数器是通过设置counter-reset 、counter-increment 两个属性 、及 counter()/counters()一个方法配合after / before 伪类实现。

## display:inline-block 什么时候不会显示间隙？ 

- 移除空格
- 使用margin 负值
- 使用 font-size:0
- letter-spacing word-spacing

## 行内元素float:left后是否变为块级元素？ 

行内元素设置成浮动之后变得更加像是 inline-block（行内块级元素，设置 成这个属性的元素会同时拥有行内和块级的特性， 明显的不同是它的默认宽度不是 100% ），这时候给行内元素设置

padding-top 和 padding-bottom或者width 、 height都是有效果的

##  如果需要手动写动画，你认为最小时间间隔是多久，为什么？

多数显示器默认频率是 60Hz ，即 1 秒刷新 60 次，所以理论上 小间隔为 1/60\*1000ms ＝ 16.7ms

## stylus，sass，less区别 

均具有"变量"、"混合"、"嵌套"、"继承"、"颜色混合"五大基本特性

Sass 和 LESS 语法较为严谨， LESS 要求一定要使用大括号"{}"， Sass 和 Stylus 可以通过缩进表示层次与嵌套关系

Sass 无全局变量的概念， LESS 和 Stylus有类似于其它语言的作用域概念

Sass 是基于 Ruby 语言的，而 LESS和 Stylus可以基于 NodeJS NPM 下载相应库后进行编译；这也是为什么安装Sass的时候有时候会报错，需要安装python脚本

优点：就不用我多说了，谁用谁知道，真香。

## 什么情况会触发重排和重绘？ 

1.  添加、删除、更新 DOM 节点
2.  通过 display: none 隐藏一个 DOM 节点-触发重排和重绘
3.  通过 visibility: hidden 隐藏一个 DOM 节点-只触发重绘，因为没有几何变化
4.  移动或者给页面中的 DOM 节点添加动画
5.  添加一个样式表，调整样式属性
6.  用户行为，例如调整窗口大小，改变字号，或者滚动

## HTML5和CSS3用的多吗？你了解它们的新属性吗？有在项目中用过吗？

 

html5：

1. 标签增删

(1)8个语义元素 header section footer aside nav main article figure

(2)内容元素mark高亮 progress进度

(3)新的表单控件calander date time email url search

(4)新的input类型 color date datetime datetime-local email

(5)移除过时标签big font frame frameset

1. canvas绘图，支持内联SVG。支持MathML
2. 多媒体audio video source embed track
3. 本地离线存储，把需要离线存储在本地的文件列在一个manifest配置文件
4. web存储。localStorage、SessionStorage css3：

CSS3边框如border-radius，box-shadow等；

CSS3背景如background-size，background-origin等；

CSS3 2D，3D转换如transform等； CSS3动画如animation等。



## get和post的区别

 

GET - 从指定的资源请求数据。

POST - 向指定的资源提交要被处理的数据。

GET：不同的浏览器和服务器不同，一般限制在2~8K之间，更加常见的是1k以内。

GET和POST的底层也是TCP/IP，GET/POST都是TCP链接。

GET产生一个TCP数据包；POST产生两个TCP数据包。

对于GET方式的请求，浏览器会把http header和data一并发送出去，服务器响应200（返回数据）；

而对于POST，浏览器先发送header，服务器响应100 continue，浏览器再发送 data，服务器响应200 ok（返回数据）。



## web性能优化

 降低请求量：合并资源，减少HTTP 请求数，minify/gzip 压缩，webP，lazyLoad。

加快请求速度：预解析DNS，减少域名数，并行加载，CDN 分发。

缓存：HTTP 协议缓存请求，离线缓存 manifest，离线数据缓存localStorage。

渲染：JS/CSS优化，加载顺序，服务端渲染，pipeline。

## 画一条0.5px的线 

采用meta viewport的方式

采用border-image的方式采用transform: scale()的方式

## transition和animation的区别

 

Animation和transition大部分属性是相同的，他们都是随时间改变元素的属性值，他们的主要区别是transition需要触发一个事件才能改变属性，而 animation不需要触发任何事件的情况下才会随时间改变属性值，并且

transition为2帧，从from .... to，而animation可以一帧一帧的。

## Flex布局

 一个用于页面布局的全新CSS3功能，Flexbox可以把列表放在同一个方向（从上到下排列，从左到右），并让列表能延伸到占用可用的空间。

较为复杂的布局还可以通过嵌套一个伸缩容器（flex container）来实现。 采用Flex布局的元素，称为Flex容器（flex container），简称\"容器\"。

它的所有子元素自动成为容器成员，称为Flex项目（flex item），简称\"项目\"。

常规布局是基于块和内联流方向，而Flex布局是基于flex-flow流可以很方便的用来做局中，能对不同屏幕大小自适应。

在布局上有了比以前更加灵活的空间

简单的分为容器属性和元素属性容器的属性：

flex-direction：决定主轴的方向（即子item的排列方法）

.box { flex-direction: row | row-reverse | column | column-reverse;

}

flex-wrap：决定换行规则

.box{

flex-wrap: nowrap | wrap | wrap-reverse;

} flex-flow： .box { flex-flow: <flex-direction> || <flex-wrap>;

}

justify-content：对其方式，水平主轴对齐方式 align-items：对齐方式，竖直轴线方向

项目的属性（元素的属性）： order属性：定义项目的排列顺序，顺序越小，排列越靠前，默认为0 flex-grow属性：定义项目的放大比例，即使存在空间，也不会放大 flex-shrink属性：定义了项目的缩小比例，当空间不足的情况下会等比例的缩小，如果定义个item的flow-shrink为0，则为不缩小 flex-basis属性：定义了在分配多余的空间，项目占据的空间。

flex：是flex-grow和flex-shrink、flex-basis的简写，默认值为0 1 auto。

align-self：允许单个项目与其他项目不一样的对齐方式，可以覆盖

align-items，默认属性为auto，表示继承父元素的align-items

比如说，用flex实现圣杯布局

## BFC（块级格式化上下文，用于清除浮动，防止margin 重叠等）

 直译成：块级格式化上下文，是一个独立的渲染区域，并且有一定的布局规则。

BFC区域不会与float box重叠

BFC是页面上的一个独立容器，子元素不会影响到外面计算BFC的高度时，浮动元素也会参与计算那些元素会生成BFC： (1)根元素

(2)float不为none的元素

(3)position为fixed和absolute的元素

(4)display为inline-block、table-cell、table-caption，flex，inline-flex

的元素

(5)overflow不为visible的元素



## 关于js动画和css3动画的差异性

 

渲染线程分为main thread和compositor thread，如果css动画只改变 transform和opacity，这时整个CSS动画得以在compositor trhead完成（而 js动画则会在main thread执行，然后出发compositor thread进行下一步操作），特别注意的是如果改变transform和opacity是不会layout或者paint的。

区别：

(1)功能涵盖面，js比css大

(2)实现/重构难度不一，CSS3比js更加简单，性能跳优方向固定

(3)对帧速表现不好的低版本浏览器，css3可以做到自然降级

(4)css动画有天然事件支持

(5)css3有兼容性问题

## 说一下块元素和行元素

块元素：独占一行，并且有自动填满父元素，可以设置margin和pading以及高度和宽度

行元素：不会独占一行，width和height会失效，并且在垂直方向的padding 和margin会失效。

## 多行元素的文本省略号



display: -webkit-box

-webkit-box-orient:vertical

-webkit-line-clamp:3 overflow:hidden

## visibility=hidden, opacity=0，display:none 

opacity=0，该元素隐藏起来了，但不会改变页面布局，并且，如果该元素已经绑定一些事件，如click事件，那么点击该区域，也能触发点击事件

visibility=hidden，该元素隐藏起来了，但不会改变页面布局，但是不会触发该元素已经绑定的事件

display=none，把元素隐藏起来，并且会改变页面布局，可以理解成在页面中把该元素删除掉一样。

## 双边距重叠问题（外边距折叠）

 多个相邻（兄弟或者父子关系）普通流的块元素垂直方向marigin会重叠折叠的结果为：

两个相邻的外边距都是正数时，折叠结果是它们两者之间较大的值。

两个相邻的外边距都是负数时，折叠结果是两者绝对值的较大值。

两个外边距一正一负时，折叠结果是两者的相加的和。

## position属性

- 固定定位fixed：
  - 元素的位置相对于浏览器窗口是固定位置，即使窗口是滚动的它也不会移动。
  - Fixed定位使元素的位置与文档流无关，因此不占据空间。Fixed定位的元素和其他元素重叠。
- 相对定位relative：
  - 如果对一个元素进行相对定位，它将出现在它所在的位置上。然后，可以通过设置垂直或水平位置，让这个元素"相对于"它的起点进行移动。 在使用相对定位时，无论是否进行移动，元素仍然占据原来的空间。因此，移动元素会导致它覆盖其它框。
- 绝对定位absolute：
  - 绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于<html>。 absolute 定位使元素的位置与文档流无关，因此不占据空间。 absolute 定位的元素和其他元素重叠。

- 粘性定位sticky：元素先按照普通文档流定位，然后相对于该元素在流中的flow root（BFC）和 containingblock（最近的块级祖先元素）定位。而后，元素定位表现为在跨越特定阈值前为相对定位，之后为固定定位。

- 默认定位Static：
  - 默认值。没有定位，元素出现在正常的流中（忽略top,bottom,left,right 或者 z-index 声明）。

- inherit:
  - 规定应该从父元素继承position 属性的值。

## 浮动清除

 

方法一：使用带clear属性的空元素

在浮动元素后使用一个空元素如`<div class="clear"></div>`，并在CSS中赋予`.clear{clear:both;}`属性即可清理浮动。亦可使用`<br class="clear" />`或`<hr class="clear" />来进行清理。`

方法二：使用CSS的overflow属性

给浮动元素的容器添加overflow:hidden;或overflow:auto;可以清除浮动，另外在 IE6 中还需要触发 hasLayout ，例如为父元素设置容器宽高或设置 zoom:1。

在添加overflow属性后，浮动元素又回到了容器层，把容器高度撑起，达到了清理浮动的效果。

方法三：给浮动的元素的容器添加浮动给浮动元素的容器也添加上浮动属性即可清除内部浮动，但是这样会使其整体浮动，影响布局，不推荐使用。

方法四：使用邻接元素处理

什么都不做，给浮动元素后面的元素添加clear属性。

方法五：使用CSS的:after伪元素

结合:after 伪元素（注意这不是伪类，而是伪元素，代表一个元素之后最近的元素）和 IEhack ，可以完美兼容当前主流的各大浏览器，这里的 IEhack 指的是触发 hasLayout。

给浮动元素的容器添加一个clearfix的class，然后给这个class添加一个:after伪元素实现元素末尾添加一个看不见的块元素（Block element）清理浮动。

## 怎么样让一个元素消失

display:none; visibility:hidden; opacity: 0; 等等

## 介绍一下盒模型 

CSS盒模型本质上是一个盒子，封装周围的HTML元素，它包括：边距，边框，填充，和实际内容。

标准盒模型：一个块的总宽度=width+margin(左右)+padding(左右)+border(左右)

怪异盒模型：一个块的总宽度=width+margin（左右）（既width已经包含了 padding和border值）

设置盒模型：box-sizing:border-box

## css动画如何实现

- animation：用于设置动画属性，他是一个简写的属性，包含6个属性

- transition：用于设置元素的样式过度，和animation有着类似的效果，但细节上有很大的不同

- transform：用于元素进行旋转、缩放、移动或倾斜，和设置样式的动画并没有什么关系

- translate：translate只是transform的一个属性值，即移动，除此之外还有 scale 等



创建动画序列，需要使用animation属性或其子属性，该属性允许配置动画时间、时长以及其他动画细节，但该属性不能配置动画的实际表现，动画的实际表现是由 \@keyframes规则实现，具体情况参见使用keyframes定义动画序列小节部分。 transition也可实现动画。transition强调过渡，是元素的一个或多个属性发生变化时产生的过渡效果，同一个元素通过两个不同的途径获取样式，而第二个途径当某种改变发生（例如hover）时才能获取样式，这样就会产生过渡动画。

## 如何实现图片在某个容器中居中的？

 父元素固定宽高，利用定位及设置子元素margin值为自身的一半。

父元素固定宽高，子元素设置position: absolute，margin：auto平均分配

margin

css3属性transform。子元素设置position: absolute; left: 50%; top:

50%;transform: translate(-50%,-50%);即可。

将父元素设置成display: table, 子元素设置为单元格 display: table-cell。

弹性布局display:flex。设置align-items:center;justify-content:center



## CSS3中对溢出的处理 todo

>  
>
>  cnkOhu
>
>  text-overflow属性，值为clip是修剪文本；
>
>  ellipsis为显示省略符号来表被修剪的文本； string为使用给定的字符串来代表被修剪的文本。 87.float的元素，display是什么
>
>  
>
>  display为block

## 隐藏页面中某个元素的方法

display:none; visibility:hidden; opacity: 0;

position移到外部，z-index涂层遮盖等等



## 什么是BFC

BFC也就是常说的块格式化上下文，这是一个独立的渲染区域，规定了内部如何布局，并且这个区域的子元素不会影响到外面的元素，其中比较重要的布局规则有内部box垂直放置，计算BFC的高度的时候，浮动元素也参与计算，触发BFC 的规则有根元素，浮动元素，position为absolute或fixed的元素，display 为inline-block，table-cell，table-caption，flex，inline-flex，overflow 不为visible的元素

## calc属性



Calc用户动态计算长度值，任何长度值都可以使用calc()函数计算，需要注意的是，运算符前后都需要保留一个空格，例如：width: calc(100% - 10px)；

## 有一个width300，height300，怎么实现在屏幕上垂直水平居中



对于行内块级元素

1）父级元素设置text-alig：center，然后设置line-height和vertical-align 使其垂直居中，最后设置font-size：0消除近似居中的bug 2）父级元素设置display：table-cell，vertical-align：middle达到水平垂直居中

1. 采用绝对定位，原理是子绝父相，父元素设置position：relative，子元素设置position：absolute，然后通过transform或margin组合使用达到垂直居中效果，设置top：50%，left：50%，transform：translate（-50%，-50%）
2. 绝对居中，原理是当top,bottom为0时，margin-top&bottom设置auto的话会无限延伸沾满空间并平分，当left，right为0时,margin-left&right设置auto会无限延伸占满空间并平分，
3. 采用flex，父元素设置display：flex，子元素设置margin：auto

视窗居中，vh为视口单位，50vh即是视口高度的50/100，设置margin：50vhauto

0，transform：translate(-50%)

## display：table和本身的table有什么区别

Display:table和本身table是相对应的，区别在于，display：table的css

声明能够让一个html元素和它的子节点像table元素一样，使用基于表格的css 布局，是我们能够轻松定义一个单元格的边界，背景等样式，而不会产生因为使用了table那样的制表标签导致的语义化问题。

之所以现在逐渐淘汰了table系表格元素，是因为用div+css编写出来的文件比用table边写出来的文件小，而且table必须在页面完全加载后才显示，div则是逐行显示，table的嵌套性太多，没有div简洁

## position属性的值有哪些及其区别



Position属性把元素放置在一个静态的，相对的，绝对的，固定的位置中.

Static：位置设置为static的元素，他始终处于页面流给予的位置，static元素会忽略任何top,buttom,left,right声明

Relative：位置设置为relative的元素，可将其移至相对于其正常位置的地方，因此left：20会将元素移至元素正常位置左边20个像素的位置

Absolute：此元素可定位于相对包含他的元素的指定坐标，此元素可通过left， top等属性规定

Fixed：位置被设为fiexd的元素，可定为与相对浏览器窗口的指定坐标，可以通过left，top，right属性来定位

## `position:absolute`和float属性的异同

共同点：对内联元素设置float和absolute属性，可以让元素**脱离文档流，并且可以设置其宽高**。
不同点：float仍会占据位置，absolute会覆盖文档流中的其他元素。



## z-index的定位方法

z-index属性设置元素的堆叠顺序，拥有更好堆叠顺序的元素会处于较低顺序元素之前，z-index可以为负，且z-index只能在定位元素上奏效，该属性设置一个定位元素沿z轴的位置，如果为正数，离用户越近，为负数，离用户越远，它的属性值有auto，默认，堆叠顺序与父元素相等，number，inherit，从父元素继承z-index属性的值

## CSS盒模型

CSS盒模型本质上是一个盒子，封装周围的HTML元素，它包括： 外边距（margin） 、 边框 

（border） 、 内边距（padding） 、 实际内容（content） 四个属性。 CSS盒模型：**标准模型** **+ IE****模型**

标准盒子模型：宽度=内容的宽度（content）+ border + padding

低版本IE盒子模型：宽度=内容宽度（content+border+padding），如何设置成 IE 盒子模型：`box-sizing: border-box;`

## 如果想要改变一个DOM元素的字体颜色，不在它本身上进行操作？

可以更改父元素的color

## 对CSS的新属性有了解过的吗？

CSS3的新特性中，在布局方面新增了flex布局，在选择器方面新增了例如

first-of-type,nth-child等选择器，在盒模型方面添加了box-sizing来改变盒模型，在动画方面增加了animation，2d变换，3d变换等，在颜色方面添加透明，rbga等，在字体方面允许嵌入字体和设置字体阴影，最后还有媒体查讯等

## line-height和height的区别

line-height一般是指布局里面一段文字上下行之间的高度，是针对字体来设置的，height一般是指容器的整体高度。

## 设置一个元素的背景颜色，背景颜色会填充哪些区域？

background-color设置的背景颜色会填充元素的content、padding、border区域。

## inline-block、inline和block的区别；为什么img 是inline还可以设置宽高



Block是块级元素，其前后都会有换行符，能设置宽度，高度，margin/padding水平垂直方向都有效。

Inline：设置width和height无效，margin在竖直方向上无效，padding在水平方向垂直方向都有效，前后无换行符

Inline-block：能设置宽度高度，margin/padding水平垂直方向 都有效，前后无换行符

## 了解重绘和重排吗，知道怎么去减少重绘和重排吗，让文档脱离文档流有哪些方法

DOM的变化影响到了预算内宿的几何属性比如宽高，浏览器重新计算元素的几何属性，其他元素的几何属性也会受到影响，浏览器需要重新构造渲染树，这个过程称之为重排，浏览器将受到影响的部分重新绘制在屏幕上 的过程称为重绘，引起重排重绘的原因有：

- 添加或者删除可见的DOM元素，

- 元素尺寸位置的改变

- 浏览器页面初始化，

- 浏览器窗口大小发生改变，重排一定导致重绘，重绘不一定导致重排.

减少重绘重排的方法有：

- 不在布局信息改变时做DOM查询，

- 使用csstext,className一次性改变属性

- 使用fragment

- 对于多次重排的元素，比如说动画。使用绝对定位脱离文档流，使其不影响其他元素

## CSS画正方体，三角形

画三角形：

​```css
#triangle02{ 
    width: 0; 
    height: 0;

	border-top: 50px solid blue; 
    border-right: 50px solid red;

	border-bottom: 50px solid green; 
    border-left: 50px solid yellow;

}
   ```

画正方体：

```html
<!DOCTYPE html>
<html lang="en">
<head>
<style>
} .side{ position: absolute; width: 2em; height: 2em; background: rgba(255,99,71,0.6); border: 1px solid rgba(0,0,0,0.5); color: white; text-align: center; line-height: 2em;

} .front{ transform:translateZ(1em); }

.bottom{

transform:rotateX(-90deg) translateZ(1em);

} .top{ transform:rotateX(90deg) translateZ(1em);

} .left{ transform:rotateY(-90deg) translateZ(1em);

} .right{ transform:rotateY(90deg) translateZ(1em);

} .back{ transform:translateZ(-1em); }

</style>

</head>

<body>

</div>

</div>

</div>

</div>

</body>

</html>
```

## overflow的原理

要讲清楚这个解决方案的原理，首先需要了解块格式化上下文，A block

块格式化上下文是CSS可视化渲染的

一部分，它是一块区域，规定了内部块盒 的渲染方式，以及浮动相互之间的影响关系；

当元素设置了overflow样式且值部位visible时，该元素就构建了一个BFC，

BFC在计算高度时，内部浮动元素的高度也要计算在内，也就是说技术BFC区域内只有一个浮动元素，BFC的高度也不会发生塌缩，所以达到了清除浮动的目的

## 清除浮动的方法

给要清除浮动的元素添加样式clear，父元素结束标签钱插入清除浮动的块级元素，给该元素添加样式clear 添加伪元素，在父级元素的最后，添加一个伪元素，通过清除伪元素的浮动，注意该伪元素的display为block，父元素添加样式overflow清除浮动，overflow设置除visible以外的任何位置

## box-sizing的语法和基本用处

box-sizing规定两个并排的带边框的框，语法为box-sizing： content-box/border-box/inherit

content-box：宽度和高度分别应用到元素的内容框，在宽度和高度之外绘制元素的内边距和边框

border-box：为元素设定的宽度和高度决定了元素的边框盒， inherit：继承父元素的box-sizing

## 使元素消失的方法有哪些？/怎么隐藏一个元素



1. opacity：0，该元素隐藏起来了，但不会改变页面布局，并且，如果该元素已经绑定一些事件，如click事件，那么点击该区域，也能触发点击事件
2. visibility：hidden，该元素隐藏起来了，但不会改变页面布局，但是不会触发该元素已经绑定的事件
3. display：none，把元素隐藏起来，并且会改变页面布局，可以理解成在页面中把该元素删除掉。

## 两个嵌套的div，position都是absolute，子div设置 top属性，那么这个top是相对于父元素的哪个位置定位的

margin的外边缘

## 说说盒子模型

CSS盒模型本质上是一个盒子，封装周围的HTML元素，它包括：边距，边框，填充，和实际内容。

标准盒模型：一个块的总宽度=width+margin(左右)+padding(左右)+border(左右)

怪异盒模型：一个块的总宽度=width+margin（左右）（既width已经包含了 padding和border值）

如何设置：box-sizing:border-box

## display

主要取值有none,block,inline-block,inline,flex等。

## 相对布局和绝对布局，position:relative和obsolute。



相对定位relative：

如果对一个元素进行相对定位，它将出现在它所在的位置上。然后，可以通过设置垂直或水平位置，让这个元素"相对于"它的起点进行移动。 在使用相对定位时，无论是否进行移动，元素仍然占据原来的空间。因此，移动元素会导致它覆盖其它框。

绝对定位absolute：

绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于<html>。 absolute 定位使元素的位置与文档流无关，因此不占据空间。 absolute 定位的元素和其他元素重叠。

##  flex布局



flex 是 Flexible Box 的缩写，意为"弹性布局"。指定容器display: flex即可。

容器有以下属性：flex-direction，flex-wrap，flex-flow，justify-content， align-items，align-content。

flex-direction属性决定主轴的方向；

flex-wrap属性定义，如果一条轴线排不下，如何换行；

flex-flow属性是flex-direction属性和flex-wrap属性的简写形式，默认值为row nowrap；

justify-content属性定义了项目在主轴上的对齐方式。

align-items属性定义项目在交叉轴上如何对齐。

align-content属性定义了多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用。

项目（子元素）也有一些属性：order，flex-grow，flex-shrink，flex-basis， flex，align-self。

order属性定义项目的排列顺序。数值越小，排列越靠前，默认为0。

flex-grow属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。

flex-shrink属性定义了项目的缩小比例，默认为1，即如果空间不足，该项目将缩小。

flex-basis属性定义了在分配多余空间之前，项目占据的主轴空间（mainsize）。

flex属性是flex-grow, flex-shrink 和 flex-basis的简写，默认值为0 1 auto。后两个属性可选。

align-self属性允许单个项目有与其他项目不一样的对齐方式，可覆盖

align-items属性。默认值为auto，表示继承父元素的align-items属性，如果没有父元素，则等同于stretch。

## block、inline、inline-block的区别

block元素会独占一行，多个block元素会各自新起一行。默认情况下，block 元素宽度自动填满其父元素宽度。

block元素可以设置width,height属性。块级元素即使设置了宽度,仍然是独占一行。

block元素可以设置margin和padding属性。

inline元素不会独占一行，多个相邻的行内元素会排列在同一行里，直到一行排列不下，才会新换一行，其宽度随元素的内容而变化。

inline元素设置width,height属性无效。

inline元素的margin和padding属性，水平方向的padding-left,

padding-right, margin-left, margin-right都产生边距效果；但竖直方向的 padding-top, padding-bottom, margin-top, margin-bottom不会产生边距效果。

inline-block：简单来说就是将对象呈现为inline对象，但是对象的内容作为 block对象呈现。之后的内联对象会被排列在同一行内。比如我们可以给一个

link（a元素）inline-block属性值，使其既具有block的宽度高度特性又具有 inline的同行特性。

## css布局

六种布局方式总结：圣杯布局、双飞翼布局、Flex布局、绝对定位布局、表格布局、网格布局。圣杯布局是指布局从上到下分为header、container、footer，然后container 部分定为三栏布局。这种布局方式同样分为header、container、footer。圣杯布局的缺陷在于 center 是在 container 的padding中的，因此宽度小的时候会出现混乱。

双飞翼布局给center 部分包裹了一个 main 通过设置margin主动地把页面撑开。

Flex布局是由CSS3提供的一种方便的布局方式。

绝对定位布局是给container 设置position: relative和overflow: hidden，因为绝对定位的元素的参照物为第一个postion不为static的祖先元素。left 向左浮动，right 向右浮动。center 使用绝对定位，通过设置left和right 并把两边撑开。 center 设置top: 0和bottom: 0使其高度撑开。

表格布局的好处是能使三栏的高度统一。

网格布局可能是最强大的布局方式了，使用起来极其方便，但目前而言，兼容性并不好。网格布局，可以将页面分割成多个区域，或者用来定义内部元素的大小，位置，图层关系。

## css定位

固定定位fixed：元素的位置相对于浏览器窗口是固定位置，即使窗口是滚动的它也不会移动。

Fixed定位使元素的位置与文档流无关，因此不占据空间。Fixed定位的元素和其他元素重叠。

相对定位relative：

如果对一个元素进行相对定位，它将出现在它所在的位置上。然后，可以通过设置垂直或水平位置，让这个元素"相对于"它的起点进行移动。 在使用相对定位时，无论是否进行移动，元素仍然占据原来的空间。因此，移动元素会导致它覆盖其它框。

绝对定位absolute：

绝对定位的元素的位置相对于最近的已定位父元素，如果元素没有已定位的父元素，那么它的位置相对于<html>。 absolute 定位使元素的位置与文档流无关，因此不占据空间。 absolute 定位的元素和其他元素重叠。

粘性定位sticky：

元素先按照普通文档流定位，然后相对于该元素在流中的flow root（BFC）和 containingblock（最近的块级祖先元素）定位。而后，元素定位表现为在跨越特定阈值前为相对定位，之后为固定定位。

默认定位Static：

默认值。没有定位，元素出现在正常的流中（忽略top,bottom,left,right 或者 z-index 声明）。

inherit:

规定应该从父元素继承position 属性的值。

## relative定位规则

如果对一个元素进行相对定位，它将出现在它所在的位置上。然后，可以通过设置垂直或水平位置，让这个元素"相对于"它的起点进行移动。 在使用相对定位时，无论是否进行移动，元素仍然占据原来的空间。因此，移动元素会导致它覆盖其它框。 

## 垂直居中

父元素固定宽高，利用定位及设置子元素margin值为自身的一半。

父元素固定宽高，子元素设置position: absolute，margin：auto平均分配margin

css3属性transform。子元素设置position: absolute; left: 50%; top:

50%;transform: translate(-50%,-50%);即可。

将父元素设置成display: table, 子元素设置为单元格 display: table-cell。弹性布局display: flex。设置align-items: center; justify-content: center;

## css预处理器有什么

less，sass等

## 如何画一个三角形

 

三角形原理：边框的均分原理

```css
div {

width:0px; height:0px; border-top:10px solid red; border-right:10px solid transparent; border-bottom:10px solid transparent; border-left:10px solid transparent; }
```

## 那些CSS属性可以继承

可继承： font-size font-family color, ul li dl dd dt; 

不可继承 ：border padding margin width height ;



# 第三章javascript

## js的数据类型

基本类型：Number、Boolean、String、null、undefined、symbol（ES6 新增的），

BigInt（ES2020） 引用类型：Object，对象子类型（Array，Function）



## js有哪些内置对象 

Object 是 JavaScript中所有对象的父对象数据封装类对象： Object 、 Array 、 Boolean 、 Number 和 String 

其他对象： Function 、 Arguments 、 Math 、 Date 、 RegExp 、 Error



## 判断一个对象不是空对象

Object.keys(obj).length === 0

## symbol有什么用处 

可以用来表示一个独一无二的变量防止命名冲突。但是面试官问还有吗？我没想出其他的用处就直接答我不知道了，还可以利用 symbol 不会被常规的方法（除了 Object.getOwnPropertySymbols 外）遍历到，所以可以用来模拟私有变量。

主要用来提供遍历接口，布置了 symbol.iterator 的对象才可以使用 for···of 循环，可以统一处理数据结构。调用之后回返回一个遍历器对象，包含有一个 next 方法，使用 next 方法后有两个返回值 value 和 done 分别表示函数当前执行位置的值和是否遍历完毕。

Symbol.for() 可以在全局访问 symbol

## null，undefined 的区别 

> undefined 表示不存在这个值。
>
> undefined :是一个表示\"无\"的原始值或者说表示\"缺少值\"，就是此处应该有一个值，但是还没有定义。尝试读取时会返回 undefined
>
> 例如变量被声明了，但没有赋值时，就等于 undefined null 表示一个对象被定义了，值为"空值"
>
> null : 是一个对象(空对象, 没有任何属性和方法)
>
> 例如作为函数的参数，表示该函数的参数不是对象；
>
> 在验证 null 时，一定要使用 === ，因为 == 无法分别 null 和 undefined

## 0.1+0.2 === 0.3？

JavaScirpt 使用 Number 类型来表示数字（整数或浮点数），遵循 IEEE 754 标准，通过 64 位来表示一个数字（1 + 11 + 52）

1 符号位，0 表示正数，1 表示负数 s

11 指数位（e）

52 尾数，小数部分（即有效数字）

最大安全数字：Number.MAX_SAFE_INTEGER = Math.pow(2, 53) - 1，转换成整数就是 16 位，所以0.1 === 0.1，是因为通过 toPrecision(16) 去有效位之后，两者是相等的。

在两数相加时，会先转换成二进制，0.1 和 0.2 转换成二进制的时候尾数会发生无限循环，然后进行对阶运算，JS 引擎对二进制进行截断，所以造成精度丢失。

**精度丢失可能出现在进制转换和对阶运算中**

## 什么是函数柯里化?

是把接受多个参数的函数变换成接受一个单一参数（最初函数的第一个参数）的函数，并且返回接受余下的参数而且返回结果的新函数的技术。

指将一个函数从可调用的 f(a, b, c) 转换为可调用的 f(a)(b)(c)。

柯里化不会调用函数。它只是对函数进行转换。

```js
function createCurry(func,args){
    var argity = func.length;
    var args = args || [];
    return function(){
        var _args = [].slice.apply(arguments);
        args.push(...args);

        if(args.length<argity){
            return createCurry.call(this,func,args);
        }
        return func.apply(this,args);
    }
}
```



https://zh.javascript.info/currying-partials

## 创建对象有几种方法？

1. 工厂模式

   用函数来封装特定接口创建对象

   ```javascript
   function createPerson(name,age,job){
   	var o = new Object();
       o.name = name;
       o.age = age;
       o.job = job;
       o.sayName = function(){
           alert(this.name);
       };
       return o;
   }
   var person1 = createPerson("lucy",22,"engineer");
   ```

   

2. 构造函数模式

   与工厂模式的区别在于，`new Object()`是在函数外进行的.

   - 没有显式地创建对象
   - 直接将属性和方法赋予this对象
   - 没有return语句

   ```javascript
   function Person(name,age,job){
       this.name = name;
       this.age = age;
       this.job = job;
       this.sayName = function(){
           alert(this.name);
       };
   }
   var person1 = new Person("lucy",22,"engineer");
   ```

   必须使用new操作符。

   创建步骤：

   1. 创建一个新对象
   2. 将构造函数的作用域赋予新对象
   3. 执行构造函数中的代码
   4. 返回新对象

   存在的问题：每个方法都要在实例上创建一遍。

3. 原型模式

   ```javascript
   function Person(){
           }
           
   Person.prototype.name = "Nicholas";
   Person.prototype.age = 29;
   Person.prototype.job = "Software Engineer";
   Person.prototype.sayName = function(){
       alert(this.name);
   };
   
   var person1 = new Person();
   person1.sayName();   //"Nicholas"
   
   var person2 = new Person();
   person2.sayName();   //"Nicholas"
         
   ```

   

4. 组合使用构造函数和原型模式

   构造函数模式用来定义实例属性，原型模式用来定义方法和共享的属性。

   每个实例都会有一份实例属性的副本，也共享方法的引用，最大限度节省内存。也支持向构造函数传递参数。

   ```javascript
   function Person(name, age, job){
       this.name = name;
       this.age = age;
       this.job = job;
       this.friends = ["Shelby", "Court"];
   }
   
   Person.prototype = {
       constructor: Person,
       sayName : function () {
           alert(this.name);
       }
   };
   
   var person1 = new Person("Nicholas", 29, "Software Engineer");
   var person2 = new Person("Greg", 27, "Doctor");
   
   person1.friends.push("Van");
   ```

   

5. 动态原型模式

   ```javascript
   function Person(name, age, job){
           
       //properties
       this.name = name;
       this.age = age;
       this.job = job;
   
       //methods
       if (typeof this.sayName != "function"){
   
           Person.prototype.sayName = function(){
               alert(this.name);
           };
   
       }
   }
   
   var friend = new Person("Nicholas", 29, "Software Engineer");
   friend.sayName();
   
   ```

   

6. 寄生构造函数模式

7. 稳妥构造函数模式

## 怎样通过ES5及ES6声明一个类？

http://caibaojian.com/es6/class.html

ES5：

JavaScript语言的传统方法是通过构造函数，定义并生成新对象。下面是一个例子。

```javascript
function Point(x, y) {
  this.x = x;
  this.y = y;
}

Point.prototype.toString = function () {
  return '(' + this.x + ', ' + this.y + ')';
};

var p = new Point(1, 2);
```

ES6：引入class的概念

```javascript
class Point {
  constructor(x, y) {
    this.x = x;
    this.y = y;
  }

  toString() {
    return '(' + this.x + ', ' + this.y + ')';
  }
}
```



## ES5和ES6继承的区别

1. ES5 的继承实质上是先创建子类的实例对象，然后再将父类的方法添加 到 this 上（Parent.apply(this)）. 
2. ES6 的继承机制完全不同，实质上是先创建父类的实例对象 this（所以必 须先调用父类的 super()方法），然后再用子类的构造函数修改 this。
3. ES5 的继承时通过原型或构造函数机制来实现。 
4. ES6 通过 class 关键字定义类，里面有构造方法，类之间通过 extends 关 键字实现继承。
5. 子类必须在 constructor 方法中调用 super 方法，否则新建实例报错。因 为子类没有自己的 this 对象，而是继承了父类的 this 对象，然后对其进行加工。 如果不调用 super 方法，子类得不到 this 对象。
6. 注意 super 关键字指代父类的实例，即父类的 this 对象。
7. 注意：在子类构造函数中，调用 super 后，才可使用 this 关键字，否则 报错。 



## let,const,var

三者的区别： 

- var 和 let 用以声明变量，const 用于声明只读的常量；
- var 声明的变量，不存在块级作用域，在全局范围内都有效，let 和 const 声明的，只在它所在的代码块内有效；
- let 和 const 不存在像 var 那样的 “变量提升” 现象，所以 var 定义变 量可以先使用，后声明，而 let 和 const 只可先声明，后使用；
- let 声明的变量存在暂时性死区，即只要块级作用域中存在 let，那么它 所声明的变量就绑定了这个区域，不再受外部的影响。
- let 不允许在相同作用域内，重复声明同一个变量； 
- const 在声明时必须初始化赋值，一旦声明，其声明的值就不允许改变， 更不允许重复声明；如 const 声明了一个复合类型的常量，其存储的是一个引 用地址，不允许改变的是这个地址，而对象本身是可变的。

 变量与内存之间的关系，主要由三个部分组成：

- 变量名
- 内存地址
- 内存空间

JS 引擎在读取变量时，先找到变量绑定的内存地址，然后找到地址所指向的内存空间，最后读取其中的内容。当变量改变时，JS 引擎不会用新值覆盖之前旧 值的内存空间（虽然从写代码的角度来看，确实像是被覆盖掉了），而是重新 分配一个新的内存空间来存储新值，并将新的内存地址与变量进行绑定，JS 引 擎会在合适的时机进行 GC，回收旧的内存空间。 const 定义变量（常量）后，变量名与内存地址之间建立了一种不可变的绑定 关系，阻隔变量地址被改变，当 const 定义的变量进行重新赋值时，根据前面 的论述，JS 引擎会尝试重新分配新的内存空间，所以会被拒绝，便会抛出异常。

```js
for(var i = 0;i<10;i++){
    setTimeout(() =>{console.log(i);},1000)
}//10,10,10,10,10,10,10,10,10,10


for(let i = 0;i<10;i++){
    setTimeout(() =>{console.log(i);},1000)
}//0,1,2,3,4,5,6,7,8,9

for(var i = 0;i<10;i++){
    ((i) => {
        setTimeout(() =>{console.log(i);},1000)(i)
    })
}//0,1,2,3,4,5,6,7,8,9
```



## 变量提升

函数在运行的时候，会首先创建执行上下文，然后将执行上下文入栈，然后当此执行上下文处于栈顶时，开始运行执行上下文。

在创建执行上下文的过程中会做三件事：**创建变量对象，创建作用域链，确定 this 指向，**其中创建变量对象的过程中，首先会为 arguments 创建一个属性，值为 arguments，然后会扫码 function 函数声明，创建一个同名属性，值为函数的引用，接着会扫码 var 变量声明，创建一个同名属性，值为undefined，这就是变量提升 。

## call、apply的共同点与区别?

https://zh.javascript.info/call-apply-decorators#zong-jie

- [func.call(context, arg1, arg2…)](https://developer.mozilla.org/zh/docs/Web/JavaScript/Reference/Global_Objects/Function/call) —— 用给定的上下文和参数调用 `func`。
- [func.apply(context, args)](https://developer.mozilla.org/zh/docs/Web/JavaScript/Reference/Global_Objects/Function/apply) —— 调用 `func` 将 `context` 作为 `this` 和类数组的 `args` 传递给参数列表。

参数传递不一样。call需要一个个传递参数，apply可以传递参数的列表

- Function.prototype.apply 和 Function.prototype.call 的作用是一样的，区别在于传入参数的不同；
- 第一个参数都是，指定函数体内 this 的指向；
- 第二个参数开始不同，apply 是传入带下标的集合，数组或者类数组， apply 把它传给函数作为参数，call 从第二个开始传入的参数是不固定的，都会 传给函数作为参数。
- call 比 apply 的性能要好，平常可以多用 call, call 传入参数的格式正是内 部所需要的格式



## JavaScript原型，原型链 ? 有什么特点？ 

每个对象都会在其内部初始化一个属性，就是 prototype (原型)，当我们访问一个对象的属性时, 如果这个对象内部不存在这个属性，那么他就会去 prototype 里找这个属性，这个prototype 又会有自己的 prototype ，于是就这样一直找下去，也就是我们平时所说的原型链的概念

关系： instance.constructor.prototype = instance.\_\*proto\*\_

特点：JavaScript 对象是通过引用来传递的，我们创建的每个新对象实体中并没有一份属于自己

的原型副本。当我们修改原型时，与之相关的对象也会继承这一改变当我们需要一个属性的时， Javascript 引擎会先看当前对象中是否有这个属性， 如果没有的,就会查找他的 Prototype 对象是否有这个属性，如此递推下去，一直检索到 Object内建对象

## 用javascript实现对象的继承,继承的几种方式,这几种方式的优缺点?

- 原型链

  - 重温一下构造函数、原型和实例的关系：每个构造函数都有一个原型对象，原型有一个属性指回构造函数，而实例有一个内部指针指向原型。如果原型是另一个类型的实例呢？那就意味着这个原型本身有一个内部指针指向另一个原型，相应地另一个原型也有一个指针指向另一个构造函数。这样就在实例和原型之间构造了一条原型链。这就是原型链的基本构想。

  - ```js
    function SuperType() {
      this.property = true;
    }
               
    SuperType.prototype.getSuperValue = function() {
      return this.property;
    };
               
    function SubType() {
      this.subproperty = false;
    }
               
    // inherit from SuperType
    SubType.prototype = new SuperType();
               
    // new method
    SubType.prototype.getSubValue = function () {
      return this.subproperty;
    };
               
    // override existing method
    SubType.prototype.getSuperValue = function () {
      return false;
    };
               
    let instance = new SubType();
    console.log(instance.getSuperValue());   // false
    ObjectMethodExample01.js
    In this code, the highlighted area shows two methods. The first is getSubValue(), which is a new method on the SubType. The second is getSuperValue(), which already exists in the prototype chain but is being shadowed here. When getSuperValue() is called on an instance of SubType, it will call this one, but instances of SuperType will still call the original. The important thing to note is that both of the methods are defined after the prototype has been assigned as an instance of SuperType.
    
    ```

  - 

- 构造函数

  - 

- 组合继承

  - ```js
    function SuperType(name){
      this.name = name;
      this.colors = ["red", "blue", "green"];
    }
               
    SuperType.prototype.sayName = function() {
      console.log(this.name);
    };
               
    function SubType(name, age){  
      // inherit properties
      SuperType.call(this, name);
      
      this.age = age;
    }
               
    // inherit methods
    SubType.prototype = new SuperType();
               
    SubType.prototype.sayAge = function() {
      console.log(this.age);
    };
               
    let instance1 = new SubType("Nicholas", 29);
    instance1.colors.push("black");
    console.log(instance1.colors);  // "red,blue,green,black"
    instance1.sayName();            // "Nicholas";
    instance1.sayAge();             // 29
               
    let instance2 = new SubType("Greg", 27);
    console.log(instance2.colors);  // "red,blue,green"
    instance2.sayName();            // "Greg";
    instance2.sayAge();             // 27
    ```

  - 

- 原型式继承

  - ```js
    function object(o) {
      function F() {}
      F.prototype = o;
      return new F();
    }
    //The object() function creates a temporary constructor, assigns a given object as the constructor’s prototype, and returns a new instance of the temporary type. Essentially, object() performs a shadow copy of any object that is passed into it. Consider the following:
    let person = {
      name: "Nicholas",
      friends: ["Shelby", "Court", "Van"]
    };
               
    let anotherPerson = object(person);
    anotherPerson.name = "Greg";
    anotherPerson.friends.push("Rob");
               
    let yetAnotherPerson = object(person);
    yetAnotherPerson.name = "Linda";
    yetAnotherPerson.friends.push("Barbie");
               
    console.log(person.friends);   // "Shelby,Court,Van,Rob,Barbie"
    PrototypalInheritanceExample01.js
    
    ```

  - 

- 寄生式继承

  - ```js
    function createAnother(original){
      let clone = object(original);  // create a new object by calling a function
      clone.sayHi = function() {     // augment the object in some way
        console.log("hi");
      };
      return clone;           // return the object
    }
    let person = {
      name: "Nicholas",
      friends: ["Shelby", "Court", "Van"]
    };
               
    let anotherPerson = createAnother(person);
    anotherPerson.sayHi();  // "hi"
    
    ```

  - 

- 寄生式组合继承

  - ```js
    function SuperType(name) {
      this.name = name;
      this.colors = ["red", "blue", "green"];
    }
               
    SuperType.prototype.sayName = function() {
      console.log(this.name);
    };
               
    function SubType(name, age){  
      SuperType.call(this, name);      // second call to SuperType()
      
      this.age = age;
    }
               
    SubType.prototype = new SuperType();   // first call to SuperType()
    SubType.prototype.constructor = SubType;           
    SubType.prototype.sayAge = function() {
      console.log(this.age);
    };
    ParasiticCominationInheritanceExample01.js
    
    ```

  - 



## 谈一谈this在各种情况的指向问题？

你不知道的JavaScript上

- 默认绑定
- 隐式绑定
- 显式绑定
- new绑定



## 几个很实用的BOM属性对象方法?

什么是Bom? Bom是浏览器对象。有哪些常用的Bom属性呢？

- (1)location对象
  - location.href-- 返回或设置当前文档的URL location.search -- 返回URL中的查询字符串部分。例如 http://www.dreamdu.com/dreamdu.php?id=5&name=dreamdu 返回包括(?) 后面的内容?id=5&name=dreamdu
  - location.hash -- 返回URL#后面的内容，如果没有#，返回空 location.host -- 返回URL中的域名部分，例如[www.dreamdu.com](www.dreamdu.com)
  - location.hostname -- 返回URL中的主域名部分，例如dreamdu.com
  - location.pathname -- 返回URL的域名后的部分。例如 http://www.dreamdu.com/xhtml/ 返回/xhtml/
  - location.port -- 返回URL中的端口部分。例如 http://www.dreamdu.com:8080/xhtml/ 返回8080
  - location.protocol -- 返回URL中的协议部分。例如 http://www.dreamdu.com:8080/xhtml/ 返回(//)前面的内容http:
  - location.assign -- 设置当前文档的URL location.replace() -- 设置当前文档的URL，并且在history对象的地址列表中移除这个URL 
  - location.replace(url); location.reload() -- 重载当前页面

- (2)history对象 
  - history.go() -- 前进或后退指定的页面数
  - history.go(num); history.back() -- 后退一页 
  - history.forward() -- 前进一页

- (3)Navigator对象
  - navigator.userAgent -- 返回用户代理头的字符串表示(就是包括浏览器版本信息等的字符串)
  - navigator.cookieEnabled -- 返回浏览器是否支持(启用)cookie





## 讲讲viewport和移动端布局 todo

 

前端开发中，静态网页通常需要适应不同分辨率的设备，常用的自适应解决方案包括媒体查询、百分比、rem和vw/vh等。下面从px单位出发，分析px在移动端布局中的不足，接着介绍几种不同的自适应解决方案。

- px和视口
- 媒体查询
- 百分比
- 自适应场景下的rem解决方案
- 通过vw/vh来实现自适应

一、px和视口

1. 像素

像素是网页布局的基础，一个像素表示了计算机屏幕所能显示的最小区域像素分为两种类型：css像素和物理像素。

我们在js或者css代码中使用的px单位就是指的是css像素，物理像素也称设备像素，只与设备或者说硬件有关，同样尺寸的屏幕，设备的密度越高，物理像素也就越多。

下表表示css像素和物理像素的具体区别： css像素 为web开发者提供，在css中使用的一个抽象单位

物理像素 只与设备的硬件密度有关，任何设备的物理像素都是固定的

那么css像素与物理像素的转换关系是怎么样的呢？

为了明确css像素和物理像素的转换关系，必须先了解视口是什么。

1. 视口

广义的视口，是指浏览器显示内容的屏幕区域，狭义的视口包括了布局视口、视觉视口和理想视口

(1)布局视口（layoutviewport）

布局视口定义了pc网页在移动端的默认布局行为，因为通常pc的分辨率较大，布局视口默认为980px。也就是说在不设置网页的viewport的情况下，pc端的网页默认会以布局视口为基准，在移动端进行展示。因此我们可以明显看出来，默认为布局视口时，根植于pc端的网页在移动端展示很模糊。

(2)视觉视口（visualviewport）

视觉视口表示浏览器内看到的网站的显示区域，用户可以通过缩放来查看网页的显示内容，从而改变视觉视口。视觉视口的定义，就像拿着一个放大镜分别从不同距离观察同一个物体，视觉视口仅仅类似于放大镜中显示的内容，因此视觉视口不会影响布局视口的宽度和高度。

(3)理想视口（idealviewport）

理想视口或者应该全称为"理想的布局视口"，在移动设备中就是指设备的分辨率。换句话说，理想视口或者说分辨率就是给定设备物理像素的情况下，最佳的"布局视口"。

上述视口中，最重要的是要明确理想视口的概念，在移动端中，理想视口或者说分辨率跟物理像素之间有什么关系呢？

为了理清分辨率和物理像素之间的联系，我们介绍一个用DPR（Device pixel ratio）设备像素比来表示，则可以写成：

DPR = 物理像素／分辨率在不缩放的情况下，一个css像素就对应一个dpr，也就是说，在不缩放 CSS像素 = 物理像素／分辨率

此外，在移动端的布局中，我们可以通过viewport元标签来控制布局，比如一般情况下，我们可以通过下述标签使得移动端在理想视口下布局：

上述meta标签的每一个属性的详细介绍如下：

  属性名          取值       描述

  width           正整数     定义布局视口的宽度，单位为像素  height          正整数     定义布局视口的高度，单位为像素，很少使用  initial-scale   [0,10]   初始缩放比例，1表示不缩放  minimum-scale   [0,10]   最小缩放比例  maximum-scale   [0,10]   最大缩放比例  user-scalable   yes／no    是否允许手动缩放页面，默认值为yes

其中我们来看width属性，在移动端布局时，在meta标签中我们会将width设

置称为device-width，device-width一般是表示分辨率的宽，通过 width=device-width的设置我们就将布局视口设置成了理想的视口。

3）px与自适应上述我们了解到了当通过viewport元标签，设置布局视口为理想视口时，1个 css像素可以表示成：

CSS像素 = 物理像素／分辨率

我们直到，在pc端的布局视口通常情况下为980px，移动端以iphone6为例，分辨率为375* 667，也就是说布局视口在理想的情况下为375px。

比如现在我们有一个750px*1134px的视觉稿，那么在pc端，一个css像素可以如下计算：

PC端：CSS像素 = 物理像素／分辨率 = 750 ／ 980 =0.76 px 而在iphone6下：

iphone6：CSS像素 = 物理像素 ／分辨率 = 750 ／ 375 = 2 px

也就是说在PC端，一个CSS像素可以用0.76个物理像素来表示，而iphone6 中 一个CSS像素表示了2个物理像素。此外不同的移动设备分辨率不同，也就是1个CSS像素可以表示的物理像素是不同的，因此如果在css中仅仅通过px 作为长度和宽度的单位，造成的结果就是无法通过一套样式，实现各端的自适应。

二、媒体查询

在前面我们说到，不同端的设备下，在css文件中，1px所表示的物理像素的大小是不同的，因此通过一套样式，是无法实现各端的自适应。由此我们联想：如果一套样式不行，那么能否给每一种设备各一套不同的样式来实现自适应的效果？

答案是肯定的。

使用[\@media](https://github.com/media)媒体查询可以针对不同的媒体类型定义不同的样式，特别是响应式页面，可以针对不同屏幕的大小，编写多套样式，从而达到自适应的效果。

举例来说：

```css
\@media screen and (max-width: 960px){

body{

background-color:#FF6699

}

}

\@media screen and (max-width: 768px){ body{

background-color:#00FF66;

}

}

\@media screen and (max-width: 550px){ body{

background-color:#6633FF;

}

}

\@media screen and (max-width: 320px){ body{

background-color:#FFFF00;

}

}
```





上述的代码通过媒体查询定义了几套样式，通过max-width设置样式生效时的最

大分辨率，上述的代码分别对分辨率在0～320px，320px～550px，550px～768px

以及768px～960px的屏幕设置了不同的背景颜色。

通过媒体查询，可以通过给不同分辨率的设备编写不同的样式来实现响应式的布局，比如我们为不同分辨率的屏幕，设置不同的背景图片。比如给小屏幕手机设置[\@2x](https://github.com/2x)图，为大屏幕手机设置[\@3x](https://github.com/3x)图，通过媒体查询就能很方便的实现。但是媒体查询的缺点也很明显，如果在浏览器大小改变时，需要改变的样式太多，那么多套样式代码会很繁琐。

三、百分比除了用px结合媒体查询实现响应式布局外，我们也可以通过百分比单位" % " 来实现响应式的效果。

比如当浏览器的宽度或者高度发生变化时，通过百分比单位，通过百分比单位可以使得浏览器中的组件的宽和高随着浏览器的变化而变化，从而实现响应式的效果。

为了了解百分比布局，首先要了解的问题是：

css中的子元素中的百分比（%）到底是谁的百分比？

直观的理解，我们可能会认为子元素的百分比完全相对于直接父元素，height 百分比相对于height，width百分比相对于width。当然这种理解是正确的，但是根据css的盒式模型，除了height、width属性外，还具有padding、border、 margin等等属性。那么这些属性设置成百分比，是根据父元素的那些属性呢？此外还有border-radius和translate等属性中的百分比，又是相对于什么呢？下面来具体分析。

1）百分比的具体分析

（1）子元素height和width的百分比

子元素的height或width中使用百分比，是相对于子元素的直接父元素，width 相对于父元素的width，height相对于父元素的height。

比如：`</div>`

如果设置：

```
.father{

width:200px; height:100px;

}

.child{

width:50%; height:50%; }
```





(2)top和bottom、left和right

子元素的top和bottom如果设置百分比，则相对于直接非static定位(默认定位)的父元素的高度，同样子元素的left和right如果设置百分比，则相对于直接非static定位(默认定位的)父元素的宽度。

（3）padding

子元素的padding如果设置百分比，不论是垂直方向或者是水平方向，都相对于直接父亲元素的width，而与父元素的height无关。

举例来说：

.parent{ width:200px; height:100px; background:green;}

.child{ width:0px; height:0px; background:blue; color:white; padding-top:50%; padding-left:50%;}

子元素的初始宽高为0，通过padding可以将父元素撑大，上图的蓝色部分是一个正方形，且边长为100px,说明padding不论宽高，如果设置成百分比都相对于父元素的width。

1. margin

> 跟padding一样，margin也是如此，子元素的margin如果设置成百分比，不论是垂直方向还是水平方向，都相对于直接父元素的width。这里就不具体举例。

1. border-radius

> border-radius不一样，如果设置border-radius为百分比，则是相对于自身的宽度，
>
> 举例来说：

<div class="trangle"></div> 设置border-radius为百分比：

.trangle{ width:100px; height:100px;

border-radius:50%; background:blue; margin-top:10px;

}

除了border-radius外，还有比如translate、background-size等都是相对于自身的，这里就不一一举例。

2）百分比单位布局应用

百分比单位在布局上应用还是很广泛的，这里介绍一种应用。

比如我们要实现一个固定长宽比的长方形，比如要实现一个长宽比为4:3的长方形,我们可以根据padding属性来实现，因为padding不管是垂直方向还是水平方向，百分比单位都相对于父元素的宽度，因此我们可以设置padding-top为百分比来实现

长宽自适应的长方形：

<div class="trangle"></div> 设置样式让其自适应：

.trangle{ height:0;

width:100%;

padding-top:75%;

}

通过设置padding-top：75%,相对比宽度的75%，因此这样就设置了一个长宽高恒定比例的长方形，具体效果展示如下：

3）百分比单位缺点

从上述对于百分比单位的介绍我们很容易看出如果全部使用百分比单位来实现响应式的布局，有明显的以下两个缺点：

1. 计算困难，如果我们要定义一个元素的宽度和高度，按照设计稿，必须换算成百分比单位。
2. 从小节1可以看出，各个属性中如果使用百分比，相对父元素的属性并不是唯一的。

比如width和height相对于父元素的width和height，而margin、padding不管垂直还是水平方向都相对比父元素的宽度、border-radius则是相对于元素自身等等，造成我们使用百分比单位容易使布局问题变得复杂。

四、自适应场景下的rem解决方案

1. rem单位

首先来看，什么是rem单位。

rem是一个灵活的、可扩展的单位，由浏览器转化像素并显示。与em单位不同，

rem单位无论嵌套层级如何，都只相对于浏览器的根元素（HTML元素）的 font-size。默认情况下，html元素的font-size为16px，

所以：rem = 16px 为了计算方便，通常可以将html的font-size设置成： html{ font-size: 62.5%

}

这种情况下：rem = 10px

1. 通过rem来实现响应式布局 rem单位都是相对于根元素html的font-size来决定大小的,根元素的 font-size相当于提供了一个基准，当页面的size发生变化时，只需要改变 font-size的值，那么以rem为固定单位的元素的大小也会发生响应的变化。因此，如果通过rem来实现响应式的布局，只需要根据视图容器的大小，动态的

改变font-size即可。

function refreshRem() { var docEl = doc.documentElement; var width = docEl.getBoundingClientRect().width; var rem = width / 10; docEl.style.fontSize = rem + 'px'; flexible.rem = win.rem = rem;

}

win.addEventListener('resize', refreshRem);

上述代码中将视图容器分为10份，font-size用十分之一的宽度来表示，最后在header标签中执行这段代码，就可以动态定义font-size的大小，从而1rem

在不同的视觉容器中表示不同的大小，用rem固定单位可以实现不同容器内布局的自适应。

3）rem2px和px2rem 如果在响应式布局中使用rem单位，那么存在一个单位换算的问题，rem2px表示从rem换算成px，这个就不说了，只要rem乘以相应的font-size中的大小，就能换算成px。更多的应用是px2rem，表示的是从px转化为rem。

比如给定的视觉稿为750px（物理像素），如果我们要将所有的布局单位都用rem 来表示，一种比较笨的办法就是对所有的height和width等元素，乘以相应的比例，现将视觉稿换算成rem单位，然后一个个的用rem来表示。另一种比较方便的解决方法就是，在css中我们还是用px来表示元素的大小，最后编写完css 代码之后，将css文件中的所有px单位，转化成rem单位。

px2rem的原理也很简单，重点在于预处理以px为单位的css文件，处理后将所有的px变成rem单位。可以通过两种方式来实现：

（1）webpack loader的形式：

npm install px2rem-loader

在webpack的配置文件中：

module.exports = { // ... module: {

rules: [{ test: /\.css$/, use: [{

loader: 'style-loader'

}, {

loader: 'css-loader'

}, {

loader: 'px2rem-loader', // options here options: {

remUni: 75, remPrecision: 8 }

}]

}]

}

}

（2）webpack中使用postcss plugin

npm install postcss-loader

在webpack的plugin中:

var px2rem = require('postcss-px2rem'); module.exports = {

module: {

loaders: [

{ test: /\.css$/, loader: "style-loader!css-loader!postcss-loader" }

] }, postcss: function() {

return [px2rem({remUnit: 75})];

}

}

4）rem 布局应用举例网易新闻的移动端页面使用了rem布局，具体例子如下：

\5. rem 布局的缺点通过rem单位，可以实现响应式的布局，特别是引入相应的postcss相关插件，免去了设计稿中的px到rem的计算。rem单位在国外的一些网站也有使用，这里所说的rem来实现布局的缺点，或者说是小缺陷是：在响应式布局中，必须通过js来动态控制根元素font-size的大小。也就是说css样式和js代码有一定的耦合性。且必须将改变font-size的代码放在css样式之前。

五. 通过vw/vh来实现自适应

1. 什么是vw/vh ?

> css3中引入了一个新的单位vw/vh，与视图窗口有关，vw表示相对于视图窗口的宽度，vh表示相对于视图窗口高度，除了vw和vh外，还有vmin和vmax两个相关的单位。
>
> 各个单位具体的含义如下：

  单位   含义

  vw     相对于视窗的宽度，视窗宽度是100vw  vh     相对于视窗的高度，视窗高度是100vh  vmin   vw和vh中的较小值  vmax   vw和vh中的较大值

> 这里我们发现视窗宽高都是100vw／100vh，那么vw或者vh，下简称vw，很类似百分比单位。
>
> vw和%的区别为：

  单位    含义

  \%      大部分相对于祖先元素，也有相对于自身的情况比如（border-radius、 translate等)  vw/vh   相对于视窗的尺寸

> 从对比中我们可以发现，vw单位与百分比类似，单确有区别，前面我们介绍了百分比单位的换算困难，这里的vw更像"理想的百分比单位"。任意层级元素，在使用vw单位的情况下，1vw都等于视图宽度的百分之一。

1. vw单位换算同样的，如果要将px换算成vw单位，很简单，只要确定视图的窗口大小（布局

> 视口），如果我们将布局视口设置成分辨率大小，比如对于iphone6/7 375*667
>
> 的分辨率，那么px可以通过如下方式换算成vw：
>
> 1px = （1/375）*100 vw
>
> 此外，也可以通过postcss的相应插件，预处理css做一个自动的转换，
>
> [postcss-px-to-viewport](https://github.com/evrone/postcss-px-to-viewport)可以自动将px转化成vw。
>
> postcss-px-to-viewport的默认参数为： var defaults = {
>
> viewportWidth: 320, viewportHeight: 568, unitPrecision: 5, viewportUnit: 'vw', selectorBlackList: [], minPixelValue: 1, mediaQuery: false
>
> };
>
> 通过指定视窗的宽度和高度，以及换算精度，就能将px转化成vw。
>
> 3）vw/vh单位的兼容性可以在https://caniuse.com/ 查看各个版本的浏览器对vw单位的支持性。绝大多数的浏览器支持vw单位，但是ie9-11不支持vmin和vmax，考虑到vmin
>
> 和vmax单位不常用，vw单位在绝大部分高版本浏览器内的支持性很好，但是 opera浏览器整体不支持vw单位，如果需要兼容opera浏览器的布局，不推荐使用vw。

## 22.click在ios上有300ms延迟，原因及如何解决？

(1)粗暴型，禁用缩放

(2)利用FastClick，其原理是：

检测到touchend事件后，立刻出发模拟click事件，并且把浏览器300毫秒之后真正出发的事件给阻断掉

## 23.addEventListener参数

addEventListener(event, function, useCapture)

其中，event指定事件名；function指定要事件触发时执行的函数；useCapture指定事件是否在捕获或冒泡阶段执行。



## 32.前端优化

 

降低请求量：合并资源，减少HTTP 请求数，minify/gzip 压缩，webP，lazyLoad。

加快请求速度：预解析DNS，减少域名数，并行加载，CDN 分发。

缓存：HTTP 协议缓存请求，离线缓存 manifest，离线数据缓存localStorage。

渲染：JS/CSS优化，加载顺序，服务端渲染，pipeline。





## 37.说一下浏览器缓存

 缓存分为两种：强缓存和协商缓存，根据响应的header内容来决定。

强缓存相关字段有expires，cache-control。如果cache-control与expires 同时存在的话，cache-control的优先级高于expires。

协商缓存相关字段有Last-Modified/If-Modified-Since，Etag/If-None-Match

## 38.HTML5新增的元素

 

首先html5为了更好的实践web语义化，增加了header，footer， nav,aside,section等语义化标签；

在表单方面，为了增强表单，为input增加了color，emial,data ,range等类型；

在存储方面，提供了sessionStorage，localStorage,和离线存储，通过这些存储方式方便数据在客户端的存储和获取；

在多媒体方面规定了音频和视频元素audio和vedio，另外还有地理定位，canvas 画布，拖放，多线程编程的web worker和websocket协议；



## 如何解决异步回调地狱

promise、generator、async/await

## 说说前端中的事件流

HTML中与javascript交互是通过事件驱动来实现的，例如鼠标点击事件 onclick、页面的滚动事件onscroll等等，可以向文档或者文档中的元素添加事件侦听器来预订事件。想要知道这些事件是在什么时候进行调用的，就需要了解一下"事件流"的概念。

什么是事件流：事件流描述的是从页面中接收事件的顺序,DOM2级事件流包括下面几个阶段。事件捕获阶段处于目标阶段事件冒泡阶段

addEventListener：addEventListener 是DOM2 级事件新增的指定事件处理程序的操作，这个方法接收3个参数：要处理的事件名、作为事件处理程序的函数和一个布尔值。最后这个布尔值参数如果是true，表示在捕获阶段调用事件处理程序；如果是false，表示在冒泡阶段调用事件处理程序。

IE只支持事件冒泡。

## 如何让事件先冒泡后捕获

在DOM标准事件模型中，是先捕获后冒泡。但是如果要实现先冒泡后捕获的效果，对于同一个事件，监听捕获和冒泡，分别对应相应的处理函数，监听到捕获事件，**先暂缓执行**，直到冒泡事件被捕获后再执行捕获之间。

## 事件委托

简介：事件委托指的是，不在事件的发生地（直接dom）上设置监听函数，而是在其父元素上设置监听函数，通过事件冒泡，父元素可以监听到子元素上事件的触发，通过判断事件发生元素DOM的类型，来做出不同的响应。

举例：最经典的就是ul和li标签的事件监听，比如我们在添加事件时候，采用事件委托机制，不会在li标签上直接添加，而是在ul父元素上添加。

好处：比较合适动态元素的绑定，新添加的子元素也会有监听函数，也可以有事件触发机制。

## 说一下图片的懒加载和预加载

预加载：提前加载图片，当用户需要查看时可直接从本地缓存中渲染。

懒加载：懒加载的主要目的是作为服务器前端的优化，减少请求数或延迟请求数。两种技术的本质：两者的行为是相反的，一个是提前加载，一个是迟缓甚至不加载。

懒加载对服务器前端有一定的缓解压力作用，预加载则会增加服务器前端压力。

## mouseover和mouseenter的区别

mouseover：当鼠标移入元素或其子元素都会触发事件，所以有一个重复触发，冒泡的过程。对应的移除事件是mouseout

mouseenter：当鼠标移除元素本身（不包含元素的子元素）会触发事件，也就是不会冒泡，对应的移除事件是mouseleave

## js的new操作符做了哪些事情

new 操作符新建了一个空对象，这个对象原型指向构造函数的prototype，执行构造函数后返回这个对象。

## 改变函数内部this指针的指向函数（bind，apply，call 的区别）todo

通过apply和call改变函数的this指向，他们两个函数的第一个参数都是一样

的表示要改变指向的那个对象，第二个参数，apply是数组，而call则是arg1,arg2...这种形式。通过bind改变this作用域会返回一个新的函数，这个函数不会马上执行。

137.js的各种位置，比如 clientHeight,scrollHeight,offsetHeight ,以及

## scrollTop, offsetTop,clientTop的区别？

clientHeight：表示的是可视区域的高度，不包含border和滚动条 

offsetHeight：表示可视区域的高度，包含了border和滚动条

scrollHeight：表示了所有区域的高度，包含了因为滚动被隐藏的部分。

clientTop：表示边框border的厚度，在未指定的情况下一般为0

scrollTop：滚动后被隐藏的高度，获取对象相对于由offsetParent属性指定的父坐标(css定位的元素或body元素)距离顶端的高度。

## js拖拽功能的实现

首先是三个事件，分别是mousedown，mousemove，mouseup

当鼠标点击按下的时候，需要一个tag标识此时已经按下，可以执行mousemove 里面的具体方法。

clientX，clientY标识的是鼠标的坐标，分别标识横坐标和纵坐标，并且我们用offsetX和offsetY来表示元素的元素的初始坐标，移动的举例应该是：鼠标移动时候的坐标-鼠标按下去时候的坐标。

也就是说定位信息为：

鼠标移动时候的坐标-鼠标按下去时候的坐标+元素初始情况下的offetLeft.

还有一点也是原理性的东西，也就是拖拽的同时是绝对定位，我们改变的是绝对定位条件下的left 以及top等等值。

补充：也可以通过html5的拖放（Drag 和 drop）来实现

## 异步加载js的方法

defer：只支持IE如果您的脚本不会改变文档的内容，可将 defer 属性加入到 `<script>`标签中，以便加快处理文档的速度。因为浏览器知道它将能够安全地读取文档的剩余部分而不用执行脚本，它将推迟对脚本的解释，直到文档已经显示给用户为止。

async，HTML5属性仅适用于外部脚本，并且如果在IE中，同时存在defer和 async，那么defer的优先级比较高，脚本将在页面完成时执行。

创建script标签，插入到DOM中.

## Ajax解决浏览器缓存问题

在ajax发送请求前加上

`anyAjaxObj.setRequestHeader("If-Modified-Since","0")`。

在ajax发送请求前加上

`anyAjaxObj.setRequestHeader("Cache-Control","no-cache")`。

在URL后面加上一个随机数： "fresh=" + Math.random()。

在URL后面加上时间搓："nowtime=" + new Date().getTime()。如果是使用jQuery，直接这样就可以了 $.ajaxSetup({cache:false})。这样页面的所有ajax都会执行这条语句就是不需要保存缓存记录。



## JS中的垃圾回收机制

必要性：由于字符串、对象和数组没有固定大小，所有当他们的大小已知时，才能对他们进行动态的存储分配。JavaScript程序每次创建字符串、数组或对象时，解释器都必须分配内存来存储那个实体。只要像这样动态地分配了内存，最终都要释放这些内存以便他们能够被再用，否则，JavaScript的解释器将会消耗完系统中所有可用的内存，造成系统崩溃。

这段话解释了为什么需要系统需要垃圾回收，JS不像C/C++，他有自己的一套垃圾回收机制（Garbage Collection）。JavaScript的解释器可以检测到何时程序不再使用一个对象了，当他确定了一个对象是无用的时候，他就知道不再需要这个对象，可以把它所占用的内存释放掉了。

例如：

`var a="hello world"; var b="world"; var a=b;` //这时，会释放掉"hello world"，释放内存以便再引用

垃圾回收的方法：标记清除、计数引用。

标记清除：

这是最常见的垃圾回收方式，当变量进入环境时，就标记这个变量为"进入环境 ",从逻辑上讲，永远不能释放进入环境的变量所占的内存，永远不能释放进入环境变量所占用的内存，只要执行流程进入相应的环境，就可能用到他们。当离开环境时，就标记为离开环境。

垃圾回收器在运行的时候会给存储在内存中的变量都加上标记（所有都加），然后去掉环境变量中的变量，以及被环境变量中的变量所引用的变量（条件性去除标记），删除所有被标记的变量，删除的变量无法在环境变量中被访问所以会被删除，最后垃圾回收器，完成了内存的清除工作，并回收他们所占用的内存。

引用计数法：

另一种不太常见的方法就是引用计数法，引用计数法的意思就是每个值没引用的次数，当声明了一个变量，并用一个引用类型的值赋值给改变量，则这个值的引用次数为1,；相反的，如果包含了对这个值引用的变量又取得了另外一个值，则原先的引用值引用次数就减1，当这个值的引用次数为0的时候，说明没有办法再访问这个值了，因此就把所占的内存给回收进来，这样垃圾收集器再次运行的时候，就会释放引用次数为0的这些值。

用引用计数法会存在内存泄露，下面来看原因：

```js
function problem() {

var objA = new Object(); var objB = new Object();

objA.someOtherObject = objB;

objB.anotherObject = objA;

}
```

在这个例子里面，objA和objB通过各自的属性相互引用，这样的话，两个对象的引用次数都为2，在采用引用计数的策略中，由于函数执行之后，这两个对象都离开了作用域，函数执行完成之后，因为计数不为0，这样的相互引用如果大量存在就会导致内存泄露。

特别是在DOM对象中，也容易存在这种问题：

```js
var element=document.getElementById（''）； 
var myObj=new Object(); myObj.element=element;
element.someObject=myObj;
```

这样就不会有垃圾回收的过程。

## eval是做什么的

它的功能是将对应的字符串解析成js并执行，应该避免使用js，因为非常消耗性能（2次，一次解析成js，一次执行）

## 如何理解前端模块化

前端模块化就是复杂的文件编程一个一个独立的模块，比如js文件等等，分成独立的模块有利于重用（复用性）和维护（版本迭代），这样会引来模块之间相互依赖的问题，所以有了commonJS规范，AMD，CMD规范等等，以及用于js打包（编译等处理）的工具webpack。

## 说一下Commonjs、AMD和CMD

一个模块是能实现特定功能的文件，有了模块就可以方便的使用别人的代码，想要什么功能就能加载什么模块。

Commonjs：开始于服务器端的模块化，同步定义的模块化，每个模块都是一个单

独的作用域，模块输出，modules.exports，模块加载require()引入模块。

AMD：中文名异步模块定义的意思。

requireJS实现了AMD规范，主要用于解决下述两个问题。

1）多个文件有依赖关系，被依赖的文件需要早于依赖它的文件加载到浏览器 2）加载的时候浏览器会停止页面渲染，加载文件越多，页面失去响应的时间越长。

语法：requireJS定义了一个函数define，它是全局变量，用来定义模块。 requireJS的例子：

//定义模块

define(['dependency'], function(){ var name = 'Byron'; function printName(){ console.log(name); } return { printName: printName

};

});

//加载模块

require(['myModule'], function (my){ my.printName(); }

requirejs定义了一个函数define,它是全局变量，用来定义模块： define(id?dependencies?,factory)

在页面上使用模块加载函数：

require([dependencies],factory)；

总结AMD规范：require（）函数在加载依赖函数的时候是异步加载的，这样浏览器不会失去响应，它指定的回调函数，只有前面的模块加载成功，才会去执行。因为网页在加载js的时候会停止渲染，因此我们可以通过异步的方式去加载js, 而如果需要依赖某些，也是异步去依赖，依赖后再执行某些方法。 146.对象深度克隆的简单实现



function deepClone(obj){ var newObj= obj instanceof Array ? []:{}; for(var item in obj){ var temple= typeof obj[item] == 'object' ?

deepClone(obj[item]):obj[item]; newObj[item] = temple;

} return newObj;

}

ES5的常用的对象克隆的一种方式。注意数组是对象，但是跟对象又有一定区别，所以我们一开始判断了一些类型，决定newObj是对象还是数组 147.实现一个once函数，传入函数参数只执行一次



function ones(func){ var tag=true; return function(){ if(tag==true){ func.apply(null,arguments); tag=false; } return undefined

}

}

## 将原生的ajax封装成promise

```js
var myNewAjax=function(url){ return new Promise(function(resolve,reject){ var xhr = new XMLHttpRequest(); xhr.open('get',url); xhr.send(data); xhr.onreadystatechange=function(){ if(xhr.status==200&&readyState==4){ var json=JSON.parse(xhr.responseText); resolve(json)

}else if(xhr.readyState==4&&xhr.status!=200){ reject('error'); }

}

})

}
```

## js监听对象属性的改变

我们假设这里有一个user对象,

(1)在ES5中可以通过Object.defineProperty来实现已有属性的监听 Object.defineProperty(user,'name',{ set：function(key,value){

}

})

缺点：如果id不在user对象中，则不能监听id的变化

(2)在ES6中可以通过Proxy来实现 var user = new Proxy({}，{

set：function(target,key,value,receiver){

}

})

这样即使有属性在user中不存在，通过user.id来定义也同样可以这样监听这个属性的变化哦~

## 如何实现一个私有变量，用getName方法可以访问，不能直接访问

```js
//(1)通过defineProperty来实现

obj={ name:yuxiaoliang, getName:function(){ return this.name

} } object.defineProperty(obj,"name",{

//不可枚举不可配置

});

//(2)通过函数的创建形式

function product(){ var name='yuxiaoliang'; this.getName=function(){ return name;

} }

var obj=new product();
```

## ==和===、以及Object.is的区别

(1) == 主要存在：强制转换成number,null==undefined

" "==0 //true

"0"==0 //true

" " !="0" //true 123=="123" //true null==undefined //true

(2)Object.js

主要的区别就是+0！=-0 而NaN==NaN (相对比===和==的改进)

## setTimeout、setInterval和requestAnimationFrame 之间的区别

requestAnimationFrame与setTimeout和setInterval不同，

requestAnimationFrame不需要设置时间间隔，

大多数电脑显示器的刷新频率是60Hz，大概相当于每秒钟重绘60次。大多数浏览器都会对重绘操作加以限制，不超过显示器的重绘频率，因为即使超过那个频率用户体验也不会有提升。因此，最平滑动画的最佳循环间隔是1000ms/60，约等于16.6ms。

RAF采用的是系统时间间隔，不会因为前面的任务，不会影响RAF，但是如果前面的任务多的话，

会响应setTimeout和setInterval真正运行时的时间间隔。

特点：

1. requestAnimationFrame会把每一帧中的所有DOM操作集中起来，在一次重绘或回流中就完成，并且重绘或回流的时间间隔紧紧跟随浏览器的刷新频率。
2. 在隐藏或不可见的元素中，requestAnimationFrame将不会进行重绘或回流，这当然就意味着更少的CPU、GPU和内存使用量.requestAnimationFrame是由浏览器专门为动画提供的API，在运行时浏览器会自动优化方法的调用，并且如果页面不是激活状态下的话，动画会自动暂停，有效节省了CPU开销。

## 实现一个两列等高布局，讲讲思路

为了实现两列等高，可以给每列加上 padding-bottom:9999px; margin-bottom:-9999px;同时父元素设置overflow:hidden;

## 自己实现一个bind函数

>  
>
> 原理：通过apply或者call方法来实现。
>
> (1)初始版本
>
> Function.prototype.bind=function(obj,arg){
>
> var arg=Array.prototype.slice.call(arguments,1);
>
> var context=this; return function(newArg){ arg=arg.concat(Array.prototype.slice.call(newArg)); return context.apply(obj,arg);
>
> }
>
> }
>
> (2) 考虑到原型链为什么要考虑？因为在new 一个bind过生成的新函数的时候，必须的条件是要继承原函数的原型
>
> Function.prototype.bind=function(obj,arg){ var arg=Array.prototype.slice.call(arguments,1); var context=this; var bound=function(newArg){ arg=arg.concat(Array.prototype.slice.call(newArg)); return context.apply(obj,arg);
>
> } var F=function(){}
>
> //这里需要一个寄生组合继承
>
> F.prototype=context.prototype; bound.prototype=new F(); return bound; }

## 用setTimeout来实现setInterval

>  
>
> (1)用setTimeout()方法来模拟setInterval()与setInterval()之间的什么区
>
> 别？首先来看setInterval的缺陷，使用setInterval()创建的定时器确保了定时器代码规则地插入队列中。这个问题在于：如果定时器代码在代码再次添加到队列之前还没完成执行，结果就会导致定时器代码连续运行好几次。而之间没有间隔。
>
> 不过幸运的是：javascript引擎足够聪明，能够避免这个问题。当且仅当没有该定时器的如何代码实例时，才会将定时器代码添加到队列中。这确保了定时器代码加入队列中最小的时间间隔为指定时间。
>
> 这种重复定时器的规则有两个问题：1.某些间隔会被跳过 2.多个定时器的代码执行时间可能会比预期小。
>
> 下面举例子说明：
>
> 假设，某个onclick事件处理程序使用啦setInterval()来设置了一个200ms的重复定时器。如果事件处理程序花了300ms多一点的时间完成。
>
> src="https://user-images.githubusercontent.com/17233651/42487876-9265
>
> 6f2c-8435-11e8-8a5f-0a97918039da.png">
>
> 这个例子中的第一个定时器是在205ms处添加到队列中，但是要过300ms才能执行。在405ms又添加了一个副本。在一个间隔，605ms处，第一个定时器代码还在执行中，而且队列中已经有了一个定时器实例，结果是605ms的定时器代码不会添加到队列中。结果是在5ms处添加的定时器代码执行结束后，405处的代码立即执行。
>
> function say(){
>
> //something
>
> setTimeout(say,200);
>
> }
>
> setTimeout(say,200) 或者 setTimeout(function(){ //do something setTimeout(arguments.callee,200); },200);

## 代码的执行顺序

>  
>
> setTimeout(function(){console.log(1)},0); new Promise(function(resolve,reject){ console.log(2); resolve(); }).then(function(){console.log(3) }).then(function(){console.log(4)}); process.nextTick(function(){console.log(5)}); console.log(6);
>
> //输出2,6,5,3,4,1

## 如何实现sleep的效果（es5或者es6）

```js
//实现sleep
//1.while循环
function sleep1(ms){
    var start = Date.now(),expire = start+ms;
    while(Date.now()<expire);
    console.log("1111")
    return;
}

//2.promise
function sleep2(ms){
    var temp = new Promise(resolve=>{
        console.log(111);
        setTimeout(resolve,ms)
    });
    return temp; 
}sleep2(500).then(function(){console.log("2222")})

//3.async
function sleep3(ms){
    return new Promise((resolve)=>setTimeout(resolve,ms));
}
async function test(){
    var temp = await sleep3(500);
    console.log("1111");
    return temp;
}
test()

//4.generate
function *sleep4(ms){
    yield new Promise(function(resolve,reject){
        console.log("1111");
        setTimeout(resolve,ms);
    })
}
sleep4(500).next().value.then(function(){
    console.log("2222");})
```

## 简单的实现一个promise

Promise允许我们通过链式调用的方式来解决"回调地狱"的问题，特别是在异步过程中，通过Promise可以保证代码的整洁性和可读性。下面主要解读 Promise/A+规范，并在此规范的基础上，自己实现一个Promise.

一、**Promise** 的使用

在了解Promise规范之前，我们知道主流的高版本浏览器已经支持ECMA中的Promise.

创建一个promise实例：

var p=new Promise(function(resolve,reject){ setTimeout(function(){ resolve("success")

},1000); console.log("创建一个新的promise");

})

p.then(function(x){

console.log(x)

})

//输出：创建一个新的promise

Success

上述是一个promise的实例，输出内容为，"创建一个promise"，延迟1000ms

后，输出"success"。

从上述的例子可以看出，promise方便处理异步操作。此外promise还可以链式

的调用：

var p=new Promise(function(resolve,reject){resolve()}); p.then(...).then(...).then(...)

此外Promise除了then方法外，还提供了Promise.resolve、Promise.all、 Promise.race等等方法。二、Promise/A+规范

[Promise/A+](https://promisesaplus.com/)规范扩展了早期的[Promise/A](http://wiki.commonjs.org/wiki/Promises/A) [proposal](http://wiki.commonjs.org/wiki/Promises/A)提案，我们来解读一下 Promise/A+规范。

1）术语

1. "promise"是一个对象或者函数，该对象或者函数有一个then方法
2. "thenable"是一个对象或者函数，用来定义then方法
3. "value"是promise状态成功时的值（4）"reason"是promise状态失败时的值

我们明确术语的目的，是为了在自己实现promise时，保持代码的规范性（也可以跳过此小节）

2）要求

1. 一个promise必须有3个状态，pending，fulfilled(resolved)，rejected 当处于pending状态的时候，可以转移到fulfilled(resolved)或者rejected 状态。当处于fulfilled(resolved)状态或者rejected状态的时候，就不可变。

promise英文译为承诺，也就是说promise的状态一旦发生改变，就永远是不可逆的。

1. 一个promise必须有一个then方法，then方法接受两个参数：

promise.then(onFulfilled,onRejected)

其中onFulfilled方法表示状态从pending------>fulfilled(resolved)时所执行的方法，而onRejected表示状态从pending------>rejected所执行的方法。

1. 为了实现链式调用，then方法必须返回一个promise

promise2=promise1.then(onFulfilled,onRejected)

三、实现一个符合Promise/A+规范的Promise 解读了Promise/A+规范之后，下面我们来看如何实现一个Promise, 首先构造一个myPromise函数，关于所有变量和函数名，应该与规范中保持相同。

**1.v1.0** 初始版本 **myPromise**

function myPromise(constructor){ let self=this;

self.status="pending" //定义状态改变前的初始状态 self.value=undefined;//定义状态为resolved的时候的状态 self.reason=undefined;//定义状态为rejected的时候的状态 function resolve(value){

//两个==="pending"，保证了状态的改变是不可逆的

if(self.status==="pending"){ self.value=value; self.status="resolved";

} } function reject(reason){

//两个==="pending"，保证了状态的改变是不可逆的

if(self.status==="pending"){ self.reason=reason; self.status="rejected";

}

}

//捕获构造异常

try{ constructor(resolve,reject);

}catch(e){ reject(e);

}

}

同时，需要在myPromise的原型上定义链式调用的then方法：

myPromise.prototype.then=function(onFullfilled,onRejected){ let self=this; switch(self.status){ case "resolved":

onFullfilled(self.value); break;

case "rejected":

onRejected(self.reason); break; default:

}

}

上述就是一个初始版本的myPromise，在myPromise里发生状态改变，然后在相

应的then方法里面根据不同的状态可以执行不同的操作。

var p=new myPromise(function(resolve,reject){resolve(1)}); p.then(function(x){console.log(x)})

//输出1 但是这里myPromise无法处理异步的resolve.比如： var p=new myPromise(function(resolve,reject){setTimeout(function(){resolve(1)},

1000)});

p.then(function(x){console.log(x)})

//无输出

2.v2.0基于观察模式实现

为了处理异步resolve，我们修改myPromise的定义，用2个数组

onFullfilledArray和onRejectedArray来保存异步的方法。在状态发生改变时，

一次遍历执行数组中的方法。

function myPromise(constructor){ let self=this;

self.status="pending" //定义状态改变前的初始状态 self.value=undefined;//定义状态为resolved的时候的状态 self.reason=undefined;//定义状态为rejected的时候的状态

self.onFullfilledArray=[]; self.onRejectedArray=[]; function resolve(value){ if(self.status==="pending"){ self.value=value; self.status="resolved"; self.onFullfilledArray.forEach(function(f){ f(self.value);

//如果状态从pending变为resolved，

//那么就遍历执行里面的异步方法

});

} } function reject(reason){ if(self.status==="pending"){ self.reason=reason; self.status="rejected"; self.onRejectedArray.forEach(function(f){ f(self.reason);

//如果状态从pending变为rejected，

//那么就遍历执行里面的异步方法

})

}

}

//捕获构造异常

try{ constructor(resolve,reject);

}catch(e){ reject(e);

}

}

对于then方法，状态为pending时，往数组里面添加方法：

myPromise.prototype.then=function(onFullfilled,onRejected){

let self=this; switch(self.status){

case "pending":

self.onFullfilledArray.push(function(){ onFullfilled(self.value)

}); self.onRejectedArray.push(function(){ onRejected(self.reason)

}); case "resolved":

onFullfilled(self.value); break; case "rejected": onRejected(self.reason); break; default:

}

}

这样，通过两个数组，在状态发生改变之后再开始执行，这样可以处理异步

resolve无法调用的问题。这个版本的myPromise就能处理所有的异步，那么这

样做就完整了吗？

没有，我们做Promise/A+规范的最大的特点就是链式调用，也就是说then方法返回的应该是一个promise。

3.v3.0then方法实现链式调用

要通过then方法实现链式调用，那么也就是说then方法每次调用需要返回一个 primise,同时在返回promise的构造体里面，增加错误处理部分，我们来改造

then方法

myPromise.prototype.then=function(onFullfilled,onRejected){ let self=this; let promise2; switch(self.status){

case "pending":

promise2=new myPromise(function(resolve,reject){ self.onFullfilledArray.push(function(){ try{ let temple=onFullfilled(self.value); resolve(temple)

}catch(e){ reject(e) //error catch

}

});

self.onRejectedArray.push(function(){ try{

let temple=onRejected(self.reason); reject(temple)

}catch(e){ reject(e)// error catch

}

});

}) case "resolved":

promise2=new myPromise(function(resolve,reject){ try{

let temple=onFullfilled(self.value);

//将上次一then里面的方法传递进下一个Promise的状态

resolve(temple);

}catch(e){ reject(e);//error catch

} }) break;

case "rejected":

promise2=new myPromise(function(resolve,reject){ try{ let temple=onRejected(self.reason);

//将then里面的方法传递到下一个Promise的状态里

resolve(temple);

}catch(e){ reject(e);

} }) break; default: } return promise2;

}

这样通过then方法返回一个promise就可以实现链式的调用：

p.then(function(x){console.log(x)}).then(function(){console.log("链式调用1")}).then(function(){console.log("链式调用2")})

//输出

1

链式调用1 链式调用2

这样我们虽然实现了then函数的链式调用，但是还有一个问题，就是在

Promise/A+规范中then函数里面的onFullfilled方法和onRejected方法的返

回值可以是对象，函数，甚至是另一个promise。

4.v4.0 then函数中的onFullfilled和onRejected方法的返回值问题

特别的为了解决onFullfilled和onRejected方法的返回值可能是一个promise

的问题。

（1）首先来看promise中对于onFullfilled函数的返回值的要求

I.  如果onFullfilled函数返回的是该promise本身，那么会抛出类型错误

II. 如果onFullfilled函数返回的是一个不同的promise，那么执行该promise 的then函数，在then函数里将这个promise的状态转移给新的promise

III. 如果返回的是一个嵌套类型的promsie，那么需要递归。

IV)如果返回的是非promsie的对象或者函数，那么会选择直接将该对象或者函

数，给新的promise。

根据上述返回值的要求，我们要重新的定义resolve函数，这里Promise/A+规

范里面称为：resolvePromise函数，该函数接受当前的promise、onFullfilled 函数或者onRejected函数的返回值、resolve和reject作为参数。

下面我们来看resolvePromise函数的定义：

function resolvePromise(promise,x,resolve,reject){

if(promise===x){ throw new TypeError("type error")

} let isUsed; if(x!==null&&(typeof x==="object"||typeof x==="function")){ try{

let then=x.then; if(typeof then==="function"){

//是一个promise的情况

then.call(x,function(y){ if(isUsed)return; isUsed=true; resolvePromise(promise,y,resolve,reject);

},function(e){ if(isUsed)return; isUsed=true; reject(e);

})

}else{

//仅仅是一个函数或者是对象

resolve(x)

}

}catch(e){ if(isUsed)return; isUsed=true; reject(e);

}

}else{

//返回的基本类型，直接resolve

resolve(x)

}

}

改变了resolvePromise函数之后，我们在then方法里面的调用也变成了 resolvePromise而不是promise。

myPromise.prototype.then=function(onFullfilled,onRejected){ let self=this; let promise2; switch(self.status){

case "pending":

promise2=new myPromise(function(resolve,reject){ self.onFullfilledArray.push(function(){ setTimeout(function(){

try{ let temple=onFullfilled(self.value); resolvePromise(temple)

}catch(e){ reject(e) //error catch

}

}) }); self.onRejectedArray.push(function(){ setTimeout(function(){ try{

let temple=onRejected(self.reason); resolvePromise(temple)

}catch(e){ reject(e)// error catch

}

})

});

}) case "resolved":

promise2=new myPromise(function(resolve,reject){ setTimeout(function(){ try{

let temple=onFullfilled(self.value);

//将上次一then里面的方法传递进下一个Promise状态

resolvePromise(temple);

}catch(e){ reject(e);//error catch

}

}) }) break;

case "rejected":

promise2=new myPromise(function(resolve,reject){ setTimeout(function(){

try{

let temple=onRejected(self.reason);

//将then里面的方法传递到下一个Promise的状态里

resolvePromise(temple);

}catch(e){ reject(e);

}

})

}) break; default:

} return promise2;

}

这样就能处理onFullfilled各种返回值的情况。

var p=new Promise(function(resolve,reject){resolve("初始化promise")}) p.then(function(){return new

Promise(function(resolve,reject){resolve("then里面的promise返回值 ")})}).then(function(x){console.log(x)})

//输出 then里面promise的返回值

到这里可能有点乱，我们再理一理，首先返回值有两个： then函数的返回值------>返回一个新promise，从而实现链式调用

then函数中的onFullfilled和onRejected方法------>返回基本值或者新的

promise

这两者其实是有关联的，onFullfilled方法的返回值可以决定then函数的返回

值。

1. 检测是否完全符合Promise/A+规范

> npm install -g promises-aplus-tests
>
> 具体用法请看[promise](https://github.com/promises-aplus/promises-tests) [test](https://github.com/promises-aplus/promises-tests)然后
>
> promises-aplus-tests myPromise.js 说明我们的实现完全符合Promise/A+规范。

1. 最后补充 **Typescript** 实现的 **Promise/A+**规范（可以忽略此节）

interface IConstructor{

(resolve:IResolve,reject:IReject):void } interface IResolve { (x:any):void } interface IReject { (x:any):void } function myPromise(constructor:IConstructor):void{

let self:object=this; self.status="pending"; self.value=undefined;//if pending->resolved self.reason=undefined;//if pending->rejected self.onFullfilledArray=[];//to deal with async(resolved) self.onRejectedArray=[];//to deal with async(rejeced) let resolve:IResolve; resolve=function(value:any):void{

//pending->resolved if(self.status==="pending"){

self.status="resolved"; self.value=value; self.onFullfilledArray.forEach(function(f){

f(self.value);

})

}

}

let reject:IReject; reject=function(reason:any):void{

if(self.status==="pending"){

self.status="rejected"; self.reason=reason; self.onRejectedArray.forEach(function(f){

f(self.reason);

})

}

}

//According to the definition that the function "constructor" accept two parameters //error catch try {

> constructor(resolve,reject);
>
> } catch (e) { reject(e);
>
> }
>
> }

## Function._proto_(getPrototypeOf)是什么？

获取一个对象的原型，在chrome中可以通过_proto_的形式，或者在ES6中可以

通过Object.getPrototypeOf的形式。

那么Function.proto是什么么？也就是说Function由什么对象继承而来，我们

来做如下判别。

Function.__proto__==Object.prototype //false

Function.__proto__==Function.prototype//true 我们发现Function的原型也是Function。

## 实现js中所有对象的深度克隆（包装对象，Date对象，正则对象

>  通过递归可以简单实现对象的深度克隆，但是这种方法不管是ES6还是ES5实现，都有同样的缺陷，就是只能实现特定的object的深度复制（比如数组和函数），
>
> 不能实现包装对象Number，String ， Boolean，以及Date对象，RegExp对象
>
> 的复制。
>
> (1)前文的方法
>
> function deepClone(obj){ var newObj= obj instanceof Array?[]:{}; for(var i in obj){ newObj[i]=typeof obj[i]=='object'?
>
> deepClone(obj[i]):obj[i]; } return newObj;
>
> }
>
> 这种方法可以实现一般对象和数组对象的克隆，比如：
>
> var arr=[1,2,3]; var newArr=deepClone(arr); // newArr->[1,2,3] var obj={ x:1, y:2 }
>
> var newObj=deepClone(obj);
>
> // newObj={x:1,y:2}
>
> 但是不能实现例如包装对象Number,String,Boolean,以及正则对象RegExp和
>
> Date对象的克隆，比如：
>
> //Number包装对象
>
> var num=new Number(1); typeof num // "object" var newNum=deepClone(num);
>
> //newNum -> {} 空对象
>
> //String包装对象
>
> var str=new String("hello"); typeof str //"object" var newStr=deepClone(str);
>
> //newStr-> {0:'h',1:'e',2:'l',3:'l',4:'o'};
>
> //Boolean包装对象
>
> var bol=new Boolean(true); typeof bol //"object" var newBol=deepClone(bol);
>
> // newBol ->{} 空对象
>
> ....
>
> (2)valueof()函数
>
> 所有对象都有valueOf方法，valueOf方法对于：如果存在任意原始值，它就默
>
> 认将对象转换为表示它的原始值。对象是复合值，而且大多数对象无法真正表示为一个原始值，因此默认的valueOf()方法简单地返回对象本身，而不是返回一个原始值。数组、函数和正则表达式简单地继承了这个默认方法，调用这些类型
>
> 的实例的valueOf()方法只是简单返回这个对象本身。对于原始值或者包装类：
>
> function baseClone(base){ return base.valueOf();
>
> } //Number var num=new Number(1); var newNum=baseClone(num);
>
> //newNum->1 //String var str=new String('hello'); var newStr=baseClone(str);
>
> // newStr->"hello" //Boolean var bol=new Boolean(true); var newBol=baseClone(bol);
>
> //newBol-> true
>
> 其实对于包装类，完全可以用=号来进行克隆，其实没有深度克隆一说，
>
> 这里用valueOf实现，语法上比较符合规范。
>
> 对于Date类型：因为valueOf方法，日期类定义的valueOf()方法会返回它的一个内部表示：1970
>
> 年1月1日以来的毫秒数.因此我们可以在Date的原型上定义克隆的方法：
>
> Date.prototype.clone=function(){ return new Date(this.valueOf());
>
> } var date=new Date('2010'); var newDate=date.clone();
>
> // newDate-> Fri Jan 01 2010 08:00:00 GMT+0800 对于正则对象RegExp：
>
> RegExp.prototype.clone = function() { var pattern = this.valueOf(); var flags = ''; flags += pattern.global ? 'g' : ''; flags += pattern.ignoreCase ? 'i' : ''; flags += pattern.multiline ? 'm' : ''; return new RegExp(pattern.source, flags);
>
> }; var reg=new RegExp('/111/'); var newReg=reg.clone(); //newReg-> /\/111\//

## 简单实现Node的Events模块

>  简介：观察者模式或者说订阅模式，它定义了对象间的一种一对多的关系，让多个观察者对象同时监听某一个主题对象，当一个对象发生改变时，所有依赖于它的对象都将得到通知。 node中的Events模块就是通过观察者模式来实现的：
>
> var events=require('events'); var eventEmitter=new events.EventEmitter(); eventEmitter.on('say',function(name){ console.log('Hello',name); }) eventEmitter.emit('say','Jony yu');
>
> 这样，eventEmitter发出say事件，通过On接收，并且输出结果，这就是一个订阅模式的实现，下面我们来简单的实现一个Events模块的EventEmitter。
>
> (1)实现简单的Event模块的emit和on方法
>
> function Events(){ this.on=function(eventName,callBack){ if(!this.handles){ this.handles={}; } if(!this.handles[eventName]){ this.handles[eventName]=[]; } this.handles[eventName].push(callBack); } this.emit=function(eventName,obj){ if(this.handles[eventName]){ for(var i=0;o<this.handles[eventName].length;i++){ this.handles[eventName][i](obj); }
>
> } } return this;
>
> }
>
> 这样我们就定义了Events，现在我们可以开始来调用：
>
> var events=new Events(); events.on('say',function(name){ console.log('Hello',nama) }); events.emit('say','Jony yu');
>
> //结果就是通过emit调用之后，输出了Jony yu
>
> (2)每个对象是独立的因为是通过new的方式，每次生成的对象都是不相同的，因此：
>
> var event1=new Events(); var event2=new Events(); event1.on('say',function(){ console.log('Jony event1');
>
> }); event2.on('say',function(){ console.log('Jony event2');
>
> }) event1.emit('say'); event2.emit('say');
>
> //event1、event2之间的事件监听互相不影响 //输出结果为'Jony event1' 'Jony event2'

## js判断类型

判断方法：typeof()，instanceof，Object.prototype.toString.call()等

## 判断数组的方法

- Object.prototype.toString.call()

  - 对于所有基本的数据类型都能进行判断，即使是 null 和 undefined 。

  - 每一个继承Object 的对象都有 toString 方法，如果 toString 方法没有重写的 

    话，会返回[Object type]，其中 type 为对象的类型。但当除了 Object 类型的 

    对象外，其他类型直接使用 toString 方法时，会直接返回都是内容的字符串， 

    所以我们需要使用 call 或者 apply 方法来改变 toString 方法的执行上下文

- instanceof

  - 通过判断对象的原型链中是不是能找到类型的 prototype。
  - 使用 instanceof 判断一个对象是否为数组，instanceof 会判断这个对象的原型 链上是否会找到对应的 Array 的原型，找到返回 true，否则返回 false。
  - `[] instanceof Array`
  - 但 instanceof 只能用来判断对象类型，原始类型不可以。并且所有对象类型 instanceof Object 都是 true。

- Array.isArray()

  - 检测 Array 实例时，Array.isArray 优于 instanceof ，因为 Array.isArray 可以检测出 iframes



## 数组常用方法

push()，pop()，shift()，unshift()，splice()，sort()，reverse()，map() 等

## 数组去重

法一：indexOf循环去重

法二：ES6 Set去重；Array.from(new Set(array))

法三：Object 键值对去重；把数组的值存成 Object 的 key 值，比如 Object[value1]=true，在判断另一个值的时候，如果 Object[value2]存在的话，就说明该值是重复的。

## 数组里面有 10 万个数据，取第一个元素和第 10 万个 元素的时间相差多少

数组可以直接根据索引取的对应的元素，所以不管取哪个位置的元素的时间复 杂度都是 O(1) 

得出结论：消耗时间几乎一致，差异可以忽略不计



## 闭包 有什么用

### 什么是闭包：

闭包是指有权访问另外一个函数作用域中的变量的函数。

闭包就是函数的局部变量集合，只是这些局部变量在函数返回后会继续存在。闭包就是就是函数的"堆栈"在函数返回后并不释放，我们也可以理解为这些函数堆栈并不在栈上分配而是在堆上分配。当在一个函数内定义另外一个函数就会产生闭包。

### 为什么要用：

匿名自执行函数：我们知道所有的变量，如果不加上var关键字，则默认的会添加到全局对象的属性上去，这样的临时变量加入全局对象有很多坏处，比如：别的函数可能误用这些变量；造成全局对象过于庞大，影响访问速度(因为变量的取值是需要从原型链上遍历的)。除了每次使用变量都是用var关键字外，我们在实际情况下经常遇到这样一种情况，即有的函数只需要执行一次，其内部变量无需维护，可以用闭包。

结果缓存：我们开发中会碰到很多情况，设想我们有一个处理过程很耗时的函数对象，每次调用都会花费很长时间，那么我们就需要将计算出来的值存储起来，当调用这个函数的时候，首先在缓存中查找，如果找不到，则进行计算，然后更新缓存并返回值，如果找到了，直接返回查找到的值即可。闭包正是可以做到这一点，因为它不会释放外部的引用，从而函数内部的值可以得以保留。

封装：实现类和继承等。

## 事件代理在捕获阶段的实际应用

可以在父元素层面阻止事件向子元素传播，也可代替子元素执行某些操作。

## 去除字符串首尾空格

使用正则(\^\s*)|(\s*$)即可

## 性能优化

减少HTTP请求

使用内容发布网络（CDN）添加本地缓存压缩资源文件

将CSS样式表放在顶部，把javascript放在底部（浏览器的运行机制决定）避免使用CSS表达式

减少DNS查询

使用外部javascript和CSS 避免重定向

图片lazyLoad

## 能来讲讲JS的语言特性吗

运行在客户端浏览器上；

不用预编译，直接解析执行代码；是弱类型语言，较为灵活；

与操作系统无关，跨平台的语言；脚本语言、解释性语言

## 如何判断一个数组



Object.prototype.call.toString()

Instanceof

## JS实现跨域



JSONP：通过动态创建 script，再请求一个带参网址实现跨域通信。 document.domain+iframe跨域：两个页面都通过js强制设置document.domain 为基础主域，就实现了同域。

location.hash + iframe跨域：a欲与b跨域相互通信，通过中间页c来实现。三个页面，不同域之间利用iframe的location.hash传值，相同域之间直接js 访问来通信。

window.name + iframe跨域：通过iframe的src属性由外域转向本地域，跨域数据即由iframe的window.name从外域传递到本地域。 postMessage跨域：可以跨域操作的window属性之一。

CORS：服务端设置Access-Control-Allow-Origin即可，前端无须设置，若要带 cookie请求，前后端都需要设置。

代理跨域：启一个代理服务器，实现数据的转发



## js深度拷贝一个元素的具体实现

var deepCopy = function(obj) { if (typeof obj !== 'object') return; var newObj = obj instanceof Array ? [] : {}; for (var key in obj) {

if (obj.hasOwnProperty(key)) { newObj[key] = typeof obj[key] === 'object' ? deepCopy(obj[key]) : obj[key]; } } return newObj; }

## 跨域的原理

跨域，是指浏览器不能执行其他网站的脚本。它是由浏览器的同源策略造成的，是浏览器对JavaScript实施的安全限制，那么只要协议、域名、端口有任何一个不同，都被当作是不同的域。跨域原理，即是通过各种方式，避开浏览器的安全限制。

## 不同数据类型的值的比较，是怎么转换的，有什么规则TODO

## null == undefined为什么

>  
>
> 要比较相等性之前，不能将null 和 undefined 转换成其他任何值，但 null== undefined 会返回 true 。ECMAScript规范中是这样定义的。

## this的指向 哪几种

默认绑定：全局环境中，this默认绑定到window。

隐式绑定：一般地，被直接对象所包含的函数调用时，也称为方法调用，this 隐式绑定到该直接对象。隐式丢失：隐式丢失是指被隐式绑定的函数丢失绑定对象，从而默认绑定到 window。显式绑定：通过call()、apply()、bind()方法把对象绑定到this上，叫做显式绑定。

new绑定：如果函数或者方法调用之前带有关键字new，它就构成构造函数调用。

对于this绑定来说，称为new绑定。

【1】构造函数通常不使用return关键字，它们通常初始化新对象，当构造函数的函数体执行完毕时，它会显式返回。在这种情况下，构造函数调用表达式的计算结果就是这个新对象的值。

【2】如果构造函数使用return语句但没有指定返回值，或者返回一个原始值，那么这时将忽略返回值，同时使用这个新对象作为调用结果。

【3】如果构造函数显式地使用return语句返回一个对象，那么调用表达式的值就是这个对象。

## 暂停死区

在代码块内，使用let、const命令声明变量之前，该变量都是不可用的。这在语法上，称为"暂时性死区"。

## AngularJS双向绑定原理



Angular将双向绑定转换为一堆watch表达式，然后递归这些表达式检查是否发生过变化，如果变了则执行相应的watcher函数（指view上的指令，如ng-bind， ng-show等或是{{}}）。等到model中的值不再发生变化，也就不会再有watcher

被触发，一个完整的digest循环就完成了。

Angular中在view上声明的事件指令，如：ng-click、ng-change等，会将浏览

器的事件转发给$scope上相应的model的响应函数。等待相应函数改变model，紧接着触发脏检查机制刷新view。

watch表达式：可以是一个函数、可以是$scope上的一个属性名，也可以是一个字符串形式的表达式。$watch函数所监听的对象叫做watch表达式。watcher 函数：指在view上的指令（ngBind，ngShow、ngHide等）以及{{}}表达式，他

们所注册的函数。每一个watcher对象都包括：监听函数，上次变化的值，获取

监听表达式的方法以及监听表达式，最后还包括是否需要使用深度对比

（angular.equals()）

## 写一个深度拷贝

```js
function deepClone(obj){
    var copy;
    switch(typeof obj){
        case "undefined":break;
        case "number":
            copy = obj-0;
            break;
        case "string":
            copy = obj+"";
            break;
        case "boolean":
            copy = obj;
            break;
        case "object":
            if(Object.prototype.toString.call(obj).slice(8,-1) === "Array"){
                copy = [];
                for(var i=0;i<obj.length;i++){
                    copy.push(deepClone(obj[i]));
                }
            }else{
                copy = {};
                for(var j in obj){
                    copy[j] = deepClone(obj[j]);
                }
            }
            break;
        default:
            copy = obj;
            break;
    }
    return copy;
}
```

## 简历中提到了requestAnimationFrame，请问是怎么使用的

requestAnimationFrame() 方法告诉浏览器您希望执行动画并请求浏览器在下一次重绘之前调用指定的函数来更新动画。该方法使用一个回调函数作为参数，这个回调函数会在浏览器重绘之前调用。

## 有一个游戏叫做Flappy Bird，就是一只小鸟在飞，前面是无尽的沙漠，上下不断有钢管生成，你要躲避钢管。然后小明在玩这个游戏时候老是卡顿甚至崩溃，说出原因（3-5个）以及解决办法（3-5个）

原因可能是：

1）内存溢出问题。 2）资源过大问题。 3）资源加载问题。

4）canvas绘制频率问题

解决办法：

1. 针对内存溢出问题，我们应该在钢管离开可视区域后，销毁钢管，让垃圾收集器回收钢管，因为不断生成的钢管不及时清理容易导致内存溢出游戏崩溃。
2. 针对资源过大问题，我们应该选择图片文件大小更小的图片格式，比如使用 webp、png格式的图片，因为绘制图片需要较大计算量。
3. 针对资源加载问题，我们应该在可视区域之前就预加载好资源，如果在可视区域生成钢管的话，用户的体验就认为钢管是卡顿后才生成的，不流畅。
4. 针对canvas绘制频率问题，我们应该需要知道大部分显示器刷新频率为60 次/s,因此游戏的每一帧绘制间隔时间需要小于1000/60=16.7ms，才能让用户觉得不卡顿。

（注意因为这是单机游戏，所以回答与网络无关）

## 什么是按需加载

当用户触发了动作时才加载对应的功能。触发的动作，是要看具体的业务场景而言，包括但不限于以下几个情况：鼠标点击、输入文字、拉动滚动条，鼠标移动、窗口大小更改等。加载的文件，可以是JS、图片、CSS、HTML等。

## 说一下什么是virtual dom

用JavaScript 对象结构表示 DOM 树的结构；然后用这个树构建一个真正的 DOM 树，插到文档当中 当状态变更的时候，重新构造一棵新的对象树。然后用新的树和旧的树进行比较，记录两棵树差异 把所记录的差异应用到所构建的真正的DOM树上，视图就更新了。Virtual DOM 本质上就是在 JS 和 DOM 之间做了一个**缓存**。

## webpack用来干什么的

webpack 是一个现代 JavaScript 应用程序的静态模块打包器(module bundler)。当 webpack 处理应用程序时，它会递归地构建一个依赖关系图 (dependencygraph)，其中包含应用程序需要的每个模块，然后将所有这些模块打包成一个或多个bundle。

## ant-design优点和缺点

优点：组件非常全面，样式效果也都比较不错。

缺点：框架自定义程度低，默认UI风格修改困难。



## 写一个函数，第一秒打印1，第二秒打印2



两个方法，第一个是用let块级作用域

for(let i=0;i<5;i++){ setTimeout(function(){ console.log(i)

},1000*i)

}

第二个方法闭包

for(var i=0;i<5;i++){

(function(i){

setTimeout(function(){ console.log(i)

},1000*i)

})(i)

}





## 什么是事件监听

addEventListener()方法，用于向指定元素添加事件句柄，它可以更简单的控制事件，语法为

element.addEventListener(event, function, useCapture); 第一个参数是事件的类型(如 "click" 或 "mousedown").

第二个参数是事件触发后调用的函数。

第三个参数是个布尔值用于描述事件是冒泡还是捕获。该参数是可选的。

事件传递有两种方式，冒泡和捕获

事件传递定义了元素事件触发的顺序，如果你将P元素插入到div元素中，用户点击P元素，

在冒泡中，内部元素先被触发，然后再触发外部元素，捕获中，外部元素先被触发，在触发内部元素，

## 介绍一下promise，及其底层如何实现

Promise是一个对象，保存着未来将要结束的事件，她有两个特征:

1. 对象的状态不受外部影响，Promise对象代表一个异步操作，有三种状态， pending进行中，fulfilled已成功，rejected已失败，只有异步操作的结果，才可以决定当前是哪一种状态，任何其他操作都无法改变这个状态，这也就是 promise名字的由来。
2. 一旦状态改变，就不会再变，promise对象状态改变只有两种可能，从pending 改到fulfilled或者从pending改到rejected，只要这两种情况发生，状态就凝固了，不会再改变，这个时候就称为定型resolved,

Promise的基本用法：

let promise1 = new Promise(function(resolve,reject){ setTimeout(function(){ resolve('ok')

},1000) }) promise1.then(function success(val){ console.log(val)

})

最简单代码实现promise

class PromiseM { constructor (process) { this.status = 'pending' this.msg = '' process(this.resolve.bind(this), this.reject.bind(this)) return this } resolve (val) { this.status = 'fulfilled' this.msg = val } reject (err) { this.status = 'rejected' this.msg = err } then (fufilled, reject) { if(this.status === 'fulfilled') { fufilled(this.msg) } if(this.status === 'rejected') { reject(this.msg) }

}

}

//测试代码

var mm=new PromiseM(function(resolve,reject){ resolve('123'); }); mm.then(function(success){ console.log(success); },function(){ console.log('fail!'); });

## bootstrap清除浮动的方法



.clearfix:before, .clearfix:after { content: " "; display: table;}

.clearfix:after { clear: both;}

/**

\* For IE 6/7 only

*/

.clearfix {*zoom: 1;}

:after伪类在元素末尾插入了一个包含空格的字符，并设置display为table

display:table会创建一个匿名的table-cell，从而触发块级上下文（BFC），

因为容器内float的元素也是BFC，由于BFC有不能互相重叠的特性，并且设置了clear:both，:after插入的元素会被挤到容器底部，从而将容器撑高。并且设置display:table后，content中的空格字符会被渲染为0*0的空白元素，不会占用页面空间。

content 包含一个空格，是为了解决 Opera 浏览器的 BUG。当 HTML 中包含 contenteditable属性时，如果content没有包含空格，会造成清除浮动元素的顶部、底部有一个空白（设置font-size：0也可以解决这个问题）。

:after伪类的设置已经达到了清除浮动的目的，但还要设置:before伪类，原因如下

:before的设置也触发了一个BFC，由于BFC有内部布局不受外部影响的特性，因此:before的设置可以阻止margin-top的合并。

这样做，其一是为了和其他清除浮动的方式的效果保持一致；其二，是为了与 ie6/7下设置zoom：1后的效果一致（即阻止margin-top合并的效果）。

zoom: 1用于在ie6/7下触发haslayout和contain floats

## 说说C++,Java，JavaScript这三种语言的区别



从静态类型还是动态类型来看：

静态类型，编译的时候就能够知道每个变量的类型，编程的时候也需要给定类型，如Java中的整型int，浮点型float等。C、C++、Java都属于静态类型语言。动态类型，运行的时候才知道每个变量的类型，编程的时候无需显示指定类型，如JavaScript中的var、PHP中的$。JavaScript、Ruby、Python都属于动态类型语言。

静态类型还是动态类型对语言的性能有很大影响。

对于静态类型，在编译后会大量利用已知类型的优势，如int类型，占用4个字节，编译后的代码就可以用内存地址加偏移量的方法存取变量，而地址加偏移量的算法汇编很容易实现。

对于动态类型，会当做字符串通通存下来，之后存取就用字符串匹配。

从编译型还是解释型来看：

编译型语言，像C、C++，需要编译器编译成本地可执行程序后才能运行，由开发人员在编写完成后手动实施。用户只使用这些编译好的本地代码，这些本地代码由系统加载器执行，由操作系统的CPU直接执行，无需其他额外的虚拟机等。

源代码=》抽象语法树=》中间表示=》本地代码

解释性语言，像JavaScript、Python，开发语言写好后直接将代码交给用户，用户使用脚本解释器将脚本文件解释执行。对于脚本语言，没有开发人员的编译过程，当然，也不绝对。

源代码=》抽象语法树=》解释器解释执行。

对于JavaScript，随着Java虚拟机JIT技术的引入，工作方式也发生了改变。可以将抽象语法树转成中间表示（字节码），再转成本地代码，如 JavaScriptCore，这样可以大大提高执行效率。也可以从抽象语法树直接转成本地代码，如V8

Java语言，分为两个阶段。首先像C++语言一样，经过编译器编译。和C++的不同，C++编译生成本地代码，Java编译后，生成字节码，字节码与平台无关。第二阶段，由Java的运行环境也就是Java虚拟机运行字节码，使用解释器执行这些代码。一般情况下，Java虚拟机都引入了JIT技术，将字节码转换成本地代码来提高执行效率。

注意，在上述情况中，编译器的编译过程没有时间要求，所以编译器可以做大量的代码优化措施。

对于JavaScript与Java它们还有的不同：

对于Java，Java语言将源代码编译成字节码，这个同执行阶段是分开的。也就是从源代码到抽象语法树到字节码这段时间的长短是无所谓的。

对于JavaScript，这些都是在网页和JavaScript文件下载后同执行阶段一起在网页的加载和渲染过程中实施的，所以对于它们的处理时间有严格要求。

## js原型链，原型链的顶端是什么？Object的原型是什么？Object的原型的原型是什么？在数组原型链上实现删除数组重复数据的方法todo

能够把这个讲清楚弄明白是一件很困难的事，

首先明白原型是什么，在ES6之前，JS没有类和继承的概念，JS是通过原型来实现继承的，在JS中一个构造函数默认带有一个prototype属性，这个的属性值是一个对象，同时这个prototype对象自带有一个constructor属性，这个属性指向这个构造函数，同时每一个实例都会有一个_proto_属性指向这个 prototype对象，我们可以把这个叫做隐式原型，我们在使用一个实例的方法的时候，会先检查这个实例中是否有这个方法，没有的话就会检查这个prototype 对象是否有这个方法，

基于 这个 规则 ，如果 让原型对 象指 向另一个类型的 实例， 即 constructor1.protoytpe=instance2，这时候如果试图引用constructor1构造的实例instance1的某个属性p1,

首先会在 instance1 内部属性中找一遍，接着会在 instance1._proto_

（constructor1.prototype）即是instance2中寻找p1

搜 寻 轨 迹 ： instance1->instance2->constructor2.prototype ... ...

->Object.prototype;这即是原型链，原型链顶端是Object.prototype

补充学习：

每个函数都有一个prototype属性，这个属性指向了一个对象，这个对象正是调用该函数而创建的实例的原型，那么什么是原型呢，可以这样理解，每一个 JavaScript对象在创建的时候就会预制管理另一个对象，这个对象就是我们所说的原型，每一个对象都会从原型继承属性，如图：

![](media/image10.jpg){width="5.383333333333334in" height="1.9333333333333333in"}

那么怎么表示实例与实例原型的关系呢，这时候就要用到第二个属性_proto_ 这是每一个JS对象都会有的一个属性，指向这个对象的原型，如图：

![](media/image11.jpg){width="5.633333333333334in" height="2.8366666666666664in"}

既然实例对象和构造函数都可以指向原型，那么原型是否有属性指向构造函数或者实例呢，指向实例是没有的，因为一个构造函数可以生成多个实例，但是原型有属性可以直接指向构造函数，通过constructor即可

接下来讲解实例和原型的关系：

当读取实例的属性时，如果找不到，就会查找与对象相关的原型中的属性，如果还查不到，就去找原型的原型，一直找到最顶层，那么原型的原型是什么呢，首先，原型也是一个对象，既然是对象，我们就可以通过构造函数的方式创建它，所以原型对象就是通过Object构造函数生成的，如图：

![](media/image12.jpg){width="4.583333333333333in" height="3.7in"}

那 么 Object.prototype 的 原 型 呢 ， 我 们 可 以 打 印 console.log(Object.prototype.__proto__ === null)，返回true

null表示没有对象，即该处不应有值，所以Object.prototype没有原型，如图：

图 中 这 条 蓝 色 的 线 即 是 原 型 链 ，

![](media/image13.jpg){width="4.455in" height="3.966666666666667in"}

最后补充三点：

constructor： function Person(){

} var person = new Person(); console.log(Person === person.constructor);

原本person中没有constructor属性，当不能读取到constructor属性时，会从person的原型中读取，所以指向构造函数Person

__proto__：

绝大部分浏览器支持这个非标准的方法访问原型，然而它并不存在与

Person.prototype中，实际上它来自Object.prototype，当使用obj.__proto__ 时，可以理解为返回来Object.getPrototype(obj)

继承：

前面说到，每个对象都会从原型继承属性，但是引用《你不知道的JS》中的话，继承意味着复制操作，然而JS默认不会复制对象的属性，相反，JS只是在两个对象之间创建一个关联，这样子一个对象就可以通过委托访问另一个对象的属性和函数，所以与其叫继承，叫委托更合适，

## 什么是js的闭包？有什么作用，用闭包写个单例模式

MDN对闭包的定义是：闭包是指那些能够访问自由变量的函数，自由变量是指在函数中使用的，但既不是函数参数又不是函数的局部变量的变量，由此可以看出，闭包=函数+函数能够访问的自由变量，所以从技术的角度讲，所有JS函数都是闭包，但是这是理论上的闭包，还有一个实践角度上的闭包，从实践角度上来说，只有满足1）即使创建它的上下文已经销毁，它仍然存在，2）在代码中引入了自由变量，才称为闭包。

闭包的应用：

1. 模仿块级作用域
2. 保存外部函数的变量
3. 封装私有变量

单例模式：

var Singleton = (function(){ var instance;

var CreateSingleton = function (name) { this.name = name;

if(instance) { return instance;

}

// 打印实例名字

this.getName(); // instance = this; // return instance; return instance = this;

}

// 获取实例的名字

CreateSingleton.prototype.getName = function() { console.log(this.name) } return CreateSingleton;

})();

// 创建实例对象1

var a = new Singleton('a');

// 创建实例对象2

var b = new Singleton('b'); console.log(a===b);

## promise+Generator+Async的使用

Promise

解决的问题:回调地狱

Promise规范:

promise有三种状态，等待（pending）、已完成（fulfilled/resolved）、已

拒绝（rejected）.Promise的状态只能从"等待"转到"完成"或者"拒绝"，

不能逆向转换，同时"完成"和"拒绝"也不能相互转换.

promise 必须提供一个 then 方法以访问其当前值、终值和据因。

promise.then(resolve, reject),resolve 和 reject 都是可选参数。如果

resolve 或reject 不是函数，其必须被忽略. then 方法必须返回一个 promise 对象.

使用:

实例化promise对象需要传入函数(包含两个参数),resolve和reject,内部确定状态.resolve和reject函数可以传入参数在回调函数中使用. resolve和reject都是函数,传入的参数在then的回调函数中接收.

var promise = new Promise(function(resolve, reject) { setTimeout(function(){ resolve('好哈哈哈哈');

}); }); promise.then(function(val){ console.log(val) })

then接收两个函数,分别对应resolve和reject状态的回调,函数中接收实例化时传入的参数.

promise.then(val=>{ //resolved

},reason=>{

//rejected })

catch相当于.then(null, rejection)

当then中没有传入rejection时,错误会冒泡进入catch函数中,若传入了 rejection,则错误会被rejection捕获,而且不会进入catch.此外,then中的回

调函数中发生的错误只会在下一级的then中被捕获,不会影响该promise的状

态.

new Promise((resolve,reject)=>{ throw new Error('错误')

}).then(null,(err)=>{ console.log(err,1);//此处捕获

}).catch((err)=>{ console.log(err,2); });

// 对比

new Promise((resolve,reject)=>{ throw new Error('错误')

}).then(null,null).catch((err)=>{ console.log(err,2);//此处捕获 });

// 错误示例

new Promise((resolve,reject)=>{ resolve('正常'); }).then((val)=>{

throw new Error('回调函数中错误')

},(err)=>{ console.log(err,1); }).then(null,(err)=>{ console.log(err,2);//此处捕获,也可用catch

});

两者不等价的情况:

此时，catch捕获的并不是p1的错误，而是p2的错误，

p1().then(res=>{

return p2()//p2返回一个promise对象

}).catch(err=> console.log(err))

一个错误捕获的错误用例:

该函数调用中即使发生了错误依然会进入then中的resolve的回调函数,因为函数p1中实例化promise对象时已经调用了catch,若发生错误会进入catch中, 此时会返回一个新的promise,因此即使发生错误依然会进入p1函数的then链

中的resolve回调函数.

function p1(val){ return new Promise((resolve,reject)=>{ if(val){

var len = val.length;//传入null会发生错误,进入catch捕获错误

resolve(len); }else{ reject(); } }).catch((err)=>{ console.log(err) }) }; p1(null).then((len)=>{ console.log(len,'resolved'); },()=>{ console.log('rejected'); }).catch((err)=>{ console.log(err,'catch');

})

Promise回调链:

promise能够在回调函数里面使用 return 和 throw， 所以在then中可以 return出一个promise对象或其他值，也可以throw出一个错误对象，但如果没有return，将默认返回 undefined，那么后面的then中的回调参数接收到的

将是undefined.

function p1(val){ return new Promise((resolve,reject)=>{ val==1?resolve(1):reject() }) }; function p2(val){ return new Promise((resolve,reject)=>{ val==2?resolve(2):reject(); }) }; let promimse = new Promise(function(resolve,reject){ resolve(1) })

.then(function(data1) {

return p1(data1)//如果去掉return,则返回undefined而不是p1的返回值,会

导致报错

}) .then(function(data2){ return p2(data2+1)

})

.then(res=>console.log(res))

Generator函数： generator函数使用:

1. 分段执行，可以暂停
2. 可以控制阶段和每个阶段的返回值
3. 可以知道是否执行到结尾

function* g() { var o = 1; yield o++; yield o++;

}

var gen = g(); console.log(gen.next()); // Object {value: 1, done: false} var xxx = g(); console.log(gen.next()); // Object {value: 2, done: false} console.log(xxx.next()); // Object {value: 1, done: false} console.log(gen.next()); // Object {value: undefined, done: true}

generator和异步控制:

利用Generator函数的暂停执行的效果，可以把异步操作写在yield语句里面，等到调用next方法时再往后执行。这实际上等同于不需要写回调函数了，因为异步操作的后续操作可以放在yield语句下面，反正要等到调用next方法时再执行。所以，Generator函数的一个重要实际意义就是用来处理异步操作，改写回调函数。

async和异步: 用法: async 表示这是一个async函数，await只能用在这个函数里面。 await 表示在这里等待异步操作返回结果，再继续执行。

await 后一般是一个promise对象

示例:async用于定义一个异步函数，该函数返回一个Promise。如果async函数返回的是一个同步的值，这个值将被包装成一个理解resolve

的Promise，等同于return Promise.resolve(value)。

await用于一个异步操作之前，表示要"等待"这个异步操作的返回值。await 也可以用于一个同步的值。

let timer = async function timer(){ return new Promise((resolve,reject) => { setTimeout(() => { resolve('500'); },500);

}); } timer().then(result => { console.log(result); //500 }).catch(err => { console.log(err.message); });

//返回一个同步的值

let sayHi = async function sayHi(){ let hi = await 'hello world'; return hi; //等同于return Promise.resolve(hi);

} sayHi().then(result => { console.log(result); });

## 事件委托以及冒泡原理

事件委托是利用冒泡阶段的运行机制来实现的，就是把一个元素响应事件的函数委托到另一个元素，一般是把一组元素的事件委托到他的父元素上，委托的优点是：

1）减少内存消耗，节约效率 2）动态绑定事件

事件冒泡，就是元素自身的事件被触发后，如果父元素有相同的事件，如onclick 事件，那么元素本身的触发状态就会传递，也就是冒到父元素，父元素的相同事件也会一级一级根据嵌套关系向外触发，直到document/window，冒泡过程结束。

## 深浅拷贝的区别和实现

>  数组的浅拷贝：
>
> 如果是数组，我们可以利用数组的一些方法，比如slice，concat方法返回一个新数组的特性来实现拷贝，但假如数组嵌套了对象或者数组的话，使用concat 方法克隆并不完整，如果数组元素是基本类型，就会拷贝一份，互不影响，而如果是对象或数组，就会只拷贝对象和数组的引用，这样我们无论在新旧数组进行了修改，两者都会发生变化，我们把这种复制引用的拷贝方法称为浅拷贝，
>
> 深拷贝就是指完全的拷贝一个对象，即使嵌套了对象，两者也互相分离，修改一个对象的属性，不会影响另一个
>
> 如何深拷贝一个数组：
>
> 1）这里介绍一个技巧，不仅适用于数组还适用于对象！那就是：
>
> var arr = ['old', 1, true, ['old1', 'old2'], {old: 1}] var new_arr = JSON.parse( JSON.stringify(arr) ); console.log(new_arr);
>
> 原理是JOSN对象中的stringify可以把一个js对象序列化为一个JSON字符串， parse可以把JSON字符串反序列化为一个js对象，通过这两个方法，也可以实现对象的深复制。
>
> 但是这个方法不能够拷贝函数
>
> 浅拷贝的实现：
>
> 以上三个方法concat,slice ,JSON.stringify都是技巧类，根据实际项目情况选择使用，我们可以思考下如何实现一个对象或数组的浅拷贝，遍历对象，然后把属性和属性值都放在一个新的对象里即可。
>
> var shallowCopy = function(obj) {
>
> // 只拷贝对象
>
> if (typeof obj !== 'object') return;
>
> // 根据obj的类型判断是新建一个数组还是对象
>
> var newObj = obj instanceof Array ? [] : {};
>
> // 遍历obj，并且判断是obj的属性才拷贝
>
> for (var key in obj) {
>
> if (obj.hasOwnProperty(key)) { newObj[key] = obj[key];
>
> } } return newObj;
>
> }
>
> 深拷贝的实现：那如何实现一个深拷贝呢？说起来也好简单，我们在拷贝的时候判断一下属性值的类型，如果是对象，我们递归调用深拷贝函数不就好了~
>
> var deepCopy = function(obj) { if (typeof obj !== 'object') return; var newObj = obj instanceof Array ? [] : {}; for (var key in obj) {
>
> if (obj.hasOwnProperty(key)) { newObj[key] = typeof obj[key] === 'object' ? deepCopy(obj[key]) : obj[key]; } } return newObj; }

## JS中string的startwith和indexof两种方法的区别

JS中startwith函数，其参数有3个，stringObj,要搜索的字符串对象，str，搜索的字符串，position，可选，从哪个位置开始搜索，如果以position开始的字符串以搜索字符串开头，则返回true，否则返回false Indexof函数，indexof函数可返回某个指定字符串在字符串中首次出现的位置

## js字符串转数字的方法

通过函数parseInt（），可解析一个字符串，并返回一个整数，语法为parseInt

（string ,radix）

string：被解析的字符串

radix：表示要解析的数字的基数，默认是十进制，如果radix<2或>36,则返回

NaN

## let const var的区别 ，什么是块级作用域，如何用 ES5的方法实现块级作用域（立即执行函数），ES6 呢

提起这三个最明显的区别是var声明的变量是全局或者整个函数块的，而 let,const声明的变量是块级的变量，var声明的变量存在变量提升，let,const 不存在，let声明的变量允许重新赋值，const不允许

## ES6箭头函数的特性



ES6 增加了箭头函数，基本语法为 let func = value => value; 相当于

let func = function (value) { return value;

};

## 箭头函数和普通函数的区别

- 函数体内的 this 对象，就是定义时所在的对象，而不是使用时所在的对 象。
- 不可以使用 arguments 对象，该对象在函数体内不存在。如果要用，可 以用 rest 参数代替。
- 不可以使用 yield 命令，因此箭头函数不能用作 Generator 函数。
- 不可以使用 new 命令，因为：
  -  1.没有自己的 this，无法调用 call，apply。 
  -  2.没有 prototype 属性 ，而 new 命令在执行时需要将构造函数 的 prototype 赋值给新的对象的 `__proto__`

>  首先我们来看这样一道题：
>
> setTimeout(function() { console.log(1) }, 0); new Promise(function(resolve, reject) { console.log(2)
>
> for (var i = 0; i < 10000; i++) { if(i === 10) {console.log(10)} i == 9999 && resolve();
>
> } console.log(3) }).then(function() { console.log(4) }) console.log(5) 输出答案为2 10 3 5 4 1
>
> 要先弄清楚settimeout（fun,0）何时执行，promise何时执行，then何时执行 settimeout这种异步操作的回调，只有主线程中没有执行任何同步代码的前提下，才会执行异步回调，而settimeout（fun,0）表示立刻执行，也就是用来改变任务的执行顺序，要求浏览器尽可能快的进行回调；
>
> promise何时执行，由上图可知promise新建后立即执行，所以promise构造函数里代码同步执行的，
>
> then方法指向的回调将在当前脚本所有同步任务执行完成后执行，
>
> 那么then为什么比settimeout执行的早呢，因为settimeout（fun,0）不是真的立即执行，
>
> 经过测试得出结论：执行顺序为：同步执行的代码-》promise.then->settimeout

## 有了解过事件模型吗，DOM0级和DOM2级有什么区别， DOM的分级是什么

JSDOM事件流存在如下三个阶段：事件捕获阶段处于目标阶段事件冒泡阶段

JSDOM标准事件流的触发的先后顺序为：先捕获再冒泡，点击DOM节点时，事件传播顺序：事件捕获阶段，从上往下传播，然后到达事件目标节点，最后是冒泡阶段，从下往上传播

DOM节点添加事件监听方法addEventListener，中参数capture可以指定该监听是添加在事件捕获阶段还是事件冒泡阶段，为false是事件冒泡，为true是事件捕获，并非所有的事件都支持冒泡，比如focus，blur等等，我们可以通过 event.bubbles来判断

事件模型有三个常用方法：

event.stopPropagation:阻止捕获和冒泡阶段中，当前事件的进一步传播，

event.stopImmediatePropagetion，阻止调用相同事件的其他侦听器，

event.preventDefault，取消该事件（假如事件是可取消的）而不停止事件的进一步传播

event.target：指向触发事件的元素，在事件冒泡过程中这个值不变

event.currentTarget=this，时间帮顶的当前元素，只有被点击时目标元素的 target才会等于currentTarget，

最后，对于执行顺序的问题，如果DOM节点同时绑定了两个事件监听函数，一个用于捕获，一个用于冒泡，那么两个事件的执行顺序真的是先捕获在冒泡吗，答案是否定的，绑定在被点击元素的事件是按照代码添加顺序执行的，其他函数是先捕获再冒泡

## 平时是怎么调试JS的

一般用Chrome自带的控制台

## JS的基本数据类型有哪些，基本数据类型和引用数据类型的区别，NaN是什么的缩写，JS的作用域类型， undefined==null返回的结果是什么，undefined与null的区别在哪，写一个函数判断变量类型



JS的基本数据类型有字符串，数字，布尔，对象，Null，Undefined,基本数据类型是按值访问的，也就是说我们可以操作保存在变量中的实际的值，基本数据类型和引用数据类型的区别如下：

基本数据类型的值是不可变的，任何方法都无法改变一个基本类型的值，当这个变量重新赋值后看起来变量的值是改变了，但是这里变量名只是指向变量的一个指针，所以改变的是指针的指向改变，该变量是不变的，但是引用类型可以改变

基本数据类型不可以添加属性和方法，但是引用类型可以

基本数据类型的赋值是简单赋值，如果从一个变量向另一个变量赋值基本类型的值，会在变量对象上创建一个新值，然后把该值复制到为新变量分配的位置上，引用数据类型的赋值是对象引用，

基本数据类型的比较是值的比较，引用类型的比较是引用的比较，比较对象的内存地址是否相同

基本数据类型是存放在栈区的，引用数据类型同事保存在栈区和堆区

NaN是JS中的特殊值，表示非数字，NaN不是数字，但是他的数据类型是数字，它不等于任何值，包括自身，在布尔运算时被当做false，NaN与任何数运算得到的结果都是NaN，党员算失败或者运算无法返回正确的数值的就会返回NaN，一些数学函数的运算结果也会出现NaN

JS的作用域类型：

一般认为的作用域是词法作用域，此外JS还提供了一些动态改变作用域的方法

常见的作用域类型有：

1. 函数作用域，如果在函数内部我们给未定义的一个变量赋值，这个变量会转变成为一个全局变量，
2. 块作用域：块作用域吧标识符限制在{}中，

改变函数作用域的方法：

eval（），这个方法接受一个字符串作为参数，并将其中的内容视为好像在书写时就存在于程序中这个位置的代码，

with关键字：通常被当做重复引用同一个对象的多个属性的快捷方式

undefined与null：目前null和undefined基本是同义的，只有一些细微的差别，null表示没有对象，undefined表示缺少值，就是此处应该有一个值但是还没有定义

undefined == null；//返回值是true

undefined === null; //返回值是false 此外了解== 和===的区别：

在做==比较时。不同类型的数据会先转换成一致后在做比较，===中如果类型不一致就直接返回false，一致的才会比较类型判断函数，使用typeof即可，首先判断是否为null，之后用typeof哦按段，如果是object的话，再用array.isarray判断是否为数组，如果是数字的话用isNaN判断是否是NaN即可

扩展学习：

JS采用的是词法作用域，也就是静态作用域，所以函数的作用域在函数定义的时候就决定了，

看如下例子： var value = 1;

function foo() {

console.log(value);

}

function bar() {

var value = 2; foo();

}

bar();

假设JavaScript采用静态作用域，让我们分析下执行过程：

执行foo 函数，先从 foo 函数内部查找是否有局部变量 value，如果没有，就根据书写的位置，查找上面一层的代码，也就是 value 等于 1，所以结果会打印 1。

假设JavaScript采用动态作用域，让我们分析下执行过程：

执行foo 函数，依然是从 foo 函数内部查找是否有局部变量 value。如果没有，就从调用函数的作用域，也就是 bar 函数内部查找 value 变量，所以结果会打印 2。前面我们已经说了，JavaScript采用的是静态作用域，所以这个例子的结果是1。

## setTimeout(fn,100);100毫秒是如何权衡的

setTimeout()函数只是将事件插入了任务列表，必须等到当前代码执行完，主线程才会去执行它指定的回调函数，有可能要等很久，所以没有办法保证回调函数一定会在setTimeout指定的时间内执行，100毫秒是插入队列的时间+等待的时间

## 写一个newBind函数，完成bind的功能

bind（）方法，创建一个新函数，当这个新函数被调用时，bind（）的第一个参数将作为它运行时的this，之后的一序列参数将会在传递的实参前传入作为它的参数

Function.prototype.bind2 = function (context) { if (typeof this !== "function") { throw new Error("Function.prototype.bind - what is trying to be bound is not callable");

} var self = this; var args = Array.prototype.slice.call(arguments, 1); var fNOP = function () {}; var fbound = function () {

self.apply(this instanceof self ? this : context,

args.concat(Array.prototype.slice.call(arguments))); } fNOP.prototype = this.prototype; fbound.prototype = new fNOP(); return fbound; }

## 怎么获得对象上的属性：比如说通过Object.key（）

>  从ES5开始，有三种方法可以列出对象的属性 for（let I in obj）该方法依次访问一个对象及其原型链中所有可枚举的类型 object.keys:返回一个数组，包括所有可枚举的属性名称
>
> object.getOwnPropertyNames:返回一个数组包含不可枚举的属性.

## 简单讲一讲ES6的一些新特性

ES6在变量的声明和定义方面增加了let、const声明变量，有局部变量的概念，赋值中有比较吸引人的结构赋值，同时ES6对字符串、 数组、正则、对象、函数等拓展了一些方法，如字符串方面的模板字符串、函数方面的默认参数、对象方面属性的简洁表达方式，ES6也 引入了新的数据类型symbol，新的数据结构 set和map,symbol可以通过typeof检测出来，为解决异步回调问题，引入了 promise和 generator，还有最为吸引人了实现Class和模块，通过Class可以更好的面向对象编程，使用模块加载方便模块化编程，当然考虑到 浏览器兼容性，我们在实际开发中需要使用babel进行编译重要的特性：

块级作用域：ES5只有全局作用域和函数作用域，块级作用域的好处是不再需要立即执行的函数表达式，循环体中的闭包不再有问题

rest参数：用于获取函数的多余参数，这样就不需要使用arguments对象了， promise:一种异步编程的解决方案，比传统的解决方案回调函数和事件更合理强大

模块化：其模块功能主要有两个命令构成，export和import，export命令用于规定模块的对外接口，import命令用于输入其他模块提供的功能

## call和apply是用来做什么？

Call和apply的作用是一模一样的，只是传参的形式有区别而已

1)改变this的指向

2)借用别的对象的方法，

调用函数，因为apply，call方法会使函数立即执行

## 了解事件代理吗，这样做有什么好处

事件代理/事件委托：利用了事件冒泡，只指定一个事件处理程序，就可以管理某一类型的事件，

简而言之：事件代理就是说我们将事件添加到本来要添加的事件的父节点，将事件委托给父节点来触发处理函数，这通常会使用在大量的同级元素需要添加同一类事件的时候，比如一个动态的非常多的列表，需要为每个列表项都添加点击事件，这时就可以使用事件代理，通过判断e.target.nodeName来判断发生的具体元素，这样做的好处是减少事件绑定，同事动态的DOM结构任然可以监听，事件代理发生在冒泡阶段

## 给出以下代码，输出的结果是什么？原因？

> for(var i=0;i<5;i++) { setTimeout(function(){ console.log(i);
>
> },1000);
>
> }
>
> console.log(i)  
>
> 在一秒后输出5个5
>
> 每次for循环的时候setTimeout都会执行，但是里面的function则不会执行被放入任务队列，因此放了5次；for循环的5次执行完之后不到1000毫秒；1000 毫秒后全部执行任务队列中的函数，所以就是输出5个5。

## 如果已经有三个promise，A、B和C，想串行执行，该怎么写？

// promise

A.then(B).then(C).catch(...)

// async/await (async ()=>{ await a(); await b(); await c(); })()

## 知道private和public吗

public：public表明该数据成员、成员函数是对所有用户开放的，所有用户都可以直接进行调用

private：private表示私有，私有的意思就是除了class自己之外，任何人都不可以直接使用

##  setTimeout、Promise、Async/Await执行顺序

1、执行console.log('script start')，输出script start；
2、执行setTimeout，是一个异步动作，放入宏任务异步队列中；
3、执行async1()，输出async1 start，继续向下执行；
4、执行async2()，输出async2，并返回了一个promise对象，await让出了线程，把返回的promise加入了微任务异步队列，所以async1()下面的代码也要等待上面完成后继续执行;
5、执行 new Promise，输出promise1，然后将resolve放入微任务异步队列；
6、执行console.log('script end')，输出script end；
7、到此同步的代码就都执行完成了，然后去微任务异步队列里去获取任务
8、接下来执行resolve（async2返回的promise返回的），输出了async1 end。
9、然后执行resolve（new Promise的），输出了promise2。
10、最后执行setTimeout，输出了settimeout。

## js加载过程阻塞，解决方法

指定script标签的async属性。

如果async="async"，脚本相对于页面的其余部分异步地执行（当页面继续进行解析时，脚本将被执行）

如果不使用async 且 defer="defer"：脚本将在页面完成解析时执行

## js对象类型，基本对象类型以及引用对象类型的区别

分为基本对象类型和引用对象类型

基本数据类型：按值访问，可操作保存在变量中的实际的值。基本类型值指的是简单的数据段。基本数据类型有这六种:undefined、null、string、number、 boolean、symbol。

引用类型：当复制保存着对象的某个变量时，操作的是对象的引用，但在为对象添加属性时，操作的是实际的对象。引用类型值指那些可能为多个值构成的对象。

引用类型有这几种：Object、Array、RegExp、Date、Function、特殊的基本包装类型(String、Number、Boolean)以及单体内置对象(Global、Math)。

## 面向对象的继承方式

原型链继承:

核心： 将父类的实例作为子类的原型

特点：

(1)非常纯粹的继承关系，实例是子类的实例，也是父类的实例

(2)父类新增原型方法/原型属性，子类都能访问到

(3)简单，易于实现

缺点：

(1)要想为子类新增属性和方法，不能放到构造器中

(2)无法实现多继承

(3)来自原型对象的所有属性被所有实例共享

(4)创建子类实例时，无法向父类构造函数传参

构造继承:

核心：使用父类的构造函数来增强子类实例，等于是复制父类的实例属性给子类

（没用到原型）

特点：

(1)解决了子类实例共享父类引用属性的问题

(2)创建子类实例时，可以向父类传递参数

(3)可以实现多继承（call多个父类对象）

缺点：

(1)实例并不是父类的实例，只是子类的实例

(2)只能继承父类的实例属性和方法，不能继承原型属性/方法

(3)无法实现函数复用，每个子类都有父类实例函数的副本，影响性能实例继承:

核心：为父类实例添加新特性，作为子类实例返回

特点：

不限制调用方式，不管是new 子类()还是子类(),返回的对象具有相同的效果缺点：

(1)实例是父类的实例，不是子类的实例

(2)不支持多继承

拷贝继承特点：

支持多继承

缺点：

效率较低，内存占用高（因为要拷贝父类的属性）

组合继承

核心：通过调用父类构造，继承父类的属性并保留传参的优点，然后通过将父类实例作为子类原型，实现函数复用特点：

(1)可以继承实例属性/方法，也可以继承原型属性/方法

(2)既是子类的实例，也是父类的实例

(3)不存在引用属性共享问题

(4)可传参

(5)函数可复用

寄生组合继承:

核心：通过调用父类构造，继承父类的属性并保留传参的优点，然后通过将父类实例作为子类原型，实现函数复用

## 引用类型常见的对象

Object、Array、RegExp、Date、Function、特殊的基本包装类型(String、Number、

Boolean)以及单体内置对象(Global、Math)等

## class

ES6提供了更接近传统语言的写法，引入了Class（类）这个概念，作为对象的模板。通过class关键字，可以定义类。

## new操作符原理

1)  创建一个类的实例：创建一个空对象obj，然后把这个空对象的__proto__设置为构造函数的prototype。

2)  初始化实例：构造函数被传入参数并调用，关键字this被设定指向该实例 obj。

3)返回实例obj。

## 箭头函数获取arguments

可用...rest参数获取

## Promise

Promise对象是CommonJS工作组提出的一种规范，目的是为异步编程提供统一接口。每一个异步任务返回一个Promise对象，该对象有一个then方法，允许指定回调函数。

f1().then(f2);

一个promise可能有三种状态：等待（pending）、已完成（resolved，又称

fulfilled）、已拒绝（rejected）。 promise必须实现then方法（可以说，then就是promise的核心），而且then 必须返回一个promise，同一个promise的then可以调用多次，并且回调的执行顺序跟它们被定义时的顺序一致。

then方法接受两个参数，第一个参数是成功时的回调，在promise由"等待" 态转换到"完成"态时调用，另一个是失败时的回调，在promise由"等待"态转换到"拒绝"态时调用。同时，then可以接受另一个promise传入，也接受一个"类then"的对象或方法，即thenable对象。

promise

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



## 事件代理

事件代理是利用事件的冒泡原理来实现的，何为事件冒泡呢？就是事件从最深的节点开始，然后逐步向上传播事件，举个例子：页面上有这么一个节点树， div>ul>li>a;比如给最里面的a加一个click点击事件，那么这个事件就会一层一层的往外执行，执行顺序a>li>ul>div，有这样一个机制，那么我们给最外面的div加点击事件，那么里面的ul，li，a做点击事件的时候，都会冒泡到最外层的div上，所以都会触发，这就是事件代理，代理它们父级代为执行事件

## 事件循环机制 （Event Loop）

事件循环机制从整体上告诉了我们 JavaScript 代码的执行顺序 Event Loop 即事件循环，是指浏览器或Node 的一种解决 javaScript 单线程运行时不会阻塞的一种机制，也就是我们经常使用**异步**的原理。

先执行宏任务队列，然后执行微任务队列，然后开始下一轮事件循环，继续先执行宏任务队列，再执行微任务队列。

- 宏任务：script/setTimeout/setInterval/setImmediate/ I/O / UI Rendering

- 微任务：process.nextTick()/Promise

上诉的 setTimeout 和 setInterval 等都是任务源，真正进入任务队列的是他们分发的任务。

优先级：

- setTimeout = setInterval 一个队列
- setTimeout 》 setImmediate
- process.nextTick > Promise



## 事件绑定

```html
div1.onclick=function(){};

<button onmouseover=""><button>
```

1.  如果说给同一个元素绑定了两次或者多次相同类型的事件，那么后面的绑定会覆盖前面的绑定

2.  不支持 DOM 事件流 事件捕获阶段=>目标元素阶段=\>事件冒泡阶段

addEventListener

1.  如果说给同一个元素绑定了两次或者多次相同类型的事件，所有的绑定将会依次触发

2.  支持 DOM 事件流的

3.  进行事件绑定传参不需要 on 前缀

## **怎样添加、移除、移动、复制、创建和查找节点**

1.  创建新节点

    1.  createDocumentFragment() // 创建一个DOM片段 
    2.  createElement() // 创建一个具体的元素 
    3.  createTextNode() // 创建一个文本节点

2.  添加、移除、替换、插入 
    1.  appendChild() 
    2.  removeChild()
    3.  replaceChild()
    4.  insertBefore() // 在已有的子节点前插入一个新的子节点

3.  查找

    1.  getElementsByTagName() // 通过标签名称
    2.  getElementsByName() // 通过元素的Name属性的值(IE容错能力较强，会得到一个数组，其中包括id等于name值的)
    3.  getElementById() // 通过元素Id，唯一性





## split() join() 的区别

前者是切割成数组的形式，后者是将数组转换成字符串

## 事件绑定和普通事件有什么区别?传统事件绑定和符合 W3C 标准的事件绑定有什么区别？

div1.onclick=function(){};

\<button onmouseover=""\>\</button\>

1.  如果说给同一个元素绑定了两次或者多次相同类型的事件，那么后面的绑定会覆盖前面的绑定

2.  不支持 DOM 事件流 事件捕获阶段目标元素阶段=\>事件冒泡阶段

addEventListener

1.  如果说给同一个元素绑定了两次或者多次相同类型的事件，所有的绑定将会依次触发

2.  支持 DOM 事件流的

3.  进行事件绑定传参不需要 on 前缀

addEventListener("click",function(){},true);//此时的事件就是在事件冒泡阶段执行 ie9 开始，ie11 edge：addEventListener

ie9 以前：attachEvent/detachEvent

1、进行事件类型传参需要带上 on 前缀 2、这种方式只支持事件冒泡，不支持事件捕获事件绑定是指把事件注册到具体的元素之上，普通事件指的是可以用来注册的事件

## 通用事件绑定/ 编写一个通用的事件监听函数？

onclick和addEventListener

```javascript
function addEvent( obj,type,fn,capture ){
        //console.log("aa");
        if(obj.addEventListener){
            obj.addEventListener("click",clickFn,true);
        }else{
            obj.attachEvent("click",clickFn,true);
        }
    }
    //添加事件
    addEvent(box,"click",clickFn,true);
    //移除事件
    /*
     * 函数名：removeEvent( obj,type,fn,capture )
     * 参数：
     * obj 目标元素
     * type 事件类型
     * fn  指定事件触发调用的函数
     * capture 是否同步
     */
     function removeEvent( obj,type,fn,capture ){
        if( obj.removeEventListener ){
            obj.removeEventListener(type,clickFn,true);
        }else{
            obj.detachEvent("on"+ type,clickFn,true);
        }
     }
     removeEvent(box,"click",clickFn,true);
```



## IE 和 DOM 事件流的区别

1.执行顺序不一样、

2.参数不一样

3.事件加不加on

4.this指向问题

IE9以前：[attachEvent("onclick")、detachEvent](http://www.baidu.com/link?url=fVtfIQaNBwj3KUO_767M8Y2AoHQa2q1pSY0iwTzkigv1ue0E8r5tBI4bezzlCu01KrbygrzNAJ-jw5H8FTc-1a)("onclick") IE9开始跟DOM事件流是一样的，都是addEventListener

## 事件是如何实现的？ 

基于发布订阅模式，就是在浏览器加载的时候会读取事件相关的代码，但是只有实际等到具体的事件触发的时候才会执行。

比如点击按钮，这是个事件（Event），而负责处理事件的代码段通常被称为事件处理程序（Event

Handler），也就是「启动对话框的显示」这个动作。

在 Web 端，我们常见的就是 DOM 事件：

DOM0 级事件，直接在 html 元素上绑定 on-event，比如 onclick，取消的话，dom.onclick = null，同一个事件只能有一个处理程序，后面的会覆盖前面的。

DOM2 级事件，通过 addEventListener 注册事件，通过 removeEventListener 来删除事件，一个事件可以有多个事件处理程序，按顺序执行，捕获事件和冒泡事件

DOM3级事件，增加了事件类型，比如 UI 事件，焦点事件，鼠标事件

## 事件委托概念和实现

让利用事件冒泡的原理，让自己的所触发的事件，让他的父元素代替执行

将事件绑定到父元素

事件代理（ Event Delegation ），又称之为事件委托。是 JavaScript 中常用的绑定事件的常用技巧。顾名思义，"事件代理"即是把原本需要绑定的事件委托给父元素，让父元素担当事件监听的职务。事件代理的原理是DOM元素的事件冒泡。使用事件代理的好处是可以提高性能、可以大量节省内存占用，减少事件注册，比如在 table上代理所有 td 的 click 事件就非常棒可以实现当新增子对象时无需再次对其绑定

## 如何阻止事件冒泡和默认事件

e. stopPropagation()

## 当一个DOM节点被点击时候，我们希望能够执行一个函数，应该怎么做？

直接在DOM里绑定事件：\<div onclick="test()"\>\</div\> 在JS里通过onclick绑定：xxx.onclick = test 通过事件添加进行绑定：addEventListener(xxx, 'click', test) 那么问题来了，Javascript的事件流模型都有什么？

"事件冒泡"：事件开始由最具体的元素接受，然后逐级向上传播 

事件捕捉"：事件由最不具体的节点先接收，然后逐级向下，一直到最具体的

"DOM事件流"：三个阶段：事件捕捉，目标阶段，事件冒泡



## "=="和"==="的不同

前者会自动转换类型后者不会

1=="1"

null==undefined

===先判断左右两边的数据类型，如果数据类型不一致，直接返回false 之后才会进行两边值的判断

## intanceOf的原理

**instanceof 主要的实现原理就是只要右边变量的 prototype 在左边变量的原型链上即可。因此，instanceof 在查找的过程中会遍历左边变量的原型链，直到找到右边变量的 prototype，如果查找失败，则会返回 false**

## typeof、construcyor和Object.propotype.toString.call()的区别

| 方式                             | 语法                                 | 优点                                                         | 缺点                                  |
| -------------------------------- | ------------------------------------ | ------------------------------------------------------------ | ------------------------------------- |
| typeof                           | typeof(data) /typeof data            | 返回结果为js基本的数据类型，包括umber、boolean、string、object、undefined、function | 不能判断null、array、regexp、自定义类 |
| constructor                      | data.constructor                     | 能判断自定义类                                               | 不能判断Null、Undefined               |
| Object.propotype.toString.call() | Object.propotype.toString.call(data) | 支持Sring、Array、Number、Boolean、Object、Regexp、Function、Object、Null、Undefined | 不能判断自定义类                      |

## 希望获取到页面中所有的checkbox怎么做？(不使用第三方框架)

var domList = document.getElementsByTagName('input') var checkBoxList = \[\];//返回的所有的checkbox var len = domList.length; //缓存到局部变量 while (len\--) { //使用while的效率会比for循环更高 if (domList\[len\].type == 'checkbox') { checkBoxList.push(domList\[len\]);

}

}

## 设置一个已知ID的DIV的html内容为xxxx，字体颜色设置为黑色(不使用第三方框架)

var dom = document.getElementById("ID"); dom.innerHTML = "xxxx" dom.style.color = "\#000"

## 当一个DOM节点被点击时候，我们希望能够执行一个函数，应该怎么做？

直接在DOM里绑定事件：\<div onclick="test()"\>\</div\> 在JS里通过onclick绑定：xxx.onclick = test 通过事件添加进行绑定：addEventListener(xxx, 'click', test) 那么问题来了，Javascript的事件流模型都有什么？

"事件冒泡"：事件开始由最具体的元素接受，然后逐级向上传播 ["事件捕捉"：事件由最不具体的节点先接收，然后逐](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)级向下，一直到最具体的

"DOM事件流"：三个阶段：事件捕捉，目标阶段，事件冒泡

## 以下代码为何输出undefined

var a; alert(typeof a); // "undefined"

//alert(b); // 报错 b=10;

alert(typeof b);//"number"

解释：Undefined是一个只有一个值的数据类型，这个值就是"undefined"，在使用var 声明变量但并未对其赋值进行初始化时，这个变量的值就是undefined。而b由于未声明将报错。注意未申明的变量和声明了未赋值的是不一样的。

undefined会在以下三种情况下产生：

1.  一个变量定义了却没有被赋值

2.  想要获取一个对象上不存在的属性或者方法:

3.  一个数组中没有被赋值的元素

注意区分undefined跟not defnied(语法错误)是不一样的

## 看下列代码,输出什么？解释typeof检测会返回"object"的原因。

var a = null;

alert(typeof a); //object

解释：null是一个只有一个值的数据类型，这个值就是null。表示一个空指针对象，所以用typeof检测会返回"object"。

## 输出今天的日期，以YYYY-MM-DD的方式，比如今天是2014年9月26日，则输出2014-09-26 todo

```js
var d = new Date();

// 获取年，getFullYear()返回4位的数字

var year = d.getFullYear();

// 获取月，月份比较特殊，0是1月，11是12月

var month = d.getMonth() + 1;

// 变成两位

month = month \< 10 ? \'0\' + month : month;

// 获取日

var day = d.getDate(); day = day 
```

## **foo = foo\|\|bar** ，这行代码是什么意思？为什么要这样写？

这种写法称之为短路表达式if(!foo) foo = bar; //如果foo存在，值不变，否则把bar的值赋给foo。

短路表达式：作为"&&"和"\|\|"操作符的操作数表达式，这些表达式在进行求值时，只要最终的结果已经可以确定是真或假，求值过程便告终止，这称之为短路求值。

注意if条件的真假判定，记住以下是false的情况：

[空字符串、false、undefined、null、0](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

## 看下列代码，将会输出什么?(变量声明提升)

var foo = 1;

> function(){ console.log(foo); var foo = 2;
>
> console.log(foo);

}

> 输出undefined 和 2。上面代码相当于：

var foo = 1;

> function(){ var foo;
>
> console.log(foo); //undefined foo = 2;
>
> console.log(foo); // 2;

}

> 函数声明与变量声明会被JavaScript引擎隐式地提升到当前作用域的顶部，但是只提升名称不会提升赋值部分。

## 用js实现随机选取10--100之间的10个数字，存入一个数组，并排序。

var iArray = \[\]; funtion getRandom(istart, iend){

var iChoice = istart - iend +1;

return Math.floor(Math.random() \* iChoice + istart;

}

Math.random()就是获取0-1之间的随机数（永远获取不到1）

for(var i=0; i\<10; i++){ var result= getRandom(10,100);

iArray.push(result);

} iArray.sort();

## 把两个数组合并，并删除第二个元素。

var array1 = \[\'a\',\'b\',\'c\'\];

[var](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [bArray](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [=](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [\[\'d\',\'e\',\'f\'\];](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) var cArray = array1.concat(bArray); cArray.splice(1,1);

## 正则表达式构造函数var reg=new RegExp("xxx")与正则表达字面量var reg=//有什么不同？匹配邮箱的正则表达式？

当使用RegExp()构造函数的时候，不仅需要转义引号（即\\"表示"），并且还需要双反斜杠（即\\\\表示一个\\）。使用正则表达字面量的效率更高。

邮箱的正则匹配：

var regMail = /\^(\[a-zA-Z0-9\_-\])+@(\[a-zA-Z0-9\_-\])+((.\[a-zA-Z0-9\_-\]{2,3}){1,2})\$/;

## 写一个function，清除字符串前后的空格。（兼容所有浏览器）

使用自带接口trim()，考虑兼容性：

[if](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [(!String.prototype.trim)](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [{](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) String.prototype.trim = function() {

return this.replace(/\^\\s+/, \"\").replace(/\\s+\$/,\"\");

//\\s匹配空白字符：回车、换行、制表符tab 空格

}

}

// test the function var str = \" \\t\\n test string \".trim(); alert(str == \"test string\"); // alerts \"true\" 43、Javascript中callee和caller的作用？ arguments.callee：获得当前函数的引用

caller是返回一个对函数的引用，该函数调用了当前函数；

callee是返回正在被执行的function函数，也就是所指定的function对象的正文。

## 要将页面的状态栏中显示"已经选中该文本框"，下列JavaScript语句正确的是（ A ）

A.  window.status="已经选中该文本框"

B.  document.status="已经选中该文本框"

C.  window.screen="已经选中该文本框"

D.  document.screen="已经选中该文本框"

## 请选择结果为真的表达式：（C）

A.null instanceof Object

B.null === undefined

C.null == undefined

D.NaN == NaN

## typeof 运算符返回值中有一个跟 javascript 数据类型不一致，它是

\_\_\_\_\_\_\_\_"function"\_\_\_\_\_\_\_\_\_。

typeof Number typeof Object

## 定义了一个变量，但没有为该变量赋值，如果alert该变量，javascript 弹出的对话框中显示\_\_\_undefined\_\_\_\_\_\_ 。

## 写出函数DateDemo的返回结果，系统时间假定为今天

> function DateDemo(){
>
> var d, s=\"今天日期是：\";
>
> d = new Date();
>
> s += d.getMonth() + \"/\";
>
> s += d.getDate() + \"/\";
>
> s += d.getFullYear();
>
> return s;}
>
> 结果：今天日期是：7/17/2010

## 阅读以下代码，请分析出结果：

var arr = new Array(1 ,3 ,5); arr\[4\]=\'z\';//\[1,3,5,undefined,'z'\] arr2 = arr.reverse();//arr2=\['z',undefined,5,3,1\];

> //arr=\['z',undefined,5,3,1\]

arr3 = arr.concat(arr2); alert(arr3);

> 弹出提示对话框：z,,5,3,1,z,,5,3,1 **reverse**方法颠倒数组中元素的位置，并返回该数组的引用。

## 完成函数 **showImg()**，要求能够动态根据下拉列表的选项变化，更新图片的显示

> \<body\>
>
> \<script type="text/javascript" \> function showImg (oSel) {
>
> //在此处添加代码
>
> var str = oSel.value;
>
> document.getElementById("pic").src= str+".jpg";
>
> }
>
> \</script\>
>
> \<img id="pic"src="img1.jpg"width="200″ height="200″ /\>
>
> \<br /\>
>
> \<select id="sel"\>
>
> \<option value="img1"\>城市生活\</option\>
>
> \<option value="img2"\>都市早报\</option\>
>
> \<option value="img3"\>青山绿水\</option\> \</select\>\</body\>

##  列举浏览器对象模型BOM里常用的至少4个对象，并列举window对象的常用方法至少5个

> 对象：Window document location screen history navigator
>
> 方法：Alert() confirm() prompt() open() close()

## 简述创建函数的几种方式

第一种（函数声明）：

function sum1(num1,num2){ return num1+num2;

}

第二种（函数表达式）：

var sum2 = function(num1,num2){ return num1+num2;

}

匿名函数：

function(){}:只能自己执行自己

第三种（函数对象方式）：

var sum3 = new Function(\"num1\",\"num2\",\"return num1+num2\");



## 把 Script 标签 放在页面的最底部的body封闭之前 和封闭之后有什么区别？浏览器会如何解析它们？

如果说放在 body 的封闭之前，将会阻塞其他资源的加载如果放在 body 封闭之后，不会影响 body 内元素的加载

## iframe的优缺点？

优点：

1.  解决加载缓慢的第三方内容如图标和广告等的加载问题

2.  Security sandbox

3.  并行加载脚本缺点：

<!-- -->

1.  iframe会阻塞主页面的Onload事件

2.  [即时内容为空，加载也需要时间](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

3.  没有语意

## 请你谈谈Cookie的弊端？

缺点：

1.`Cookie`数量和长度的限制。每个domain最多只能有20条cookie，每个cookie长度不能超过4KB，否则会被截掉。

2.安全性问题。如果cookie被人拦截了，那人就可以取得所有的session信息。即使加密也与事无补，因为拦截者并不需要知道cookie的意义，他只要原样转发cookie就可以达到目的了。

3.有些状态不可能保存在客户端。例如，为了防止重复提交表单，我们需要在服务器端保存一个计数器。如果我们把这个计数器保存在客户端，那么它起不到任何作用。

## js延迟加载的方式有哪些？

1.  defer和async

2.  动态创建DOM方式（创建script，插入到DOM中，加载完毕后callBack）

3.  按需异步载入js

## documen.write和 innerHTML 的区别？

document.write 只能重绘整个页面 innerHTML 可以重绘页面的一部分

## 哪些操作会造成内存泄漏？

内存泄漏指任何对象在您不再拥有或需要它之后仍然存在。

垃圾回收器定期扫描对象，并计算引用了每个对象的其他对象的数量。如果一个对象的引用数量为 0（没有其他对象引用过该对象），或对该对象的惟一引用是循环的，那么该对象的内存即可回收。

1.  setTimeout 的第一个参数使用字符串而非函数的话，会引发内存泄漏。
2.  闭包
3.  控制台日志
4.  循环（在两个对象彼此引用且彼此保留时，就会产生一个循环）



## js内存泄漏的解决方式

- 在退出函数之前，将不用的全局变量删除，或者赋值为null。or 避免变量的循环赋值和引用

## IE和DOM事件流的区别

1.执行顺序不一样、

2.参数不一样

3.事件加不加on 

4.this指向问题

## javascript的本地对象，内置对象和宿主对象

本地对象为array obj regexp等可以new实例化内置对象为gload Math 等不可以实例化的宿主为浏览器自带的document,window 等

## document load 和document ready的区别

Document.onload 是在结构和样式加载完才执行 js

Document.ready原生种没有这个方法，jquery中有 \$().ready(function)





## window.location.search返回的是什么？

查询(参数)部分。除了给动态语言赋值以外，我们同样可以给静态页面,并使用 javascript来获得相信应的参数值

返回值：?ver=1.0&id=timlq 也就是问号后面的！

## window.location.hash 返回的是什么？

锚点 ， 返回值：\#love ；

//url:http://www.sina.com/getage?\#age

这时就返回"\#age"

## window.location.reload() 作用？

刷新当前页面。

## 阻止冒泡函数

> function stopPropagation(e) { e = e \|\| window.event; if(e.stopPropagation) { //W3C阻止冒泡方法
>
> e.stopPropagation();
>
> } else {
>
> e.cancelBubble = true; //IE阻止冒泡方法
>
> } }
>
> document.getElementById(\'need\_hide\').onclick = function(e) { stopPropagation(e);
>
> }



111. 下面输出多少？

> var o1 = new Object();
>
> var o2 = o1;
>
> o2.name = \"CSSer\";
>
> console.log(o1.name);

如果不看答案，你回答真确了的话，那么说明你对javascript的数据类型了解的还是比较清楚了。js中有两种数据类型，分别是：基本数据类型和引用数据类型

（objectArray）。对于保存基本类型值的变量，变量是按值访问的，因为我们操作的是变量实际保存的值。对于保存引用类型值的变量，变量是按引用访问的，[我们操作的是变量值所引用（指向）的对象。答案就清楚了： 输出CSSer;

## JS的继承性

> window.color = \'red\'; var o = {color: \'blue\'};
>
> function sayColor(){ alert(this.color);
>
> }
>
> 考点：1、this的指向
>
> 2、call的用法
>
> sayColor(); //red
>
> sayColor.call(this); //red this指向的是window对象 sayColor.call(window); //red sayColor.call(o); //blue



## 计算字符串字节数：

> new function(s){
>
> if(!arguments.length\|\|!s) return null;
>
> if(\"\"==s) return 0; //无效代码，因为上一句!s已经判断过 var l=0;
>
> for(var i=0;i\<s.length;i++){ if(s.charCodeAt(i)\>255) l+=2; else l+=1; //charCodeAt()得到的是unCode码
>
> } //汉字的unCode码大于 255bit 就是两个字节 alert(l); }(\"hello world!\");

## `var bool = !!2; alert(bool)；`结果是：

> //true;

技巧：双向非操作可以把字符串和数字转换为布尔值。

## 匹配输入的字符：第一个必须是字母或下划线开头，后面就是字母和数字或者下划线构成，长度5-20

> var reg = /\^\[a-zA-Z\_\]\[a-zA-Z0-9\_\]{4,19}/,
>
> name1 = \'leipeng\', name2 = \'0leipeng\', name3 = \'你好leipeng\', name4 = \'hi\'; alert(reg.test(name1)); alert(reg.test(name2)); alert(reg.test(name3)); alert(reg.test(name4));

## 如何在HTML中添加事件，几种方法？

```
1.  标签之中直接添加 onclick=\"fun()\";

2.  JS添加 Eobj.onclick = method;

3.  现代事件 IE9以前： obj.attachEvent(\'onclick\', method)；标准浏览器: obj.addEventListener(\'click\', method, false);
```

## BOM对象有哪些，列举window对象？

window对象 ，是 JS的最顶层对象，其他的 BOM对象都是 window对象的属性；
document对象，文档对象；
location对象，浏览器当前 URL信息；
navigator对象，浏览器本身信息；
screen对象，客户端屏幕信息；
history对象，浏览器访问历史信息；

## 解析URL成一个对象？

> String.prototype.urlQueryString = function(){ var url = this.split(\'?\')\[1\].split(\'&\'), len = url.length;
>
> this.url = {};
>
> for(var i = 0; i \< len; i += 1){
>
> var cell = url\[i\].split(\'=\'), key = cell\[0\], val = cell\[1\];
>
> this.url\[\'\'+key+\'\'\] = val;
>
> } return this.url;
>
> }
>
> var url = \'?name=12&age=23\';
>
> console.log(url.urlQueryString().age);

## 看下列代码输出什么？

> var foo = \"11\"+2-\"1\"; console.log(foo); console.log(typeof foo); 执行完后foo的值为111，foo的类型为Number。

## 看下列代码输出什么？

> var a = new Object(); a.value = 1; b = a;
>
> b.value = 2; alert(a.value);
>
> 执行完后输出结果为2

## 已知数组var stringArray = \[\"This", \"is", \"Baidu", \"Campus"\]， Alert出"This is Baidu Campus"。

> alert(stringArray.join(\" \"))

## 已知有字符串foo=\"get-element-by-id\",写一个function将其转化成驼峰表示法\"getElementById\"。

function combo(msg){ var arr = msg.split(\"-\");

var len = arr.length; //将arr.length存储在一个局部变量可以提高for循环效率

for(var i=1;i\<len;i++){ arr\[i\]=arr\[i\].charAt(0).toUpperCase()+arr\[i\].substr(1,arr\[i\].length-1);

}

msg=arr.join(\"\"); return msg;

}

## 你如何优化自己的代码？

代码重用

避免全局变量（命名空间，封闭空间，模块化mvc..）拆分函数避免函数过于臃肿：单一职责原则

适当的注释，尤其是一些复杂的业务逻辑或者是计算逻辑，都应该写出这个业务逻辑的具体过程内存管理，尤其是闭包中的变量释放

## 请尽可能详尽的解释ajax的工作原理

思路：先解释异步，再解释 ajax 如何使用

Ajax 的原理简单来说通过 XmlHttpRequest 对象来向服务器发异步请求，从服务器获得数据，然后用javascript来操作DOM而更新页面。这其中最关键的一步就是从服务器获得请求数据。

要清楚这个过程和原理，我们必须对 XMLHttpRequest 有所了解。

XMLHttpRequest 是 ajax 的核心机制，它是在 IE5 中首先引入的，是一种支持异步请求的技术。简单的说，也就是 javascript 可以及时向服务器提出请求和处理响应，而不阻塞用户。

达到无刷新的效果。

## 为什么扩展javascript内置对象不是好的做法？

> 因为扩展内置对象会影响整个程序中所使用到的该内置对象的原型属性

## 请解释一下javascript的同源策略

> 域名、协议、端口相同

## 如果设计中使用了非标准的字体，你该如何去实现？

先通过 font-face 定义字体，再引用

```css
@font-face
{
     font-family: myFirstFont;
    src: url(\'Sansation\_Light.ttf\'), url(\'Sansation\_Light.eot\'); /\* IE9+ \*/ 
}
```





## 解释什么是sql注入，xss漏洞



## 约瑟夫环---已知n个人（以编号1，2，3...分别表示）围坐在一张圆桌周围。从编号为k的人开始报数，数到m的那个人出列；他的下一个人又从1开始报数，数到m的那个人又出列；依此规律重复下去，直到圆桌周围的人全部出列。

## 有1到10w这个10w个数，去除2个并打乱次序，如何找出那两个数？

## 如何获取对象 **a** 拥有的所有属性（可枚举的、不可枚举的，不包括继承来的属性）

Object.keys------IE9+

> 或者使用 **for...in** 并过滤出继承的属性 for(o in obj){
>
> if(obj.hasOwnproperty(o)){

//把 o 这个属性放入到一个数组中

}

}

## 三种弹窗的单词以及三种弹窗的功能

alert confirm prompt

## console.log( 8 \| 1 ); 输出值是多少？

> 9

## JavaScript alert(0.4\*0.2);结果是多少？和你预期的一样吗？如果不一样该如何处理？

有误差，应该比准确结果偏大。 一般我会将小数变为整数来处理。当前之前遇到这个问题时也上网查询发现有人用try catch return写了一个函数，

当然原理也是一致先转为整数再计算。看起来挺麻烦的，我没用过。

## **jQuery** 框架中**\$.ajax()**的常用参数有哪些？todo

**type**

> 类型：String
>
> 默认值: \"GET\")。请求方式 (\"POST\" 或 \"GET\")， 默认为 \"GET\"。注意：其它 HTTP 请求方法，如 PUT 和 DELETE 也可以使用，但仅部分浏览器支持。
>
> **url**
>
> 类型：String
>
> 默认值: 当前页地址。发送请求的地址。

**success**

> 类型：Function
>
> 请求成功后的回调函数。
>
> 参数：由服务器返回，并根据 dataType 参数进行处理后的数据；描述状态的字符串。
>
> 这是一个 Ajax 事件。

**options**

> 类型：Object
>
> 可选。AJAX 请求设置。所有选项都是可选的。
>
> **async**
>
> 类型：Boolean
>
> 默认值: true。默认设置下，所有请求均为异步请求。如果需要发送同步请求，请将此选项设置为 false。
>
> 注意，同步请求将锁住浏览器，用户其它操作必须等待请求完成才可以执行。
>
> **beforeSend(XHR)**
>
> 类型：Function 发送请求前可修改 XMLHttpRequest 对象的函数，如添加自定义 HTTP 头。
>
> XMLHttpRequest 对象是唯一的参数。
>
> [这是一个](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [Ajax](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [事件。如果返回](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [false](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [可以取消本次](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) ajax 请求。
>
> **cache**
>
> 类型：Boolean
>
> 默认值: true，dataType 为 script 和 jsonp 时默认为 false。设置为 false 将不缓存此页面。
>
> jQuery 1.2 新功能。

**contentType**

> 类型：String 默认值: \"application/x-www-form-urlencoded\"。发送信息至服务器时内容编码类型。
>
> 默认值适合大多数情况。如果你明确地传递了一个 content-type 给 \$.ajax() 那么它必定会发送给服务器（即使没有数据要发送）。

**data**

> 类型：String
>
> 发送到服务器的数据。将自动转换为请求字符串格式。GET 请求中将附加在 URL 后。查看
>
> processData 选项说明以禁止此自动转换。必须为 Key/Value 格式。如果为数组，jQuery 将自动为不同值对应同一个名称。如 {foo:\[\"bar1\", \"bar2\"\]} 转换为 \'&foo=bar1&foo=bar2\'。
>
> **dataFilter**
>
> 类型：Function
>
> 给 Ajax 返回的原始数据的进行预处理的函数。提供 data 和 type 两个参数：data 是 Ajax 返回的原始数据，type 是调用 jQuery.ajax 时提供的 dataType 参数。函数返回的值将由 jQuery 进一步处理。
>
> **dataType**
>
> 类型：String
>
> 预期服务器返回的数据类型。如果不指定，jQuery 将自动根据 HTTP 包 MIME 信息来智能判断，比如 XML MIME 类型就被识别为 XML。在 1.4 中，JSON 就会生成一个 JavaScript 对象，而 script 则会执行这个脚本。随后服务器端返回的数据会根据这个值解析后，传递给回调函数。可用值:



> **error**
>
> 类型：Function
>
> 默认值: 自动判断 (xml 或 html)。请求失败时调用此函数。
>
> 有以下三个参数：XMLHttpRequest 对象、错误信息、（可选）捕获的异常对象。
>
> 如果发生了错误，错误信息（第二个参数）除了得到 null 之外，还可能是 \"timeout\", \"error\",
>
> \"notmodified\" 和 \"parsererror\"。
>
> 这是一个 Ajax 事件。

## 写一个 **post** 请求并带有发送数据和返回数据的样例todo

## JavaScript数组元素添加、删除、排序等方法有哪些？

Array.concat( ) 连接数组

Array.join() 将数组元素连接起来以构建一个字符串

Array.length 数组的大小

Array.pop( ) 删除并返回数组的最后一个元素

Array.push( ) 给数组添加元素

Array.reverse( ) 颠倒数组中元素的顺序

Array.shift( ) 将元素移出数组

Array.slice( ) 返回数组的一部分

Array.sort( ) 对数组元素进行排序

Array.splice( ) 插入、删除或替换数组的元素

Array.toLocaleString( ) 把数组转换成局部字符串

Array.toString( ) 将数组转换成一个字符串

Array.unshift( ) 在数组头部插入一个元素

## 如何添加html元素的事件，有几种方法？请列举

a、直接在标签里添加：\<div onclick="alert(你好)"\>这是一个层\</div\>

 b、在元素上通过 js 添加: 

c、使用事件注册函数添加 

## 如现在有一个效果，有显示用户头像、用户昵称、用户其他信息；当用户鼠标移到头像上时，会弹出用户的所有信息；如果是你，你会如何实现这个功能，请用代码实现？

## 在Javascript中什么是伪数组？如何将伪数组转化为标准数组？

伪数组（类数组）：无法直接调用数组方法或期望length属性有什么特殊的行为，但仍可以对真正数组遍历方法来遍历它们。典型的是函数的argument参数，还有像调用 [getElementsByTagName,document.childNodes之类的](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png),它们都返回NodeList对象都属于伪数组。

可以使用Array.prototype.slice.call(fakeArray)将数组转化为真正的Array对象。

## 写一个函数可以计算 sum(5,0,-5);输出0; sum(1,2,3,4);输出10;

```js
function calculate(){
   var ans = 0;
   for(var i=0;i<arguments.length;i++){
       let temp = arguments[i];
       ans = ans+temp;
   }
   return ans;
}
console.log(calculate(3,5,7))
```



## 删除与某个字符相邻且相同的字符，比如fdaffdaaklfjklja字符串处理之后成为"fdafdaklfjklja"

```js
function deleteRepeat(str){
    var template = str.split('');
    var temp = template[0];
    var res = []
    res.push(temp);
    if (template.length<=0){
        return template;
    }else{
        for (var i=1;i<template.length;i++){
            if(template[i] != temp){
                res.push(template[i])
                temp = template[i];
            }
        }
    }
    return res.join('');

}
```



## 下列 **JavaScript** 代码执行后，依次 **alert** 的结果是

> (function test(){ var a=b=5; alert(typeof a); alert(typeof b);
>
> })(); alert(typeof a); alert(typeof b);
>
> //number number undefined number

## 程序中捕获异常的方法？

> window.error try{}catch(){}finally{}

## 同步和异步的区别?

同步：阻塞的

> -张三叫李四去吃饭，李四一直忙得不停，张三一直等着，直到李四忙完两个人一块去吃饭 =浏览器向服务器请求数据，服务器比较忙，浏览器一直等着（页面白屏），直到服务器返回数据，浏览器才能显示页面异步：非阻塞的
>
> -张三叫李四去吃饭，李四在忙，张三说了一声然后自己就去吃饭了，李四忙完后自己去吃
>
> =浏览器向服务器请求数据，服务器比较忙，浏览器可以自如的干原来的事情（显示页面），服务器返回数据的时候通知浏览器一声，浏览器把返回的数据再渲染到页面，局部更新

## 如何解决跨域问题?

理解跨域的概念：协议、域名、端口都相同才同域，否则都是跨域

出于安全考虑，服务器不允许ajax跨域获取数据，但是可以跨域获取文件内容，所以基于这一点，可以动态创建script标签，使用标签的src属性访问js文件的形式获取js [脚本，并且这个js脚本中的内容是函数调用，该函数](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)调用的参数是服务器返回的数据，为了获取这里的参数数据，需要事先在页面中定义回调函数，在回调函数中处理服务器返回的数据，这就是解决跨域问题的主流解决方案

## 页面编码和被请求的资源编码如果不一致如何处理？

对于ajax请求传递的参数，如果是get请求方式，参数如果传递中文，在有些浏览器会乱码，不同的浏览器对参数编码的处理方式不同，所以对于get请求的参数需要使用

encodeURIComponent函数对参数进行编码处理，后台开发语言都有相应的解码api。对于post请求不需要进行编码

## 简述ajax 的过程。

1.  创建XMLHttpRequest对象,也就是创建一个异步调用对象
2.  创建一个新的HTTP请求,并指定该HTTP请求的方法、URL及验证信息
3.  设置响应HTTP请求状态变化的函数
4.  发送HTTP请求
5.  获取异步调用返回的数据
6.  使用JavaScript和DOM实现局部刷新

## ajax 是什么?ajax 的交互模型?同步和异步的区别?如何解决跨域问题?

通过异步模式，提升了用户体验

优化了浏览器和服务器之间的传输，减少不必要的数据往返，减少了带宽占用

Ajax在客户端运行，承担了一部分本来由服务器承担的工作，减少了大用户量下的服务器负载。

## Ajax的最大的特点是什么。

Ajax可以实现异步通信效果，实现页面局部刷新，带来更好的用户体验；按需获取数据，节约带宽资源；

## ajax的缺点

- ajax不支持浏览器back按钮。 
- 安全问题 AJAX暴露了与服务器交互的细节。
- 对搜索引擎的支持比较弱。
- 破坏了程序的异常机制。

## 解释jsonp的原理，以及为什么不是真正的ajax

Jsonp并不是一种数据格式，而json是一种数据格式，jsonp是用来解决跨域获取数据的一种解决方案，具体是通过动态创建script标签，然后通过标签的src属性获取js文件中的js脚本，该脚本的内容是一个函数调用，参数就是服务器返回的数据，为了处理这些返回的数据，需要事先在页面定义好回调函数，本质上使用的并不是ajax技术

## ajax请求时，如何解释json数据

> 使用eval() 或者JSON.parse() 鉴于安全性考虑，推荐使用JSON.parse()更靠谱，对数据的安全性更好。

## 请说出三种减低页面加载时间的方法

1.  压缩css、js文件

2.  合并js、css文件，减少http请求

3.  外部js、css文件放在最底下

4.  减少dom操作，尽可能用变量替代不必要的dom操作

## JQuery一个对象可以同时绑定多个事件，这是如何实现的？

jQuery可以给一个对象同时绑定多个事件，低层实现方式是使用addEventListner或 attachEvent兼容不同的浏览器实现事件的绑定，这样可以给同一个对象注册多个事件。

## 知道什么是webkit么? 知道怎么用浏览器的各种工具来调试和debug代码么?

> Webkit是浏览器引擎，包括html渲染和js解析功能，手机浏览器的主流内核，与之相对应的引擎有Gecko（MozillaFirefox 等使用）和Trident（也称MSHTML，IE 使用）。[对于浏览器的调试工具要熟练使用，主要是页面](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)结构分析，后台请求信息查看，js调试工具使用，熟练使用这些工具可以快速提高解决问题的效率

## 如何测试前端代码? 知道BDD, TDD, Unit Test么? 知道怎么测试你的前端工程么(mocha, sinon, jasmin, qUnit..)?

> 了解BDD行为驱动开发与TDD测试驱动开发已经单元测试相关概念，

## 前端 templating(Mustache, underscore, handlebars)是干嘛的, 怎么用?

> Web 模板引擎是为了使用户界面与业务数据（内容）分离而产生的，
>
> Mustache 是一个 logic-less （轻逻辑）模板解析引擎，它的优势在于可以应用在
>
> Javascript、PHP、Python、Perl 等多种编程语言中。
>
> Underscore封装了常用的JavaScript对象操作方法，用于提高开发效率。
>
> Handlebars 是 JavaScript 一个语义模板库，通过对view和data的分离来快速构建
>
> Web模板。

## 编写一个 JavaScript 函数，输入指定类型的选择器(仅需支持 id，class，tagName）三种简单 CSS 选择器，无需兼容组合选择器)可以返回匹配的 DOM 节点，需考虑浏览器兼容性和性能。

> /\*\*\* \@param selector {String} 传入的CSS选择器。\* \@return {Array}\*/
>
> var query = function(selector) { var reg = /\^(\#)?(\\.)?(\\w+)\$/img; var regResult = reg.exec(selector); var result = \[\];
>
> //如果是id选择器
>
> if(regResult\[1\]) { if(regResult\[3\]) { if(typeof document.querySelector === \"function\") { result.push(document.querySelector(regResult\[3\]));
>
> }else { result.push(document.getElementById(regResult\[3\])); }
>
> }
>
> }
>
> //如果是class选择器
>
> else if(regResult\[2\]) { if(regResult\[3\]) { if(typeof document.getElementsByClassName === \'function\') { var doms = document.getElementsByClassName(regResult\[3\]); if(doms) { result = converToArray(doms);
>
> }
>
> }
>
> [//如果不支持getElementsByClassN](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)ame函数 else { var allDoms = document.getElementsByTagName(\"\*\") ; for(var i = 0, len = allDoms.length; i \< len; i++) { if(allDoms\[i\].className.search(new RegExp(regResult\[2\])) \> -1) { result.push(allDoms\[i\]);
>
> }
>
> }
>
> }
>
> }
>
> }
>
> //如果是标签选择器
>
> else if(regResult\[3\]) { var doms = document.getElementsByTagName(regResult\[3\].toLowerCase()); if(doms) { result = converToArray(doms);
>
> } } return result;
>
> }
>
> function converToArray(nodes){ var array = null; try{ array = Array.prototype.slice.call(nodes,0);//针对非IE浏览器
>
> }catch(ex){ array = new Array();
>
> for( var i = 0 ,len = nodes.length; i \< len ; i++ ) { array.push(nodes\[i\])
>
> } } return array;
>
> }

## 在 Javascript 中什么是伪数组？如何将伪数组转化为标准数组？

伪数组（类数组）：无法直接调用数组方法或期望length属性有什么特殊的行为，但仍可

以对真正数组遍历方法来遍历它们。典型的是函数的argument参数，还有像调用

getElementsByTagName,document.childNodes之类的,它们都返回NodeList对象都属于伪

数组。可以使用Array.prototype.slice.call(fakeArray)将数组转化为真正的Array对象。

假设接第八题题干，我们要给每个log方法添加一个"(app)"前缀，比如'helloworld!'

-\>'(app)hello world!'。方法如下：

[function](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [log(){](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

var args = Array.prototype.slice.call(arguments); //为了使用unshift数组方法，将argument转化为真正的数组

args.unshift(\'(app)\'); console.log.apply(console, args);

};

## （设计题）想实现一个对页面某个节点的拖曳？如何做？（使用原生 JS）

回答出概念即可，下面是几个要点

1.给需要拖拽的节点绑定mousedown, mousemove, mouseup事件

2.mousedown事件触发后，开始拖拽

3.mousemove时，需要通过event.clientX和clientY获取拖拽位置，并实时更新位置

4.mouseup时，拖拽结束

5.需要注意浏览器边界的情况

## 严格模式

链接：[[http://www.ruanyifeng.com/blog/2013/01/javascript\_strict\_mode.html]{.underline}](http://www.ruanyifeng.com/blog/2013/01/javascript_strict_mode.html)

全局变量显式声明

静态绑定

禁止使用**with** 语句

**eval** 中定义的变量都是局部变量

禁止 **this** 关键字指向全局对象

禁止在函数内部遍历调用栈

严格模式下无法删除变量。只有 configurable 设置为 true 的对象属性，才能被删除

正常模式下，对一个对象的只读属性进行赋值，不会报错，只会默默地失败。严格模式下，将报错。

严格模式下，对一个使用 getter 方法读取的属性进行赋值，会报错。

严格模式下，对禁止扩展的对象添加新属性，会报错。

严格模式下，删除一个不可删除的属性，会报错。

+------------+----+--------------------------+----+----------------------------------+------+------------+
| 正常模式下 | ， | > 如果对象有多个重名属性 | ， | 最后赋值的那个属性会覆盖前面的值 | > 。 | 严格模式下 |
+------------+----+--------------------------+----+----------------------------------+------+------------+

，这属于语法错误。

正常模式下，如果函数有多个重名的参数，可以用 arguments\[i\]读取。严格模式下，这属于

语法错误。

正常模式下，整数的第一位如果是 0，表示这是八进制数，比如 0100 等于十进制的 64。严

格模式禁止这种表示法，整数第一位为 0，将报错。

不允许对**arguments** 赋值

**arguments** 不再追踪参数的变化

禁止使用**arguments.callee**

严格模式只允许在全局作用域或函数作用域的顶层声明函数。也就是说，不允许在非函数的代码块内声明函数

严格模式新增了一些保留字：implements, interface, let, package, private, protected, public,

static, yield。

## 如何判断一个对象是否属于某个类(严格来说在ES6之前，js没有类的概念)？

instanceof constructor

## new操作符具体干了什么呢?

1.  创建一个空对象，并且 this 变量引用该对象，同时还继承了该函数的原型。

2.  属性和方法被加入到 this 引用的对象中。

3.  新创建的对象由 this 所引用，并且最后隐式的返回 this 。

## Javascript中，有一个函数，执行时对象查找时，永远不会去查找原型，这个函数是？

HasOwnProperty

## 对JSON的了解？

> 轻量级数据交互格式，可以形成复杂的嵌套格式，解析非常方便

## js延迟加载的方式有哪些？

> 方案一：\<script\>标签的async=\"async\"属性（详细参见：script标签的async属性）
>
> 方案二：\<script\>标签的defer=\"defer\"属性
>
> 方案三：动态创建\<script\>标签
>
> 方案四：AJAX eval（使用AJAX得到脚本内容，然后通过eval\_r(xmlhttp.responseText) 来运行脚本）
>
> 方案五：iframe方式

## [模块化开发怎么做？](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

> 理解模块化开发模式：浏览器端requirejs，seajs；服务器端nodejs；ES6模块化；fis、 webpack等前端整体模块化解决方案；grunt、gulp等前端工作流的使用

## Object对象的常用方法

Object.hasOwnProperty( ) 检查属性是否被继承

Object.isPrototypeOf( ) 一个对象是否是另一个对象的原型

Object.propertyIsEnumerable( ) 是否可以通过for/in循环看到属性

Object.toLocaleString( ) 返回对象的本地字符串表示

Object.toString( ) 定义一个对象的字符串表示

Object.valueOf( ) 指定对象的原始值

## JS 怎么实现一个类。怎么实例化这个类

> 严格来讲js中并没有类的概念，不过js中的函数可以作为构造函数来使用，通过new 来实例化，其实函数本身也是一个对象。

## **JavaScript** 中的作用域与变量声明提升？

> 理解JavaScript的预解析机制，js的运行主要分两个阶段：js的预解析和运行，预解析阶段所有的变量声明和函数定义都会提前，但是变量的赋值不会提前

## **javascript** 对象的几种创建方式？

1.  工厂模式

2.  构造函数模式

3.  原型模式

4.  混合构造函数和原型模式

5.  动态原型模式

6.  寄生构造函数模式

7.  稳妥构造函数模式

## **javascript** 继承的 **6** 种方法？

1.  原型链继承

2.  借用构造函数继承

3.  组合继承(原型+借用构造)

4.  原型式继承

5.  寄生式继承

6.  寄生组合式继承

## 简述一下Sass、Less，且说明区别？

他们是动态的样式语言，是CSS预处理器,CSS上的一种抽象层。他们是一种特殊的语法/语言而编译成CSS。

变量符不一样，less是@，而Sass是\$;

Sass支持条件语句，可以使用if{}else{},for{}循环等等。而Less不支持;

Sass是基于Ruby的，是在服务端处理的，而Less是需要引入less.js来处理Less代码输[出Css到浏览器

## 分别阐述split(),slice(),splice(),join()？

join()用于把数组中的所有元素拼接起来放入一个字符串。所带的参数为分割字符串的分隔符，默认是以逗号分开。归属于Array

split()即把字符串分离开，以数组方式存储。归属于Stringstring

slice() 方法可从已有的数组中返回选定的元素。该方法并不会修改数组，而是返回一个子数组。如果想删除数组中的一段元素，应该使用方法 Array.splice()

splice() 方法向/从数组中添加/删除项目，然后返回被删除的项目。返回的是含有被删除的元素的数组。

## 如何阻止事件冒泡和默认事件？

阻止浏览器的默认行为

window.event?window.event.returnValue=false:e.preventDefault();

停止事件冒泡

window.event?window.event.cancelBubble=true:e.stopPropagation();

原生JavaScript中，returnfalse;只阻止默认行为，不阻止冒泡，jQuery中的returnfalse; 既阻止默认行为，又阻止冒泡 63、添加 删除 替换 插入到某个接点的方法？

obj.appendChidl() obj.removeChild() obj.replaceChild() obj.innersetBefore()

## 请用正则表达式写一个简单的邮箱验证。

> /\^\[a-zA-Z0-9\_-\]+@\[a-zA-Z0-9\_-\]+(\\.\[a-zA-Z0-9\_-\]+)+\$/;

## 简述一下你对web性能优化的方案？

1.  尽量减少 HTTP 请求

2.  使用浏览器缓存

3.  使用压缩组件

4.  图片、JS的预载入

5.  将脚本放在底部

6.  将样式文件放在页面顶部

7.  使用外部的JS和CSS

8.  精简代码

## 在JS中有哪些会被隐式转换为false

Undefined、null、布尔值 false、NaN、零、空字符串

## 写一个通用的事件侦听器函数TODO

```js
// event(事件)工具集，来源：github.com/markyun
markyun.Event = {
    // 页面加载完成后
    readyEvent : function(fn) {
        if (fn==null) {
            fn=document;
        }
        var oldonload = window.onload;
        if (typeof window.onload != 'function') {
            window.onload = fn;
        } else {
            window.onload = function() {
                oldonload();
                fn();
            };
        }
    },
    // 视能力分别使用dom0||dom2||IE方式 来绑定事件
    // 参数： 操作的元素,事件名称 ,事件处理程序
    addEvent : function(element, type, handler) {
        if (element.addEventListener) {
            //事件类型、需要执行的函数、是否捕捉
            element.addEventListener(type, handler, false);
        } else if (element.attachEvent) {
            element.attachEvent('on' + type, function() {
                handler.call(element);
            });
        } else {
            element['on' + type] = handler;
        }
    },
    // 移除事件
    removeEvent : function(element, type, handler) {
        if (element.removeEnentListener) {
            element.removeEnentListener(type, handler, false);
        } else if (element.detachEvent) {
            element.detachEvent('on' + type, handler);
        } else {
            element['on' + type] = null;
        }
    }, 
    // 阻止事件 (主要是事件冒泡，因为IE不支持事件捕获)
    stopPropagation : function(ev) {
        if (ev.stopPropagation) {
            ev.stopPropagation();
        } else {
            ev.cancelBubble = true;
        }
    },
    // 取消事件的默认行为
    preventDefault : function(event) {
        if (event.preventDefault) {
            event.preventDefault();
        } else {
            event.returnValue = false;
        }
    },
    // 获取事件目标
    getTarget : function(event) {
        return event.target || event.srcElement;
    },
    // 获取event对象的引用，取到事件的所有信息，确保随时能使用event；
    getEvent : function(e) {
        var ev = e || window.event;
        if (!ev) {
            var c = this.getEvent.caller;
            while (c) {
                ev = c.arguments[0];
                if (ev && Event == ev.constructor) {
                    break;
                }
                c = c.caller;
            }
        }
        return ev;
    }
};
```



## 说几条JavaScript的基本规范 

不要在同一行声明多个变量

用 ===/!== 来比较 true/false或者数值使用对象字面量替代new Array这种形式

不要使用全局函数

Switch 语句必须带有 default 分支

If语句必须使用大括号

for-in 循环中的变量 应该使用 let 关键字明确限定作用域，从而避免作用域污染

## 作用域 

执行上下文中还包含作用域链。理解作用域之前，先介绍下作用域。作用域其实可理解为该上下文中声明的 变量和声明的作用范围。可分为 块级作用域 和 函数作用域特性:

声明提前: 一个声明在函数体内都是可见的, 函数优先于变量非匿名自执行函数，函数变量为 只读 状态，无法修改

## 说说你对作用域链的理解 

作用域链的作用是保证执行环境里有权访问的变量和函数是有序的，作用域链的变量只能向上访问，变量访问到 window对象即被终止，作用域链向下访问变量是不被允许的。

简单的说，作用域就是变量与函数的可访问范围，即作用域控制着变量与函数的可见性和生命周期

## JavaScript原型，原型链 ? 有什么特点？ 

每个对象都会在其内部初始化一个属性，就是 prototype (原型)，当我们访问一个对象的属性时, 如果这个对象内部不存在这个属性，那么他就会去 prototype 里找这个属性，这个prototype 又会有自己的 prototype ，于是就这样一直找下去，也就是我们平时所说的原型链的概念

关系： instance.constructor.prototype = instance.\_\*proto\*\_

特点：JavaScript 对象是通过引用来传递的，我们创建的每个新对象实体中并没有一份属于自己的原型副本。当我们修改原型时，与之相关的对象也会继承这一改变当我们需要一个属性的时， Javascript 引擎会先看当前对象中是否有这个属性， 如果没有的,就会查找他的 Prototype 对象是否有这个属性，如此递推下去，一直检索到 Object内建对象

### 什么是事件委托 

事件代理（ Event Delegation ），又称之为事件委托。是 JavaScript 中常用的绑定事件的常用技巧。顾名思义，"事件代理"即是把原本需要绑定的事件委托给父元素，让父元素担当事件监听的职务。事件代理的原理是DOM元素的事件冒泡。使用事件代理的好处是可以提高性能可以大量节省内存占用，减少事件注册，比如在 table上代理所有 td 的 click 事件就非常棒可以实现当新增子对象时无需再次对其绑定

## 事件模型 

W3C 中定义事件的发生经历三个阶段：捕获阶段（capturing ）、目标阶段 （targetin）、冒泡阶段（ bubbling）

冒泡型事件：当你使用事件冒泡时，子级元素先触发，父级元素后触发捕获型事件：当你使用事件捕获时，父级元素先触发，子级元素后触发

DOM 事件流：同时支持两种事件模型：捕获型事件和冒泡型事件

阻止冒泡：在 W3c 中，使用 stopPropagation() 方法；在IE下设置 cancelBubble =true 阻止捕获：阻止事件的默认行为，例如click - a后的跳转。在 W3c中，使用

preventDefault() 方法，在 IE 下设置 window.event.returnValue = false

## 说说对AMD和Commonjs的理解 

CommonJS 是服务器端模块的规范， Node.js 采用了这个规范。 CommonJS 规范加载模块是同步的，也就是说，只有加载完成，才能执行后面的操作。AMD规范则是非同步加载 模块，允许指定回调函数

AMD 推荐的风格通过返回一个对象做为模块对象， CommonJS的风格通过对 module.exports 或 exports的属性赋值来达到暴露模块对象的目的

## jQuery源码有哪些写的好的地方

jquery 源码封装在一个匿名函数的自执行环境中，有助于防止变量的全局污染，然后通过传入

window 对象参数，可以使 window对象作为局部变量使用，好处是当 jquery中访问window对象的时候，就不用将作用域链退回到顶层作用域了，从而可以更快的访问window对象。同样，传入 undefined参数，可以缩短查找 undefined 时的作用域链

jquery将一些原型属性和方法封装在了 jquery.prototype中，为了缩短名称，又赋值给了 jquery.fn，这是很形象的写法

有一些数组或对象的方法经常能使用到， jQuery 将其保存为局部变量以提高访问速度 jquery实现的链式调用可以节约代码，所返回的都是同一个对象，可以提高代码效率

## null，undefined 的区别 

undefined 表示不存在这个值。

undefined :是一个表示\"无\"的原始值或者说表示\"缺少值\"，就是此处应该有一个值，但是还没有定义。尝试读取时会返回 undefined

例如变量被声明了，但没有赋值时，就等于 undefined null 表示一个对象被定义了，值为"空值"

null : 是一个对象(空对象, 没有任何属性和方法)

例如作为函数的参数，表示该函数的参数不是对象；

在验证 null 时，一定要使用 === ，因为 == 无法分别 null 和 undefined

## 异步编程的实现方式 

1. 回调函数（callback） 
   - 优点：解决了同步的问题（只要有一个任务耗时很长，后面的任务都必须排队 等着，会拖延整个程序的执行。） 
   - 缺点：回调地狱，不能用 try catch 捕获错误，不能 return
2. Promise 
   - promise 构造函数是同步执行的，then 方法是异步执行的
   - 优点：解决了回调地狱的问题 
   - 缺点：无法取消 Promise ，错误需要通过回调函数来捕获
3. Generator 
   - 特点：可以控制函数的执行，可以配合 co 函数库使用
4. Async/await 
   - 优点：代码清晰，不用像 Promise 写一大堆 then 链，处理了回调地狱的问题 
   - 缺点：await 将异步代码改造成同步代码，如果多个异步操作没有依赖性而使 用 await 会导致性能上的降低。

## 对原生Javascript了解方向 

> 数据类型、运算、对象、Function、继承、闭包、作用域、原型链、事件、 RegExp、JSON 、
>
> Ajax、 DOM 、 BOM、内存泄漏、跨域、异步装载、模板引擎、前端MVC、路由、模块化、 Canvas、
>
> ECMAScript

## JS 原生拖拽节点 

> 给需要拖拽的节点绑定 mousedown , mousemove , mouseup 事件 mousedown 事件触发后，开始拖拽
>
> mousemove 时，需要通过 event.clientX 和 clientY获取拖拽位置，并实时更新位置 mouseup 时，拖拽结束
>
> 需要注意浏览器边界值，设置拖拽范围

## js单线程 

> 单线程 - 只有一个线程，只能做一件事原因 - 避免 DOM 渲染的冲突
>
> 浏览器需要渲染 DOM
>
> JS 可以修改 DOM结构
>
> JS 执行的时候，浏览器 DOM渲染会暂停
>
> 两段 JS 也不能同时执行（都修改 DOM 就冲突了）
>
> webworker 支持多线程，但是不能访问 DOM 解决方案 - 异步



## Set、Map、WeakSet 和 WeakMap 的区别

Set——对象允许你存储任何类型的唯一值，无论是原始值或者是对象引用 

WeakSet——成员都是对象；成员都是**弱引用**，可以被垃圾回收机制回收，可以 用来保存 DOM 节点，不容易造成内存泄漏； 

Map——本质上是键值对的集合，类似集合；可以遍历，方法很多，可以跟各种数据格式转换。 

WeakMap——只接受对象最为键名（null 除外），不接受其他类型的值作为键名；键名是**弱引用**，键值可以是任意的，键名所指向的对象可以被垃圾回收， 此时键名是无效的；不能遍历，方法有 get、set、has、delete。

## ajax、axios、fetch区别 

> ajax：
>
> 本身是针对MVC 的编程,不符合现在前端MVVM的浪潮
>
> 基于原生的 XHR开发， XHR 本身的架构不清晰，已经有了 fetch的替代方案

JQuery 整个项目太大，单纯使用 ajax 却要引入整个 JQuery 非常的不合理（采取个性化打包的方案又不能享受CDN服务） axios：

> 从浏览器中创建 XMLHttpRequest 从 node.js 发出 http请求
>
> 支持Promise API 拦截请求和响应转换请求和响应数据
>
> 取消请求
>
> 自动转换JSON数据

客户端支持防止 CSRF/XSRF fetch：

> 只对网络请求报错，对 400 ， 500 都当做成功的请求，需要封装去处理
>
> 这里对于 cookie 的处理比较特殊，不同浏览器对credentials的默认值不一样，也就使得默认情况下cookie变的不可控。
>
> 本身无自带 abort，无法超时控制，可以使用AbortController解决取消请求问题。
>
> 没有办法原生监测请求的进度，而XHR可以



## 1.JSONP的缺点

>  
>
> JSON只支持get，因为script标签只能使用get请求； JSONP需要后端配合返回指定格式的数据。

## 2.跨域（jsonp，ajax）

>  
>
> JSONP：ajax请求受同源策略影响，不允许进行跨域请求，而script标签src 属性中的链接却可以访问跨域的js脚本，利用这个特性，服务端不再返回JSON 格式的数据，而是返回一段调用某个函数的js代码，在src中进行了调用，这样实现了跨域。

## 3.如何实现跨域

>  
>
> JSONP：通过动态创建script，再请求一个带参网址实现跨域通信。 document.domain+iframe跨域：两个页面都通过js强制设置document.domain 为基础主域，就实现了同域。
>
> location.hash + iframe跨域：a欲与b跨域相互通信，通过中间页c来实现。三个页面，不同域之间利用iframe的location.hash传值，相同域之间直接js 访问来通信。
>
> window.name + iframe跨域：通过iframe的src属性由外域转向本地域，跨域数据即由iframe的window.name从外域传递到本地域。 postMessage跨域：可以跨域操作的window属性之一。
>
> CORS：服务端设置Access-Control-Allow-Origin即可，前端无须设置，若要带 cookie请求，前后端都需要设置。
>
> 代理跨域：起一个代理服务器，实现数据的转发

## 4.dom是什么，你的理解？

>  
>
> 文档对象模型（Document Object Model，简称DOM），是W3C组织推荐的处理可扩展标志语言的标准编程接口。在网页上，组织页面（或文档）的对象被组织在一个树形结构中，用来表示文档中对象的标准模型就称为DOM。

## 5.关于dom的api有什么

>  
>
> 节点创建型api，页面修改型API，节点查询型API，节点关系型api，元素属性型api，元素样式型api等

## 6.ajax返回的状态

>  

1. － （未初始化）还没有调用send()方法
2. － （载入）已调用send()方法，正在发送请求
3. － （载入完成）send()方法执行完成，已经接收到全部响应内容
4. － （交互）正在解析响应内容
5. － （完成）响应内容解析完成，可以在客户端调用了

## 7.实现一个Ajax

>  
>
> AJAX创建异步对象XMLHttpRequest 操作XMLHttpRequest 对象

1. 设置请求参数（请求方式，请求页面的相对路径，是否异步）
2. 设置回调函数，一个处理服务器响应的函数，使用 onreadystatechange ，类似函数指针
3. 获取异步对象的readyState 属性：该属性存有服务器响应的状态信息。

> 每当 readyState 改变时，onreadystatechange 函数就会被执行。（4）判断响应报文的状态，若为200说明服务器正常运行并返回响应数据。
>
> （5）读取响应数据，可以通过 responseText 属性来取回由服务器返回的数据。

## 8.如何实现ajax请求，假如我有多个请求，我需要让这些 ajax请求按照某种顺序一次执行，有什么办法呢？如何处理 ajax跨域

>  
>
> 通过实例化一个XMLHttpRequest对象得到一个实例，调用实例的open方法为这次ajax请求设定相应的http方法，相应的地址和是否异步，以异步为例，调用 send 方法，这个方法可以设定需要发送的报文主体，然后通过监听 readystatechange事件，通过这个实例 的readyState属性来判断这个ajax请求状态，其中分为0，1，2，3，4这四种状态（0未初始化，1载入/正在发送请求2载入完成/数据接收，3交互/解析数据，4接收数据完成），当状态为4的时候也就是接受数据完成的时候，这时候可以通过实例的status属性判断这个请求是否成功
>
> var xhr = new XMLHttpRequest();
>
> xhr.open('get', 'aabb.php', true); xhr.send(null);
>
> xhr.onreadystatechange = function() { if(xhr.readyState==4) { if(xhr.status==200) {
>
> console.log(xhr.responseText);
>
> }
>
> } }
>
> 使ajax请求按照队列顺序执行，通过调用递归函数：
>
> //按顺序执行多个ajax命令，因为数量不定，所以采用递归
>
> function send(action, arg2) {
>
> //将多个命令按顺序封装成数组对象，递归执行
>
> //利用了deferred对象控制回调函数的特点
>
> $.when(send_action(action[0], arg2))
>
> .done(function () {
>
> //前一个ajax回调函数完毕之后判断队列长度
>
> if (action.length > 1) {
>
> //队列长度大于1，则弹出第一个，继续递归执行该队列
>
> action.shift(); send(action, arg2);
>
> }
>
> }).fail(function (){
>
> //队列中元素请求失败后的逻辑
>
> //
>
> //重试发送
>
> //send(action, arg2);
>
> //
>
> //忽略错误进行下个
>
> //if (action.length > 1) {
>
> //队列长度大于1，则弹出第一个，继续递归执行该队列

// action.shift();

// send(action, arg2);

> //}
>
> });
>
> }
>
> //处理每个命令的ajax请求以及回调函数 function send_action(command, arg2) { var dtd = $.Deferred();//定义deferred对象
>
> $.post(
>
> "url",
>
> {
>
> command: command, arg2: arg2
>
> }
>
> ).done(function (json) { json = $.parseJSON(json);
>
> //每次请求回调函数的处理逻辑
>
> //
>
> //
>
> //
>
> //逻辑结束
>
> dtd.resolve(); }).fail(function (){
>
> //ajax请求失败的逻辑
>
> dtd.reject(); });
>
> return dtd.promise();//返回Deferred对象的promise，防止在外部修改状态
>
> }

## 9.如何实现一个ajax请求？如果我想发出两个有顺序的 ajax需要怎么做？

>  
>
> AJAX创建异步对象XMLHttpRequest 操作XMLHttpRequest 对象

1. 设置请求参数（请求方式，请求页面的相对路径，是否异步）
2. 设置回调函数，一个处理服务器响应的函数，使用 onreadystatechange ，

> 类似函数指针

1. 获取异步对象的readyState 属性：该属性存有服务器响应的状态信息。

> 每当 readyState 改变时，onreadystatechange 函数就会被执行。

1. 判断响应报文的状态，若为200说明服务器正常运行并返回响应数据。
2. 读取响应数据，可以通过 responseText 属性来取回由服务器返回的数据。

> 发出两个有顺序的ajax，可以用回调函数，也可以使用Promise.then或者async 等。

## 10.Fetch和Ajax比有什么优缺点？

>  
>
> promise方便异步，在不想用jQuery的情况下，相比原生的ajax，也比较好写。

## 11. 移动应用和web应用的关系

>  
>
> 原生app是基于手机操作系统，所以兼容性和接口方面特别丰富。而webapp是基于浏览器所以接口并不是很多，但是开发速率快，版本控制简单。成本低。

## 12.知道PWA吗

>  
>
> PWA全称ProgressiveWebApp，即渐进式WEB应用。一个 PWA 应用首先是一个网页, 可以通过 Web 技术编写出一个网页应用. 随后添加上 App Manifest 和
>
> Service Worker 来实现 PWA 的安装和离线等功能

## 13.做过移动端吗

>  根据自身实际情况回答

## 14.知道touch事件吗

>  
>
> 触摸事件，有touchstart touchmove touchend touchcancel 四种之分，常用的有：
>
> (1)touchstart：当有新手指触控到绑定的元素，会触发一次事件。

(2)touchmove：当有手指放绑定的元素上会一直触发，从触发条件准确的说只有手指移动时才触发。但是经过测试，这一项检测十分灵敏，人为手指保持不动，系统也会侦测到细小的移动。所以会一直触发。

> (3)touchend：当有手指从绑定元素上抬起，会触发一次。

(4)touchcancel：可由系统进行的触发（不常用事件），比如手指触摸屏幕的时候，突然alert了一下，或者系统中其他打断了touch的行为，则可以触发该事件。

> 事件列表：在移动端中上面的三个触摸事件每个事件都有以下列表:
>
> (1)changedTouches：保存了所有引发事件的手指信息
>
> (2)targetTouches：保存了当前对象上所有触摸点的列表;
>
> (3)touches：保存了当前所有触碰屏幕的手指信息

# 第四章 浏览器



## 浏览器内核的理解 

主要分两个部分：渲染引擎、js引擎

渲染引擎：负责取得网页的内容（html css img \...），以及计算网页的显示方式，然后会输出至显示器或者打印机。浏览器的内核不同对于网页的语法解释也不同，所以渲染的效果也不一样 js引擎：解析和执行javascript 来实现网页的动态效果

开始渲染引擎和js引擎并没有区分的很明确，后来js引擎越来越独立，内核就倾向于只值渲染引擎

IE : trident 内核

Firefox ： gecko 内核

Safari : webkit 内核

Opera :以前是 presto 内核， Opera 现已改用Google - Chrome 的 Blink 内核

Chrome:Blink (基于 webkit ，Google与Opera Software共同开发)

## HTTP 的请求方式场景 

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

## 谈谈Cookie的优缺点 

**优点：**极高的扩展性和可用性

1)  数据持久性。

2)  不需要任何服务器资源。 Cookie 存储在客户端并在发送后由服务器读取。

3)  可配置到期规则。 控制 cookie 的生命期，使之不会永远有效。偷盗者很可能拿到一个过期的 cookie。

4)  简单性。 基于文本的轻量结构。

5)  通过良好的编程，控制保存在 cookie 中的 session 对象的大小。

6)  通过加密和安全传输技术（ SSL ），减少 cookie 被破解的可能性。

7)  只在 cookie 中存放不敏感数据，即使被盗也不会有重大损失。

缺点：

1\) Cookie 数量和长度的限制 。

数量：每个域的 cookie 总数有限。 

a) IE6 或更低版本 多 20 个 cookie

b)  IE7 和之后的版本 后可以有 50 个 cookie

c)  Firefox 多 50 个 cookie

d)  chrome 和 Safari 没有做硬性限制

长度：每个 cookie 长度不超过 4KB （ 4096B ），否则会被截掉。

2)  潜在的安全风险 。 Cookie 可能被拦截、篡改。如果 cookie 被拦截，就有可能取得所有的 session 信息。

3)  用户配置为禁用 。有些用户禁用了浏览器或客户端设备接受 cookie 的能力，因此限制了这一功能。

4)  有些状态不可能保存在客户端 。例如，为了防止重复提交表单，我们需要在服务器端保存一个计数器。如果我们把这个计数器保存在客户端，那么它起不到任何作用。

## 浏览器缓存 

浏览器缓存分为**强缓存和协商缓存**。当客户端请求某个资源时，获取缓存的流程如下

先根据这个资源的一些 http header 判断它是否命中强缓存，如果命中，则直接从本地获取缓存资源，不会发请求到服务器；

当强缓存没有命中时，客户端会发送请求到服务器，服务器通过另一些 request header验证这个资源是否命中协商缓存，称为http 再验证，如果命中，服务器将请求返回，但不返回资源，而是告诉客户端直接从缓存中获取，客户端收到返回后就会从缓存中获取资源； 强缓存和协商缓存共同之处在于，如果命中缓存，服务器都不会返回资源； 区别是，强缓存不对发送请求到服务器，但协商缓存会。

当协商缓存也没命中时，服务器就会将资源发送回客户端。

当 ctrl+f5 强制刷新网页时，直接从服务器加载，跳过强缓存和协商缓存；当 f5 刷新网页时，跳过强缓存，但是会检查协商缓存；

## 浏览器渲染的步骤 

1.  HTML 解析出 DOM Tree

2.  CSS 解析出 Style Rules

3.  两者关联生成 Render Tree

4.  Layout（布局）根据 Render Tree 计算每个节点的信息

5.  Painting 根据计算好的信息进行渲染整个页面

浏览器解析文档的过程中，如果遇到 script 标签，会立即解析脚本，停止解析文档（因为 JS 可能会改变DOM 和 CSS,如果继续解析会造成浪费）。

如果是外部 script, 会等待脚本下载完成之后在继续解析文档。现在 script 标签增加了 defer 和 async 属性，脚本解析会将脚本中改变 DOM 和 css 的地方\> 解析出来，追加到 DOM Tree 和 Style Rules 上

## 浏览器渲染机制

浏览器采用流式布局模型（Flow Based Layout） 

浏览器会把 HTML 解析成 DOM，把 CSS 解析成 CSSOM，DOM 和 CSSOM 合并就 产生了渲染树（Render Tree）。

有了 RenderTree，我们就知道了所有节点的样式，然后计算他们在页面上的大 小和位置，最后把节点绘制到页面上。 

由于浏览器使用流式布局，对 Render Tree 的计算通常只需要遍历一次就可以完 成，但 table 及其内部元素除外，他们可能需要多次计算，通常要花 3 倍于同 等元素的时间，这也是为什么要避免使用 table 布局的原因之一。

### 优化

现代浏览器大多都是通过队列机制来批量更新布局，浏览器会把修改操作放在 队列中，至少一个浏览器刷新（即 16.6ms）才会清空队列，但当你获取布局信 息的时候，队列中可能有会影响这些属性或方法返回值的操作，即使没有，浏 览器也会强制清空队列，触发回流与重绘来确保返回正确的值。

 主要包括以下属性或方法： 

1. offsetTop、offsetLeft、offsetWidth、offsetHeight 
2. scrollTop、scrollLeft、scrollWidth、scrollHeight 
3. clientTop、clientLeft、clientWidth、clientHeight 
4. width、height
5. getComputedStyle() 
6. getBoundingClientRect() 

所以，我们应该避免频繁的使用上述的属性，他们都会强制渲染刷新队列

## 重排和重绘 

部分渲染树（或者整个渲染树）需要重新分析并且节点尺寸需要重新计算。这被称为重排。注意这里至少会有一次重排-初始化页面布局。

由于节点的几何属性发生改变或者由于样式发生改变，例如改变元素背景色时，屏幕上的部分内容需要更新。这样的更新被称为重绘。

### 什么情况会触发重排和重绘？ 

1.  添加、删除、更新 DOM 节点

2.  通过 display: none 隐藏一个 DOM 节点-触发重排和重绘

3.  通过 visibility: hidden 隐藏一个 DOM 节点-只触发重绘，因为没有几何变化

4.  移动或者给页面中的 DOM 节点添加动画

5.  添加一个样式表，调整样式属性

6.  用户行为，例如调整窗口大小，改变字号，或者滚动

## 重绘和回流以及优化方式

- 重绘：
  - 由于节点的几何属性发生改变或者由于样式发生改变而不会影响布局的，称为 重绘，例如 outline, visibility, color、background-color 等，重绘的代价是高昂的， 因为浏览器必须验证 DOM 树上其他节点元素的可见性。
- 回流：
  - 回流是布局或者几何属性需要改变就称为回流。回流是影响浏览器性能的关键 因素，因为其变化涉及到部分页面（或是整个页面）的布局更新。一个元素的 回流可能会导致了其所有子元素以及 DOM 中紧随其后的节点、祖先节点元素 的随后的回流
- 回流必定会发生重绘，重绘不一定会引发回流。



### 重绘和回流的优化

CSS 

1. 使用 transform 替代 top
2. 使用 visibility 替换 display: none ，因为前者只会引起重绘，后者会引发回 流（改变了布局 
3. 避免使用 table 布局，可能很小的一个小改动会造成整个 table 的重新布局。 
4. 尽可能在 DOM 树的最末端改变 class，回流是不可避免的，但可以减少其影 响。尽可能在 DOM 树的最末端改变 class，可以限制了回流的范围，使其影响 尽可能少的节点。
5. 避免设置多层内联样式，CSS 选择符从右往左匹配查找，避免节点层级过多。

**JavaScript** 

1. 避免频繁操作样式，最好一次性重写 style 属性，或者将样式列表定义为 class并一次性更改 class 属性。 
2. 避免频繁操作 DOM，创建一个 documentFragment，在它上面应用所有 DOM 操作，最后再把它添加到文档中。 
3. 避免频繁读取会引发回流/重绘的属性，如果确实需要多次使用，就用一个变量缓存起来。
4. 对具有复杂动画的元素使用绝对定位，使它脱离文档流，否则会引起父元素及后续元素频繁回流。

## 什么是reflow 

浏览器为了重新渲染部分或整个页面，重新计算页面元素位置和几何结构的进程叫做 reflow . 通俗点说就是当开发人员定义好了样式后(也包括浏览器的默认样式),浏览器根据这些来计算并根据结果将元素放到它应该出现的位置上，这个过程叫做 reflow . 由于reflow是一种浏览器中的用户拦截操作，所以我们了解如何减少 reflow 次数，及DOM的层级，css 效率对 refolw 次数的影响是十分有必要的。 reflow

(回流)是导致DOM脚本执行效率低的关键因素之一，页面上任何一个节点触发了 reflow，会导致它的子节点及祖先节点重新渲染。 简单解释一下 Reflow：当元素改变的时候，将会影响文档内容或结构，或元素位置，此过程称为 Reflow。

当p节点上发生reflow时，hello和body也会重新渲染，甚至h5和ol都会收到影响。

## 什么时候会导致reflow发生呢？ TODO

改变窗口大小改变文字大小添加/删除样式表

内容的改变，(用户在输入框中写入内容也会) 激活伪类，如:hover

操作class属性脚本操作DOM

计算offsetWidth和offsetHeight 设置style属性

+----------------------+--------------+----------------+------------+
| > **常见的重排元素** |              |                |            |
+======================+==============+================+============+
| > width              | height       | padding        | margin     |
+----------------------+--------------+----------------+------------+
| > display            | border-width | border         | top        |
+----------------------+--------------+----------------+------------+
| > position           | font-size    | float          | text-align |
+----------------------+--------------+----------------+------------+
| > overflow-y         | font-weight  | overflow       | left       |
+----------------------+--------------+----------------+------------+
| > font-family        | line-height  | vertical-align | right      |
+----------------------+--------------+----------------+------------+
| > clear              | white-space  | bottom         | min-height |
+----------------------+--------------+----------------+------------+

## 减少reflow对性能的影响 

不要一条一条地修改 DOM 的样式，预先定义好 class，然后修改 DOM 的 className

把 DOM 离线后修改，比如：先把 DOM 给 display:none (有一次 Reflow)，然后你修改100次，然后再把它显示出来

不要把 DOM 结点的属性值放在一个循环里当成循环里的变量尽可能不要修改影响范围比较大的 DOM

为动画的元素使用绝对定位 absolute / fixed 不要使用 table 布局，可能很小的一个小改动会造成整个 table 的重新布局尽可能限制reflow的影响范围，尽可能在低层级的DOM节点上，上述例子中，如果你要改变p的样式，class就不要加在div上，通过父元素去影响子元素不好。

避免设置大量的 style 属性，因为通过设置 style 属性改变结点样式的话，每一次设置都会触发一次 reflow，所以 好是使用 class 属性

实现元素的动画，它的position属性， 好是设为absoulte或fixed，这样不会影响其他元素的布局

动画实现的速度的选择。比如实现一个动画，以1个像素为单位移动这样 平滑，但是reflow就会过于频繁，大量消耗CPU资源，如果以3个像素为单位移动则会好很多。

不要使用 table 布局，因为table中某个元素旦触发了 reflow，那么整个 table 的元素都会触发reflow 。那么在不得已使用 table 的场合，可以设置 table-layout:auto; 或者是 table-layout:fixed 这样可以让table一行一行的渲染，这种做法也是为了限制reflow的影响范围

如果CSS里面有计算表达式，每次都会重新计算一遍，出发一次reflow。

## 浏览器缓存机制

https://www.jianshu.com/p/54cc04190252

浏览器缓存分为强缓存和协商缓存。当客户端请求某个资源时，获取缓存的流程如下

先根据这个资源的一些 http header 判断它是否命中强缓存，如果命中，则直接从本地获取缓存资源，不会发请求到服务器；

当强缓存没有命中时，客户端会发送请求到服务器，服务器通过另一些 request header验证这个资源是否命中协商缓存，称为http 再验证，如果命中，服务器将请求返回，但不返回资源，而是告诉客户端直接从缓存中获取，客户端收到返回后就会从缓存中获取资源； 强缓存和协商缓存共同之处在于，如果命中缓存，服务器都不会返回资源； 区别是，强缓存不对发送请求到服务器，但协商缓存会。

当协商缓存也没命中时，服务器就会将资源发送回客户端。

当 ctrl+f5 强制刷新网页时，直接从服务器加载，跳过强缓存和协商缓存；当 f5 刷新网页时，跳过强缓存，但是会检查协商缓存；

## 浏览器存储机制

| 特性           | 数据生命周期                       | 数据存储大小 | 与服务端通信                                |
| -------------- | ---------------------------------- | ------------ | ------------------------------------------- |
| cookie         | 一般由服务器生成，可以设置过期时间 | 4K           | 每次都会携带在 header，中，对于请求性能影响 |
| localStroage   | 除非被清理，否则一直存在           | 5M           | 不参与                                      |
| sessionStorage | 页面关闭就清理                     | 5M           | 不参与                                      |
| indexedDB      | 除非被清理，否则一直存在           | 无限         | 不参与                                      |

> 补充：cookie 原本并不是用来储存的，而是用来与服务端通信的，需要存取请自行封装 api。
>
> 而 localStorage 则自带 getItem 和 setItem 方法，使用很方便。
>
> localStorage 注意点：

1.  localStorage 只能存字符串，存取 JSON 数据需配合 JSON.stringify() 和 JSON.parse()
2.  遇上禁用 setItem 的浏览器，需要使用 try\...catch 捕获异常



## AJAX原理

Ajax 的原理简单来说是在用户和服务器之间加了一个中间层( AJAX 引擎)，通过XmlHttpRequest 对象来向服务器发异步请求，从服务器获得数据，然后用 javascript来操作 DOM 而更新页面。使用户操作与服务器响应异步化。这其中 关键的一步就是从服务器获得请求数据

Ajax的过程只涉及JavaScript 、 XMLHttpRequest 和 DOM 。 XMLHttpRequest是ajax的核心机制

## AJAX解决浏览器缓存

在ajax发送请求前加上 anyAjaxObj.setRequestHeader(\"If-Modified-Since\",\"0\")。

在ajax发送请求前加上 anyAjaxObj.setRequestHeader(\"Cache-Control\",\"no-cache\")。

在URL后面加上一个随机数： \"fresh=\" + Math.random()。

在URL后面加上时间搓：\"nowtime=\" + new Date().getTime()。

如果是使用jQuery，直接这样就可以了 $.ajaxSetup({cache:false})。这样页面的所有ajax都会执行这条语句就是不需要保存缓存记录。



## 如何解决跨域问题

- 了解浏览器的同源策略

解决跨域问题：

- jsonp

  ```js
  var script = document.create("script")
  script.type = "text/javascript";
  script.src = "http://www.......8080/login?user=admin&callback=onBack";
  document.head.appendChild(script);
  function onBack(res){
      alert(JSON.stringify(res));
  }
  ```

  

- `document.domain+iframe`

  - nginx 代理跨域
  - node.js中间件代理跨域
  - 后端在头部信息里设置安全域名



## 对AMD和Commonjs的理解 

CommonJS 是服务器端模块的规范， Node.js 采用了这个规范。 CommonJS 规范加载模

块是同步的，也就是说，只有加载完成，才能执行后面的操作。AMD规范则是非同步加载 模块，允许指定回调函数

AMD 推荐的风格通过返回一个对象做为模块对象， CommonJS的风格通过对 module.exports 或 exports的属性赋值来达到暴露模块对象的目的

## 创建ajax的过程

step1. 创建XMLHttpRequest对象，也就是创建一个异步调用对象； 
step2. 创建一个新的HTTP请求，并指定改HTTP请求的方法、URL以及验证信息； 
step3. 设置响应HTTP状态变化的函数； 
step4. 发送HTTP请求； 
step5. 获取异步调用返回的数据； 
step6. 使用javascript和DOM实现局部刷新；

```javascript
<script type="text/javascript">
    window.onload = function(){
        //第一步：创建xhr对象
        //xhr是一个对象；里面可以放很多东西，数据；
        var xhr = null;
        if(window.XMLHttpRequest){//标准浏览器
            xhr = new XMLHttpRequest();//创建一个对象
        }else{//早期的IE浏览器
            xhr = new ActiveXObject('Microsoft.XMLHTTP');//参数是规定的；
        }
        console.log("状态q"+xhr.readyState);//0
        //第二步：准备发送请求-配置发送请求的一些行为
        //open即打开链接，第一个参数是以什么方式；第二个是往哪儿发送请求，第三个可以不写，默认true,表示异步，false表示同步；；
        xhr.open('get','03form.php',true);
        console.log("状态w"+xhr.readyState);//1

        //第三步：执行发送的动作
        //send也可以写在前面，推荐写在后面；写null是兼容问题；
        xhr.send(null);
        console.log("状态e"+xhr.readyState);//1

        //第四步：指定一些回调函数，也属于事件函数；不触发不执行，触发条件是xhr.readyState;z这个值有0-4，共5个状态，是由浏览器控制的；
        xhr.onreadystatechange = function(){
            if(xhr.readyState == 4){//4指服务器返回的数据可以使用；
                if(xhr.status == 200){ //判断已经成功的获取了数据；200表示hTTP请求成功；404表示找不到页面；503表示服务器端有语法错误；
                    var data = xhr.responseText;//json，文本，主角；
                    // var data1 = xhr.responseXML;
                }
            }
            // console.log("状态t"+xhr.readyState);//2表示已经发送完成；

            // console.log(1234);
        }

        // console.log(456);
        console.log("状态r"+xhr.readyState);//1


    }
    </script>
```



## 常见兼容性问题？

1. 双边距 BUG float 引起的 使用 display 

2. 3 像素问题 使用 float 引起的 使用 `dislpay:inline -3px `

3. 超链接 hover 点击后失效 使用正确的书写顺序 link visited hover active 

4. Ie z-index 问题 给父级添加 `position:relative `

5. PNG透明 使用 js 代码 改 

6. Min-height 最小高度 `！Important` 解决

7. select 在 ie6 下遮盖 使用 `iframe` 嵌套
8. 为 什 么 没 有 办 法 定 义 1px 左 右 的 宽 度 容 器 （ IE6 默 认 的 行 高 造 成 的 ， 使 用 `over:hidden,zoom:0.08 line-height:1px`） 
9. IE5-8 不支持 opacity，解决办法： `.opacity { opacity: 0.4 filter: alpha(opacity=60); /* for IE5-7 */ -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)"; /* for IE 8*/ }`

10. IE6 不支持 PNG 透明背景，解决办法: IE6 下使用 gif 图片







## 性能优化 

### 1，SEO优化 

> 合理的 title 、 description 、 keywords ：搜索对着三项的权重逐个减小， title值强调重点即可，重要关键词出现不要超过2次，而且要靠前，不同页面 title 要有所不同； description把页
>
> 面内容高度概括，长度合适，不可过分堆砌关键词，不同页面description有所不同； keywords 列举出重要关键词即可
>
> 语义化的HTML 代码，符合W3C规范：语义化代码让搜索引擎容易理解网页
>
> 重要内容HTML代码放在 前：搜索引擎抓取HTML 顺序是从上到下，有的搜索引擎对抓取长度有限制，保证重要内容一定会被抓取重要内容不要用 js 输出：爬虫不会执行js获取内容少用 iframe：搜索引擎不会抓取 iframe中的内容非装饰性图片必须加alt
>
> 提高网站速度：网站速度是搜索引擎排序的一个重要指标

### 2，server优化 

> 减少HTTP请求，合并文件、雪碧图减少DNS查询，使用缓存
>
> 减少Dom元素的数量使用CDN
>
> 配置ETag ,http缓存的手段对组件使用Gzip压缩减少cookie的大小

### 3，css优化 

> 将样式表放在页面顶部使用less scss表达式
>
> 使用link不适用\@import引入样式压缩css
>
> 禁止使用 gif图片实现 loading 效果（降低 CPU 消耗，提升渲染性能）
>
> 使用 CSS3代码代替 JS 动画（尽可能避免重绘重排以及回流）对于一些小图标，可以使用base64位编码，以减少网络请求。
>
> 页面头部的 \<style\> \<script\> 会阻塞页面；（因为 Renderer进程中 JS 线程和渲染线程是互斥的）
>
> 当需要设置的样式很多时设置 className而不是直接操作 style

### 4，js方面 

> 将脚本放到页面底部
>
> 将js外部引入压缩js
>
> 使用Eslint语法检测
>
> 减少Dom的操作
>
> 熟练使用设计模式
>
> 禁止使用 iframe（阻塞父文档 onload 事件）
>
> 页面中空的 href 和 src会阻塞页面其他资源的加载网页 gzip ， CDN托管， data 缓存 ，图片服务器

### 5，webpack优化点 

> 代码压缩插件UglifyJsPlugin 服务器启用gzip压缩
>
> 按需加载资源文件require.ensure
>
> 优化 devtool中的 source-map 剥离 css 文件，单独打包
>
> 去除不必要插件，通常就是开发环境与生产环境用同一套配置文件导致开发环境不做无意义的工作如提取 css计算文件hash等
>
> 配置 devtool
>
> 优化构建时的搜索路径 指明需要构建目录及不需要构建目录

### 6，加载优化： 

> 合并CSS、JavaScript
>
> 合并小图片、使用精灵图
>
> 缓存一切可缓存的资源
>
> 使用外链式引用CSS、JavaScript
>
> 压缩HTML、CSS、JavaScript 启用GZip
>
> 使用首屏加载、按需加载、滚屏加载通过Media Query加载增加Loading进度条
>
> 减少Cookie 避免重定向异步加载第三方资源

### 7，页面渲染优化 

> HTML 文档结构层次尽量少， 好不深于 6 层脚本尽量放后边，避免组织页面加载少量首屏样式可以放在便签内
>
> 样式结构层次尽量简单
>
> 脚本减少 DOM 操作，减少回流，尽量缓存访问 DOM 的样式信息尽量减少 JS 修改样式，可以通过修改 class 名的方式解决减少 DOM 查找，缓存 DOM 查找结果
>
> 动画在屏幕外或页面滚动时，尽量停止

### 8，图片优化 

> 使用智图
>
> 使用（CSS3、SVG、IconFont）代替图片使用Srcset webP优于JPG
>
> PNG8优于GIF
>
> 图片不宽于640

### 9，脚本优化 

> 减少重绘和回流
>
> 缓存Dom选择与计算
>
> 尽量使用事件处理，避免批量绑定事件尽量使用ID选择器
>
> 使用touchstart、touchend代替click

### 10，为什么利用多个域名来存储网站资源会更有效？ 

> CDN 缓存更方便
>
> 突破浏览器并发限制节约 cookie 带宽
>
> 节约主域名的连接数，优化页面响应速度防止不必要的安全问题

# 第五章 前端进阶

## Vue框架 

### vue的生命周期★★

Vue实例有一个完整的生命周期，也就是从开始创建、初始化数据、编译模板、挂载Dom、渲染→更新→渲染、销毁等一系列过程，我们称这是Vue的生命周期。

通俗说就是Vue实例从创建到销毁的过程，就是生命周期。

每一个组件或者实例都会经历一个完整的生命周期，总共分为三个阶段：初始化、运行中、销毁。

实例、组件通过new Vue() 创建出来之后会初始化事件和生命周期，然后就会执行beforeCreate钩子函数，这个时候，数据还没有挂载呢，只是一个空壳，无法访问到数据和真实的dom，一般不做操作

挂载数据，绑定事件等等，然后执行created函数，这个时候已经可以使用到数据，也可以更改数据,在这里更改数据不会触发updated函数，在这里可以在渲染前倒数第二次更改数据的机会，不会触发其他的钩子函数，一般可以在这里做初始数据的获取

接下来开始找实例或者组件对应的模板，编译模板为虚拟dom放入到render函数中准备渲染，然后执行beforeMount钩子函数，在这个函数中虚拟dom已经创建完成，马上就要渲染,在这里也可以更改数据，不会触发updated，在这里可以在渲染前最后一次更改数据的机会，不会触发其他的钩子函数，一般可以在这里做初始数据的获取

接下来开始render，渲染出真实dom，然后执行mounted钩子函数，此时，组件已经出现在页面中，数据、真实dom都已经处理好了,事件都已经挂载好了，可以在这里操作真实dom等事情...

当组件或实例的数据更改之后，会立即执行beforeUpdate，然后vue的虚拟dom 机制会重新构建虚拟dom与上一次的虚拟dom树利用diff算法进行对比之后重新渲染，一般不做什么事儿

当更新完成后，执行updated，数据已经更改完成，dom也重新render完成，可以操作更新后的虚拟dom

当经过某种途径调用$destroy方法后，立即执行beforeDestroy，一般在这里做一些善后工作，例如清除计时器、清除非指令绑定的事件等等

组件的数据绑定、监听...去掉后只剩下dom空壳，这个时候，执行destroyed，在这里做善后工作也可以

###  **active-class是哪个组件的属性？嵌套路由怎么定义？**

vue-router模块的router-link组件。

### **怎么定义vue-router的动态路由？怎么获取传过来的动态参数？**

在router目录下的index.js文件中，对path属性加上/:id。 使用router对象的params.id

### vue-router有哪几种导航钩子？ 

三种，一种是全局导航钩子：router.beforeEach(to,from,next)，作用：跳转前进行判断拦截。第二种：组件内的钩子；第三种：单独路由独享组件

### scss是什么？在vue.cli中的安装使用步骤是？有哪几大特性？ 

css的预编译。使用步骤：

第一步：用npm 下三个loader（sass-loader、css-loader、node-sass）

第二步：在build目录找到webpack.base.config.js，在那个extends属性中加一个拓展.scss 

第三步：还是在同一个文件，配置一个module属性

第四步：然后在组件的style标签加上lang属性 ，例如：lang="scss" 有哪几大特性:

1.  可以用变量，例如（\$变量名称=值）；

2.  可以用混合器，例如（）

3.  可以嵌套

### mint-ui是什么？怎么使用？说出至少三个组件使用方法？ 

基于vue的前端组件库。npm安装，然后import样式和js，vue.use（mintUi）全局引入。在单个组件局部引入：import {Toast} from 'mint-ui'。组件一：Toast('登录成功')；组件二：mint-header；组件三： mint-swiper

### v-model是什么？怎么使用？ vue中标签怎么绑定事件？ 

可以实现双向绑定，指令（v-class、v-for、v-if、v-show、v-on）。vue的model层的data属性。绑定事件：\<input \@click=doLog() /\>

### axios是什么？怎么使用？描述使用它实现登录功能的流程？ 

> 请求后台资源的模块。npm install axios -S装好，然后发送的是跨域，需在配置文件中config/index.js 进行设置。后台如果是Tp5则定义一个资源路由。js中使用import进来，然后.get或.post。返回在.then 函数中如果成功，失败则是在.catch函数中

### axios+tp5进阶中，调用axios.post('api/user')是进行的什么操作？ axios.put('api/user/8′)呢？

> 跨域，添加用户操作，更新操作。

### 什么是RESTful API？怎么使用?

> 是一个api的标准，无状态请求。请求的路由地址是固定的，如果是tp5则先路由配置中把资源路由配置好。标准有：.post .put .delete

### vuex是什么？怎么使用？哪种功能场景使用它？ 

vue框架中状态管理。在main.js引入store，注入。新建了一个目录store，..... export 。场景有：单页应用中，组件之间的状态。音乐播放、登录状态、加入购物车

### mvvm框架是什么？它和其它框架（jquery）的区别是什么？哪些场景适合？ 

一个model+view+viewModel框架，数据模型model，viewModel连接两个区别：vue数据驱动，通过数据来显示视图层而不是节点操作。

场景：数据操作比较多的场景，更加便捷

### 自定义指令（v-check、v-focus）的方法有哪些？它有哪些钩子函数？还有哪些钩子函数参数？

> 全局定义指令：在vue对象的directive方法里面有两个参数，一个是指令名称，另外一个是函数。组件内定义指令：directives
>
> 钩子函数：bind（绑定事件触发）、inserted(节点插入的时候触发)、update（组件内相关更新）钩子函数参数：el、binding

### 说出至少4种vue当中的指令和它的用法

> v-if：判断是否隐藏；v-for：数据循环出来；v-bind:class：绑定一个属性；v-model：实现双向绑定

### vue-router是什么？它有哪些组件？ 

vue用来写路由一个插件。router-link、router-view

### 导航钩子有哪些？它们有哪些参数？ 

导航钩子有：a/全局钩子和组件内独享的钩子。b/beforeRouteEnter、afterEnter、 beforeRouterUpdate、beforeRouteLeave

> 参数：有to（去的那个路由）、from（离开的路由）、next（一定要用这个函数才能去到下一个路由，如果不用就拦截） 常用就这几种

### Vue的双向数据绑定原理是什么？ 

vue.js 是采用数据劫持结合发布者-订阅者模式的方式，通过Object.defineProperty()来劫持各个属性的setter，getter，在数据变动时发布消息给订阅者，触发相应的监听回调。

具体步骤：

第一步：需要observe的数据对象进行递归遍历，包括子属性对象的属性，都加上 setter和getter 这样的话，给这个对象的某个值赋值，就会触发setter，那么就能监听到了数据变化

第二步：compile解析模板指令，将模板中的变量替换成数据，然后初始化渲染页面视图，并将每个指令对应的节点绑定更新函数，添加监听数据的订阅者，一旦数据有变动，收到通知，更新视图

第三步：Watcher订阅者是Observer和Compile之间通信的桥梁，主要做的事情是:

1.  在自身实例化时往属性订阅器(dep)里面添加自己

2.  自身必须有一个update()方法

3.  待属性变动dep.notice()通知时，能调用自身的update()方法，并触发Compile中绑定的回调，则功成身退。

第四步：MVVM作为数据绑定的入口，整合Observer、Compile和Watcher三者，通过Observer来监听自己的model数据变化，通过Compile来解析编译模板指令， 终利用Watcher搭起Observer和

Compile之间的通信桥梁，达到数据变化 -\> 视图更新；视图交互变化(input) -\> 数据model变更的双向绑定效果。

### 请详细说下你对vue生命周期的理解？ 

> 总共分为8个阶段创建前/后，载入前/后，更新前/后，销毁前/后。

创建前/后： 在beforeCreated阶段，vue实例的挂载元素\$el和数据对象data都为undefined，还未初始化。在created阶段，vue实例的数据对象data有了，\$el还没有。

载入前/后：在beforeMount阶段，vue实例的\$el和data都初始化了，但还是挂载之前为虚拟的dom节点，data.message还未替换。在mounted阶段，vue实例挂载完成，data.message成功渲染。

更新前/后：当data变化时，会触发beforeUpdate和updated方法。

销毁前/后：在执行destroy方法后，对data的改变不会再触发周期函数，说明此时vue实例已经解除了事件监听以及和dom的绑定，但是dom结构依然存在

### 请说下封装 vue 组件的过程？ 

首先，组件可以提升整个项目的开发效率。能够把页面抽象成多个相对独立的模块，解决了我们传统项目开发：效率低、难维护、复用性等问题。

然后，使用Vue.extend方法创建一个组件，然后使用Vue.component方法注册组件。子组件需要数据，可以在props中接受定义。而子组件修改好数据后，想把数据传递给父组件。可以采用emit方法。

### 你是怎么认识vuex的？ 

vuex可以理解为一种开发模式或框架。比如PHP有thinkphp，java有spring等。

通过状态（数据源）集中管理驱动组件的变化（好比spring的IOC容器对bean进行集中管理）。

应用级的状态集中放在store中； 改变状态的方式是提交mutations，这是个同步的事物； 异步逻辑应该封装在action中。

### vue-loader是什么？使用它的用途有哪些？ 

解析.vue文件的一个加载器，跟template/js/style转换成js模块。

用途：js可以写es6、style样式可以scss或less、template可以加jade等

### 请说出vue.cli项目中src目录每个文件夹和文件的用法？ 

assets文件夹是放静态资源；components是放组件；router是定义路由相关的配置;view视图； app.vue是一个应用主组件；main.js是入口文件

###  vue.cli中怎样使用自定义的组件？有遇到过哪些问题吗？ 

第一步：在components目录新建你的组件文件（smithButton.vue），script一定要export default {

第二步：在需要用的页面（组件）中导入：import smithButton from

'../components/smithButton.vue'

第三步：注入到vue的子组件的components属性上面,components:{smithButton}

第四步：在template视图view中使用，问题有：smithButton命名，使用的时候则smith-button。

### 聊聊你对Vue.js的template编译的理解？ 

简而言之，就是先转化成AST树，再得到的render函数返回VNode（Vue的虚拟DOM节点）详情步骤：

首先，通过compile编译器把template编译成AST语法树（abstract syntax tree 即 源代码的抽象语法结构的树状表现形式），compile是createCompiler的返回值，createCompiler是用以创建编译器的。另外compile还负责合并option。

然后，AST会经过generate（将AST语法树转化成render funtion字符串的过程）得到render函数， render的返回值是VNode，VNode是Vue的虚拟DOM节点，里面有（标签名、子节点、文本等等）

### Vuex是什么？为什么使用Vuex？ 

Vuex 类似 Redux 的状态管理器，用来管理Vue的所有组件状态。

当你打算开发大型单页应用（SPA），会出现多个视图组件依赖同一个状态，来自不同视图的行为需要变更同一个状态。

### vuejs与angularjs的区别？ 

1. 定位 ：虽然Vue.js被定义为MVC framework，但其实Vue本身还是一个library，加了一些其他的工具，可以被当成一个framework，而Angular 2虽然还是一个framework，但其实在设计之初，Angular 2的团队站在了更高的角度，希望做一个platform。

2. 文档：

   vue.js的更加亲切

3. 性能：angular所有的数据和方法都是挂载在\$scope上。而vue的数据和方法都是挂载在vue上，只是数据挂载在vue的data,方法挂载在vue的methods上，vue的代码风格更加优雅，json格式书写代码。Vue.js 有更好的性能，并且非常非常容易优化，因为它不使用脏检查。Angular，当 watcher 越来越多时会变得越来越慢，因为作用域内的每一次变化，所有 watcher 都要重新计算。

其它区别：

渲染性能：Vue\> react \>angular。

使用场景：Vue React 覆盖中小型，大型项目。angular 一般用于大型（因为比较厚重）。

###  vue为什么不直接操作dom？ 

因为操作dom对象后，会触发一些浏览器行为，比如布局（layout）和绘制（paint）。 paint 是一个耗时的过程，然而layout是一个更耗时的过程，我们无法确定layout一定是自上而下或是自下而上进行的，甚至一次layout会牵涉到整个文档布局的重新计算。浏览器的layout是lazy的，也就是说：在 js脚本执行时，是不会去更新DOM的，任何对DOM的修改都会被暂存在一个队列中，在当前js的执行上下文完成执行后，会根据这个队列中的修改，进行一次layout。

### 怎么理解vue是一个渐进式的框架？ 

渐进式就是不必一开始就用Vue所有的全家桶，可以根据场景，按需使用想要的插件。也可以说就使用vue不需要太多的要求。

### Vue声明组件的state是用data方法，那为什么data是通过一个function来返回一个对象，而不是直接写一个对象呢？

> 从语法上说，如果不用function返回就会出现语法错误导致编译不通过。从原理上的话，大概就是组件可以被多次创建，如果不使用function就会使所有调用该组件的页面公用同一个数据域，这样就失去了组件的概念了

###  说下vue组件之间的通信？ 

> 非父子组件间通信，Vue 有提供 Vuex，以状态共享方式来实现同信，对于这一点，应该注意考虑平衡，从整体设计角度去考量，确保引入她的必要。

父传子: this.\$refs.xxx 子传父: this.\$parent.xxx

> 还可以通过\$emit方法出发一个消息，然后\$on接收这个消息

### vue中mixin与extend区别？ 



全局注册混合对象，会影响到所有之后创建的vue实例，而Vue.extend是对单个实例进行扩展。

mixin 混合对象（组件复用）

同名钩子函数（bind，inserted，update，componentUpdate，unbind）将混合为一个数组，因此都将被调用，混合对象的钩子将在组件自身钩子之前调用

methods，components，directives将被混为同一个对象。两个对象的键名（方法名，属性名）冲突时，取组件（而非mixin）对象的键值对。



## 1.前端测试

>  
>
> 为什么要进行测试？
>
> (1)保证代码正确性
>
> (2)放心进行重构
>
> (3)驱动开发TDD
>
> (4)实现自动化测试测试驱动开发它是一种测试先于编写代码的思想用于指导软件开发
>
> 在TDD中侧重点偏向开发，通过测试用例来规范约束开发者编写出质量更高、bug 更少的代码行为驱动开发
>
> 行为驱动开发是一种敏捷软件开发的技术，它鼓励软件项目中的开发者、QA和非技术人员或商业参与者之间的协作
>
> BDD更加侧重设计，其要求在设计测试用例的时候对系统进行定义，倡导使用通用的语言将系统的行为描述出来，将系统设计和测试用例结合起来，从而以此为驱动进行开发工作。
>
> 断言库
>
> 所谓"断言"，就是判断源码的实际执行结果与预期结果是否一致，如果不一致就抛出一个错误。
>
> 它是编写测试用例的关键。断言功能由断言库来实现，Mocha 本身不带断言库，所以必须先引入断言库。
>
> 前端测试流

1. 测试脚本

> 通常，测试脚本与所要测试的源码脚本同名，但是后缀名为.test.js（表示测试）或者.spec.js（表示规格）。

1. mocha

> Mocha 测试用例主要包含下面几部分:
>
> (1)describe 定义的测试套件(test suite)，表示一组相关的测试。
>
> (2)it 定义的测试用例(testcase)，表示一个单独的测试，是测试的最小单位。
>
> (3)测试代码
>
> (4)断言部分

1. Karma

> 可以监控一套文件的变换，并立即开始测试已保存的文件，用户无需离开文本编辑器。
>
> 如果要使用 karma 和 mocha 最好通过npm install karma-cli -g全局安装 karma-cli。

1. Travis.CI

> 提供的是持续集成服务（ContinuousIntegration，简称 CI）。它绑定 Github 上面的项目，只要有新的代码，就会自动抓取。然后，提供一个运行环境，执行测试，完成构建，还能部署到服务器。

## 2.接口文档

>  

1. 什么是接口文档？

> 在项目开发中，web项目的前后端分离开发，APP开发，需要由前后端工程师共同定义接口，编写接口文档，之后大家都根据这个接口文档进行开发，到项目结束前都要一直维护。

1. 为什么要写接口文档？

<!-- -->

1. 项目开发过程中前后端工程师有一个统一的文件进行沟通交流开发
2. 项目维护中或者项目人员更迭，方便后期人员查看、维护

> 三、接口规范是什么？
>
> 首先接口分为四部分：方法、uri、请求参数、返回参数

1. 方法:新增(post) 修改(put) 删除(delete) 获取(get)
2. uri：以/a开头，如果需要登录才能调用的接口(如新增、修改；前台的用户个人信息，资金信息等)后面需要加/u，即：/a/u；中间一般放表名或者能表达这个接口的单词；get方法，如果是后台通过搜索查询列表，那么以/search结尾，如果是前台的查询列表，以/list结尾；url参数就不说了。
3. 请求参数和返回参数，都分为5列：字段、说明、类型、备注、是否必填字段是类的属性；说明是中文释义；类型是属性类型，只有String、Number、 Object、Array四种类型；备注是一些解释，或者可以写一下例子，比如负责json 结构的情况，最好写上例子，好让前端能更好理解；是否必填是字段的是否必填。
4. 返回参数结构有几种情况：

<!-- -->

1. 如果只返回接口调用成功还是失败（如新增、删除、修改等），则只有一个结构体：code和message两个参数；
2. 如果要返回某些参数，则有两个结构体：1是code/mesage/data，2是data 里写返回的参数,data是object类型；
3. 如果要返回列表，那么有三个结构体，1是code/mesage/data,data是

> object，里面放置page/size/total/totalPage/list 5个参数，其中list是
>
> Arrary类型，list里放object，object里是具体的参数。

## 3.webpack和gulp区别（模块化与流的区别）

>  
>
> gulp强调的是前端开发的工作流程，我们可以通过配置一系列的task，定义task 处理的事务（例如文件压缩合并、雪碧图、启动server、版本控制等），然后定义执行顺序，来让gulp执行这些task，从而构建项目的整个前端开发流程。 webpack是一个前端模块化方案，更侧重模块打包，我们可以把开发中的所有资源（图片、js文件、css文件等）都看成模块，通过loader（加载器）和plugins
>
> （插件）对资源进行处理，打包成符合生产环境部署的前端资源。

## 4.redux用处

>  
>
> 在组件化的应用中，会有着大量的组件层级关系，深嵌套的组件与浅层父组件进行数据交互，变得十分繁琐困难。而redux，站在一个服务级别的角度，可以毫无阻碍地将应用的状态传递到每一个层级的组件中。redux就相当于整个应用的管家。

## 6.redux里常用方法

>  
>
> 提供 getState() 方法获取 state；
>
> 提供 dispatch(action) 方法更新 state；
>
> 通过 subscribe(listener) 注册监听器; 等等

## 6.angularJs和react区别

>  
>
> React对比Angular是思想上的转变，它也并不是一个库，是一种开发理念，组件化，分治的管理，数据与view的一体化。它只有一个中心,发出状态，渲染 view，对于虚拟dom它并没有提高渲染页面的性能，它提供更多的是利用jsx 便捷生成dom元素，利用组件概念进行分治管理页面每个部分(例如 header section footer slider)

## 7.vue双向绑定原理

>  
>
> vue数据双向绑定是通过数据劫持结合发布者-订阅者模式的方式来实现的。利用了 Object.defineProperty() 这个方法重新定义了对象获取属性值(get)和设置属性值(set)。

## 8.说说vue react angularjs jquery的区别

>  
>
> JQuery与另外几者最大的区别是，JQuery是事件驱动，其他两者是数据驱动。
>
> JQuery业务逻辑和UI更改该混在一起， UI里面还参杂这交互逻辑，让本来混乱的逻辑更加混乱。
>
> Angular，vue是双向绑定，而React不是其他还有设计理念上的区别等

## 9.node的事件方法讲讲看

>  

emitter.addListener(eventName, listener) ，

> emitter.emit(eventName[, ...args])，emitter.on(eventName, listener)， emitter.removeListener(eventName, listener)等

## 10.node的特性，适合处理什么场景

>  
>
> Node.js借助事件驱动，非阻塞I/O模型变得轻量和高效，非常适合运行在分布式设备的数据密集型实时应用。

## 11.你有用到Express,讲讲Express

>  
>
> Express 是一个简洁而灵活的 node.js Web应用框架, 提供了一系列强大特性帮助你创建各种 Web 应用，和丰富的 HTTP 工具。

# 第六章 移动端开发

## 移动端最小触控区域是多大？

移动端的点击事件的有延迟，时间是多久，为什么会有？ 怎么解决这个延时？（click 有

300ms 延迟,为了实现safari的双击事件的设计，浏览器要知道你是不是要双击操作。）十、NodeJs

## 对Node的优点和缺点提出了自己的看法：

\*（优点）因为Node是基于事件驱动和无阻塞的，所以非常适合处理并发请求，

因此构建在Node上的代理服务器相比其他技术实现（如Ruby）的服务器表现要好得多。

此外，与Node代理服务器交互的客户端代码是由javascript语言编写的，因此客户端和服务器端都用同一种语言编写，这是非常美妙的事情。

\*（缺点）Node是一个相对新的开源项目，所以不太稳定，它总是一直在变，而且缺少足够多的第三方库支持。看起来，就像是Ruby/Rails当年的样子。

## 需求：实现一个页面操作不会整页刷新的网站，并且能在浏览器前进、后退时正确响应。给出你的技术实现方案？

> 至少给出自己的思路（url-hash,可以使用已有的一些框架history.js等）

## Node.js [的适用场景？](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)

1)、实时应用：如在线聊天，实时通知推送等等（如socket.io）

2)、分布式应用：通过高效的并行I/O使用已有的数据

3)、工具类应用：海量的工具，小到前端压缩部署（如grunt），大到桌面图形界面应用程序

4)、游戏类应用：游戏领域对实时和并发有很高的要求（如网易的pomelo框架）

5)、利用稳定接口提升Web渲染能力

6)、前后端编程语言环境统一：前端开发人员可以非常快速地切入到服务器端的开发（如著名的纯Javascript全栈式MEAN架构）

## (如果会用 node)知道 route, middleware, cluster, nodemon, pm2, server-side rendering 么?TODO

> Nodejs 相关概念的理解程度

## TODO解释一下 Backbone 的 MVC 实现方式？

> 流行的MVC架构模式

##  TODO什么是"前端路由"?什么时候适合使用"前端路由"? "前端路由"有哪些优点和缺点?

> 熟悉前后端通信相关知识前端路由就是在不进行后端请求的情况下对页面进行跳转

## 常使用的库有哪些？常用的前端开发工具？开发过什么应用或组件？

使用率较高的框架有jQuery、YUI、Prototype、Dojo、Ext.js、Mootools等。尤其是 jQuery，超过91%。

轻量级框架有Modernizr、underscore.js、backbone.js、Raphael.js等。（理解这些框架的功能、性能、设计原理）

前端开发工具：Sublime Text 、Eclipse、Notepad、Firebug、HttpWatch、Yslow。

开发过的插件：城市选择插件，汽车型号选择插件、幻灯片插件。弹出层。（写过开源程序，加载器，js引擎更好）

## WEB应用从服务器主动推送Data到客户端有那些方式？

html5 websoket

WebSocket通过Flash

XHR长时间连接

XHR Multipart Streaming 不可见的Iframe

\<script\>标签的长时间连接(可跨域

## 平时如何管理你的项目，如何设计突发大规模并发架构？

先期团队必须确定好全局样式（globe.css），编码模式(utf-8) 等

编写习惯必须一致（例如都是采用继承式的写法，单样式都写成一行）；标注样式编写人，各模块都及时标注（标注关键样式调用的地方）；页面进行标注（例如 页面 模块 开始和结束）；

CSS跟HTML 分文件夹并行存放，命名都得统一（例如style.css）

JS 分文件夹存放 命民以该JS 功能为准英文翻译；

[图片采用整合的](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [images.png](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [png8](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [格式文件使用](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png) [尽量](http://jbcdn2.b0.upaiyun.com/2014/10/511748c935cab6e8c46d56b2e6e9c342.png)整合在一起使用方便将来的管理

## 1.介绍一下react

>  
>
> React 是一个用于构建用户界面的 JAVASCRIPT 库。React主要用于构建UI，很多人认为 React 是 MVC 中的 V（视图）
>
> React特点有：
>
> 声明式设计 −React采用声明范式，可以轻松描述应用。
>
> 高效 −React通过对DOM的模拟，最大限度地减少与DOM的交互。
>
> 灵活 −React可以与已知的库或框架很好地配合。
>
> JSX − JSX 是 JavaScript 语法的扩展。React 开发不一定使用 JSX ，但我们建议使用它。
>
> 组件 − 通过 React 构建组件，使得代码更加容易得到复用，能够很好的应用在大项目的开发中。
>
> 单向响应的数据流 − React 实现了单向响应的数据流，从而减少了重复代码，这也是它为什么比传统数据绑定更简单。

## 2.React单项数据流

>  
>
> 在React中，数据是单向流动的，是从上向下的方向，即从父组件到子组件的方向。
>
> state和props是其中重要的概念，如果顶层组件初始化props，那么React会向下遍历整颗组件树，重新渲染相关的子组件。其中state表示的是每个组件中内部的的状态，这些状态只在组件内部改变。
>
> 把组件看成是一个函数，那么他接受props作为参数，内部由state作为函数的内部参数，返回一个虚拟dom的实现。

## 3.react生命周期函数和react组件的生命周期

>  
>
> React的组件在第一次挂在的时候首先获取父组件传递的props，接着获取初始的 state 值，接着经历挂载阶段的三个生命周期函数，也就是 ComponentWillMount，render，ComponentDidMount，这三个函数分别代表组件将会挂载，组件渲染，组件挂载完毕三个阶段，在组件挂载完成后，组件的props 和state的任意改变都会导致组建进入更新状态，在组件更新阶段，如果是props 改 变 ， 则 进 入 ComponentWillReceiveProps 函 数 ， 接 着 进 入 ComponentShouldUpdate进行判断是否需要更新，如果是state改变则直接进入 ComponentShouldUpdate判定，这个默认是true，当判定不需要更新的话，组件继续运行，需要更新的话则依次进入 ComponentWillMount，render， ComponentDidMount 三个函数，当组件卸载时，会首先进入生命周期函数
>
> ComponentWillUnmount,之后才进行卸载，如图
>
> ![](media/image14.jpg){width="5.7716666666666665in" height="3.25in"}
>
> React的生命周期函数：
>
> 初始化阶段：
>
> getDefaultProps获取实例的默认属性，
>
> getInitialState获取每个实例的初始化状态，
>
> ComponentWillMount：组件将被装载，渲染到页面上，render：组件在这里生成虚拟的DOM节点，
>
> ComponentDidMount:组件真正被装载之后
>
> 运行中状态：
>
> componentWillReceiveProps:组件将要接收到属性的时候调用
>
> shouldComponentUpdate:组件接受到新属性或者新状态的时候（可以返回 false，接收数据后不更新，阻止 render 调用，后面的函数不会被继续执行了） shouldComponentUpdate 这个方法用来判断是否需要调用 render 方法重新描绘 dom。因为 dom 的描绘非常消耗性能，如果我们能在
>
> shouldComponentUpdate 方法中能够写出更优化的 domdiff 算法，可以极大的提高性能。
>
> componentWillUpdate:组件即将更新不能修改属性和状态 render:组件重新描绘
>
> componentDidUpdate:组件已经更新销毁阶段： componentWillUnmount:组件即将销毁

## 4.react和Vue的原理，区别，亮点，作用

>  
>
> 曾经看过vue作者尤雨溪的一个专访，他说过这样一段话(大概内容)：做框架的时候我们也很纠结，到底是定制内容少一点好还是定制内容多一点好。定制少了，很多人不知道一些情况应该怎么处理，所以他就乱来，写的代码乱七八糟，性能也不好，然后他就会认为你的框架没做好，有的人还去网上喷你。但是当大家经验越来越丰富，反而希望受到框架的限制越少越好。因为随着经验的增加，大家都知道了各种场景下应该怎么处理，优化自己的代码。限制越少，自我发挥的空间就越大。
>
> 最终我们可以看到，纠结之后，vue的选择居于react与angular之间，框架自身的语法比react多一点，但是又比angular少一点。
>
> 也正是由于选择的不同，所呈现出来的写法与思考方式就一定会有所差异，不论优劣，但肯定会导致不同的偏好。
>
> react的简单在于，它的核心API其实非常少。所以我们会看到很多地方在说 react其实是一个UI库，并不是一个完整的框架。他只是告诉我们如何创建组件以及组件之间如何进行数据传递。甚至于创建组件的方式正是使用ES6的 class语法(createClass将会在react 16被丢弃)。因此开发中react的使用对于ES6的语法依赖非常高。因为react自身本来就没有多少强限制的语法。我们只需要掌握组件里的props，state，ref，生命周期，就好像没有过多额外的知识了。就连如果想要在jsx模板来遍历渲染，还得使用原生的map方法。而react的高阶组件，理解之后发现，其实就是JavaScript 函数式编程中所涉及到的思维方式。
>
> 所以在我看来，react的最大特点就是简单并且与原生JavaScript非常接近。即给开发者带来的束缚非常少。一个功能的实现，如果你知道使用原生 JavaScript如何实现，那么你就一定能够很轻松的知道使用react如何实现。
>
> 当然，核心API简单并不代表上手容易。在使用之初，如果你经验缺乏，那么你用react写出来的页面，性能可能会非常差。因为无意识的，你的组件可能会有非常多的多余的渲染。
>
> 比如很多人在学习react的时候，会接触到一个倒计时的例子，这个例子使用修改组件中state的方式来实现。但是其实后来大家会慢慢知道，这种方式是非常错误的。因为state的每次修改，都会导致组件及其所有子组件的重新渲染。这是成本非常高的行为。当然，我还知道很多人，在调试react的时候，由于高频的重复渲染直接把浏览器都卡死的。这些问题都是尤雨溪所担心的限制过少带来的。
>
> 网上有的自以为牛逼的人，用着react/vue这样的框架，其实写着很烂的代码，恐怖的是他们还嘲讽这嘲讽那的。还遇到过一个人，口口声声说自己用了 angular好多年，说angular真的好垃圾啊，性能好差啊，什么什么的各种黑，结果连track by都不会用。而react由于没有真正意义上的双向绑定。因此在处理一些复杂场景会非常麻烦，比如复杂的表单验证。而相对而言，vue提供的能力则更多一点，这些便捷的能力会让初学者感觉到非常的幸福，因为很多效果只需要一些简单的代码既可以实现。我大概列举几条我个人认为非常棒的能力：
>
> 统一管理的计算属性
>
> JavaScript的表达式非常便利，无论是vue还是react，表达式的能力是必不可
>
> 少的。但正如vue官方文档所说，在模板中放入太多的逻辑会让模板过重且难以维护。而vue的组件中提供了一个计算属性来统一管理表达式。
>
> <template>
>
> </div>
>
> </template> <script>
>
> export default { name: 'example',
>
> data () {
>
> return { message: 'Hello'
>
> } }, computed: { reversedMessage: function() { return this.message.split('').reverse().join('')
>
> } } }
>
> </script>
>
> class的动态语法让我感觉非常爽
>
> 在实践中我们会发现非常多这样的场景，需要根据不同的状态来决定一个元素 class的具体值。而如果仅仅只是简单的表达式或者条件判断在jsx模板中，例如下面这个样子就会让人感觉非常难受
>
> 当稍微复杂一点的逻辑还这样处理就是难受到忍不了了。而vue中支持的语法则非常轻松的搞定了这个问题。
>
> // 可以放在任何你觉得舒服的位置 const pcls = {
>
> active: active, note: true
>
> }
>
> 这样我们继续添加更多的class名也不会造成额外的复杂度了。
>
> 当然，这仅仅只是一个工具方法就能搞定的问题，在使用react时，大家可以借助classnames来完成同样的功能。但vue是直接支持了。
>
> 双向绑定由于react并不支持双向绑定，因此在复杂的表单验证时实现起来非常痛苦。而 vue在以单向数据流为核心的同时，又没有完全抛弃双向绑定，这让在这样复杂的表单验证场景开发效率比react高出非常多。这也是vue省事儿的一个方面。
>
> 修饰符
>
> 我们在写事件处理逻辑时，常常需要e.preventDefault等操作。vue提供的修饰符功能可以帮助我们省去这些代码，极为方便。用多了就会发现，真TM好用。
>
> <!-- 阻止单击事件冒泡 -->
>
> <!-- 提交事件不再重载页面 -->
>
> 1<form v-on:submit.prevent="onSubmit"></form>
>
> <!-- 修饰符可以串联 -->
>
> <!-- 只有修饰符 -->
>
> <form v-on:submit.prevent></form>
>
> <!-- 添加事件侦听器时使用事件捕获模式 -->
>
> <!-- 只当事件在该元素本身（而不是子元素）触发时触发回调 -->
>
> 当然，还有按键修饰符等，可以去官网进一步查看学习。
>
> vue提供的方便可爱的语法糖还有很多，就不细说，大家可以在官网上一一体验。正如文章开头所说，vue会有一些语法限制，而这些语法限制在某种程度上来说降低了我们的开发成本，提高了开发效率。这大概也就是很多人认为vue更加简单易学的原因所在吧。
>
> 就从学习难易程度上来说，react之所以上手更加困难，主要的原因并不在于 react本身，而在于围绕react的丰富的生态圈。正是由于react本身足够简单，所以我们需要掌握的react组件就更多。比如react-router，react-redux等。
>
> 而且很多好用的，功能特别棒的组件在我们涉猎不广的时候都不知道。

## 5.reactJs的组件交流

>  
>
> React组件之间的交流方式可以分为以下三种

1. 父组件向子组件传值:主要是利用props来进行交流
2. 子组件向父组件传值：子组件通过控制自己的state然后告诉父组件的点击状态。然后在父组件中展示出来，如图

> ![](media/image15.jpg){width="5.7716666666666665in" height="3.135in"}

1. 没有任何嵌套关系的组件之间传值：如果组件之间没有任何关系，组件嵌套层次比较深（个人认为 2 层以上已经算深了），或者你为了一些组件能够订阅、写入一些信号，不想让组件之间插入一个组件，让两个组件处于独立的关系。对于事件系统，这里有 2 个基本操作步骤：订阅（subscribe）/监听（listen）一个事件通知，并发送（send）/触发（trigger）/发布（publish）/发送（dispatch）一个事件通知那些想要的组件。

## 6.有了解过react的虚拟DOM吗，虚拟DOM是怎么对比的呢

>  
>
> 当然是使用的diff算法，diff算法有三种优化形式：

1. treediff：将新旧两颗DOM树按照层级遍历，只对同级的DOM节点进行比较，即同一父节点下的所有子节点，当发现节点已经不存在，则该节点及其子节点会被完全删除，不会进一步比较
2. component diff：不同组件之间的对比，如果组件类型相同，暂不更新，

> 否则删除旧的组件，再创建一个新的组件，插入到删除组件的位置

1. element diff:在类型相同的组件内，再继续对比组件内部的元素

## 7.项目里用到了react，为什么要选择react，react有哪些好处

>  

1. 声明式设计
2. 高效：通过对DOM的模拟，最大限度的减少与DOM的交互。
3. 灵活：可以与已知的框架或库很好的配合。
4. JSX：是js语法的扩展，不一定使用，但建议用。（5）组件：构建组件，使代码更容易得到复用，能够很好地应用在大项目的开发中。

> （6）单向响应的数据流：React实现了单向响应的数据流，从而减少了重复代码，这也是解释了它为什么比传统数据绑定更简单。

## 8.怎么获取真正的dom

>  
>
> ReactDOM.findDOMNode()或this.refs
>
> 9.选择react的原因

## 10.react的生命周期函数

>  
>
> 初始化

1. getDefaultProps()

> 设置默认的props，也可以用dufaultProps设置组件的默认属性.

1. getInitialState()

> 在使用es6的class语法时是没有这个钩子函数的，可以直接在constructor 中定义this.state。此时可以访问this.props

1. componentWillMount()

> 组件初始化时只调用，以后组件更新不调用，整个生命周期只调用一次，此时可以修改state。

1. render()

> react最重要的步骤，创建虚拟dom，进行diff算法，更新dom树都在此进行。
>
> 此时就不能更改state了。

1. componentDidMount()

> 组件渲染之后调用，只调用一次。
>
> 更新

1. componentWillReceiveProps(nextProps)

> 组件初始化时不调用，组件接受新的props时调用。 7）shouldComponentUpdate(nextProps, nextState)
>
> react性能优化非常重要的一环。组件接受新的state或者props时调用，我们可以设置在此对比前后两个props和state是否相同，如果相同则返回false 阻止更新，因为相同的属性状态一定会生成相同的dom树，这样就不需要创造新的dom树和旧的dom树进行diff算法对比，节省大量性能，尤其是在dom结构复杂的时候

1. componentWillUpdata(nextProps, nextState)

> 组件初始化时不调用，只有在组件将要更新时才调用，此时可以修改state

1. render() 组件渲染
2. componentDidUpdate()

> 组件初始化时不调用，组件更新完成后调用，此时可以获取dom节点。
>
> 卸载

1. componentWillUnmount()

> 组件将要卸载时调用，一些事件监听和定时器需要在此时清除。

## 11.setState之后的流程

>  
>
> 在代码中调用setState函数之后，React 会将传入的参数对象与组件当前的状态合并，然后触发所谓的调和过程（Reconciliation）。 经过调和过程，React 会以相对高效的方式根据新的状态构建 React 元素树并且着手重新渲染整个 UI界面。 在 React 得到元素树之后，React 会自动计算出新的树与老树的节点差异，然后根据差异对界面进行最小化重渲染。在差异计算算法中，React 能够相对精确地知道哪些位置发生了改变以及应该如何改变，这就保证了按需更新，而不是全部重新渲染。

## 12.react高阶组件知道吗？

>  
>
> 高阶组件接收React组件作为参数，并且返回一个新的React组件。高阶组件本质上也是一个函数，并不是一个组件。

## 13.React的生命周期

>  
>
> React 生命周期分为三种状态
>
> 1.初始化
>
> 2.更新
>
> 3.销毁
>
> 具体见下图：
>
> ![](media/image16.jpg){width="4.913333333333333in" height="5.9816666666666665in"}

## 14.说说自己理解的react

>  
>
> React是用于构建用户界面的JavaScript库。React可以创建交互式UI。为应用程序中的每个状态建立的视图，并且React将在数据更改时进行更新，呈现正确的组件。另外，我们也可以构建管理自己状态的封装组件，然后将它们组合成复杂的UI。因为组件用JS编写而不是模板，所以可以通过应用传递数据，并使状态与DOM分离

## 15.react的组件是通过什么去判断是否刷新的

>  
>
> 通过state是否改变

# 第七章 计算机基础

## 说一下http和https

 

https的SSL加密是在传输层实现的。

### (1)http和https的基本概念

http: 超文本传输协议，是互联网上应用最为广泛的一种网络协议，是一个客户端和服务器端请求和应答的标准（TCP），用于从WWW服务器传输超文本到本地

浏览器的传输协议，它可以使浏览器更加高效，使网络传输减少。

https: 是以安全为目标的HTTP通道，简单讲是HTTP的安全版，即HTTP下加入SSL层，HTTPS的安全基础是SSL，因此加密的详细内容就需要SSL。

https协议的主要作用是：建立一个信息安全通道，来确保数组的传输，确保网站的真实性。

### (2)http和https的区别？

http传输的数据都是未加密的，也就是明文的，网景公司设置了SSL协议来对 http协议传输的数据进行加密处理，简单来说https协议是由http和ssl协议构建的可进行加密传输和身份认证的网络协议，比http协议的安全性更高。

主要的区别如下：

a.Https协议需要ca证书，费用较高。

b.http是超文本传输协议，信息是明文传输，https则是具有安全性的ssl加密传输协议。

c.使用不同的链接方式，端口也不同，一般而言，http协议的端口为80，https 的端口为443

d.http的连接很简单，是无状态的；HTTPS协议是由SSL+HTTP协议构建的可进行加密传输、身份认证的网络协议，比http协议安全。

### (3)https协议的工作原理客户端在使用HTTPS方式与Web服务器通信时有几个步骤。

a.客户使用https url访问服务器，则要求web 服务器建立ssl链接。

b.web服务器接收到客户端的请求之后，会将网站的证书（证书中包含了公钥），返回或者说传输给客户端。

c.客户端和web服务器端开始协商SSL链接的安全等级，也就是加密等级。

d.客户端浏览器通过双方协商一致的安全等级，建立会话密钥，然后通过网站的公钥来加密会话密钥，并传送给网站。

e.web服务器通过自己的私钥解密出会话密钥。

f.web服务器通过会话密钥加密与客户端之间的通信。

### (4)https协议的优点

使用HTTPS协议可认证用户和服务器，确保数据发送到正确的客户机和服务器；

HTTPS协议是由SSL+HTTP协议构建的可进行加密传输、身份认证的网络协议，要比http协议安全，可防止数据在传输过程中不被窃取、改变，确保数据的完整性。

HTTPS是现行架构下最安全的解决方案，虽然不是绝对安全，但它大幅增加了中间人攻击的成本。

谷歌曾在2014年8月份调整搜索引擎算法，并称"比起同等HTTP网站，采用

HTTPS加密的网站在搜索结果中的排名将会更高"。

### (5)https协议的缺点

https握手阶段比较费时，会使页面加载时间延长50%，增加10%~20%的耗电。

https缓存不如http高效，会增加数据开销。

SSL证书也需要钱，功能越强大的证书费用越高。

SSL证书需要绑定IP，不能再同一个ip上绑定多个域名，ipv4资源支持不了这种消耗。



## 10.说一下http2.0

 首先补充一下，http和https的区别，相比于http,https是基于ssl加密的http 协议

简要概括：http2.0是基于1999年发布的http1.0之后的首次更新。

提升访问速度（可以对于，请求资源所需时间更少，访问速度更快，相比http1.0）

允许多路复用：多路复用允许同时通过单一的HTTP/2连接发送多重请求-响应信息。

改善了：在http1.1中，浏览器客户端在同一时间，针对同一域名下的请求有一定数量限制（连接数量），超过限制会被阻塞。

二进制分帧：HTTP2.0会将所有的传输信息分割为更小的信息或者帧，并对他们进行二进制编码。

首部压缩服务器端推送

## 介绍知道的http返回的状态码

100  Continue  继续。客户端应继续其请求

101  Switching Protocols  切换协议。服务器根据客户端的请求切换协议。只能切换到更高级的协议，例如，切换到HTTP的新版本协议

200  OK  请求成功。一般用于GET与POST请求

201  Created  已创建。成功请求并创建了新的资源

202  Accepted  已接受。已经接受请求，但未处理完成

203  Non-Authoritative Information  非授权信息。请求成功。但返回的meta信息不在原始的服务器，而是一个副本

204  No Content  无内容。服务器成功处理，但未返回内容。在未更新网页的情况下，可确保浏览器继续显示当前文档

205  Reset Content  重置内容。服务器处理成功，用户终端（例如：浏览器）应重置文档视图。可通过此返回码清除浏览器的表单域

206  Partial Content  部分内容。服务器成功处理了部分GET请求

300  Multiple Choices  多种选择。请求的资源可包括多个位置，相应可返回一个资源特征与地址的列表用于用户终端（例如：浏览器）选择

301  Moved Permanently  永久移动。请求的资源已被永久的移动到新URI，返回信息会包括新的URI，浏览器会自动定向到新URI。今后任何新的请求都应使用新的URI代替

302  Found  临时移动。与301类似。但资源只是临时被移动。客户端应继续使用原有URI

303  See Other  查看其它地址。与301类似。使用GET和POST请求查看

304  Not Modified  未修改。所请求的资源未修改，服务器返回此状态码时，不会返回任何资源。客户端通常会缓存访问过的资源，通过提供一个头信息指出客户端希望只返回在指定日期之后修改的资源

305  Use Proxy  使用代理。所请求的资源必须通过代理访问

306  Unused  已经被废弃的HTTP状态码

307  Temporary Redirect  临时重定向。与302类似。使用GET请求重定向

400  Bad Request  客户端请求的语法错误，服务器无法理解

401  Unauthorized  请求要求用户的身份认证

402  Payment Required  保留，将来使用

403  Forbidden  服务器理解请求客户端的请求，但是拒绝执行此请求

404  Not Found  服务器无法根据客户端的请求找到资源（网页）。通过此代码，网站设计人员可设置"您所请求的资源无法找到"的个性页面

405  Method Not Allowed  客户端请求中的方法被禁止

406  Not Acceptable  服务器无法根据客户端请求的内容特性完成请求

407  Proxy Authentication Required  请求要求代理的身份认证，与401类似，但请求者应当使用代理进行授权

408  Request Time-out  服务器等待客户端发送的请求时间过长，超时

409  Conflict  服务器完成客户端的PUT请求是可能返回此代码，服务器处理请求时发生了冲突

410  Gone  客户端请求的资源已经不存在。410不同于404，如果资源以前有现在被永久删除了可使用410代码，网站设计人员可通过301代码指定资源的新位置

411  Length Required  服务器无法处理客户端发送的不带Content-Length的请求信息

412  Precondition Failed  客户端请求信息的先决条件错误

413  Request Entity Too Large  由于请求的实体过大，服务器无法处理，因此拒绝请求。为防止客户端的连续请求，服务器可能会关闭连接。如果只是服务器暂时无法处理，则会包含一个Retry-After的响应信息

414  Request-URI Too Large  请求的URI过长（URI通常为网址），服务器无法处理

415  Unsupported Media Type  服务器无法处理请求附带的媒体格式

416  Requested range not satisfiable  客户端请求的范围无效

417  Expectation Failed  服务器无法满足Expect的请求头信息

500  Internal Server Error  服务器内部错误，无法完成请求

501  Not Implemented  服务器不支持请求的功能，无法完成请求

502  Bad Gateway  作为网关或者代理工作的服务器尝试执行请求时，从远程服务器接收到了一个无效的响应

503  Service Unavailable  由于超载或系统维护，服务器暂时的无法处理客户端的请求。延时的长度可包含在服务器的Retry-After头信息中

504  Gateway Time-out  充当网关或代理的服务器，未及时从远端服务器获取请求

505  HTTP Version not supported  服务器不支持请求的HTTP协议的版本，无法完成处理

## http常用请求头

| 协议头              | 说明                                                         |
| ------------------- | ------------------------------------------------------------ |
| Accept              | 可接受的响应内容类型（Content-Types）。                      |
| Accept-Charset      | 可接受的字符集                                               |
| Accept-Encoding     | 可接受的响应内容的编码方式。                                 |
| Accept-Language     | 可接受的响应内容语言列表。                                   |
| Accept-Datetime     | 可接受的按照时间来表示的响应内容版本                         |
| Authorization       | 用于表示HTTP协议中需要认证资源的认证信息                     |
| Cache-Control       | 用来指定当前的请求/回复中的，是否使用缓存机制。              |
| Connection          | 客户端（浏览器）想要优先使用的连接类型                       |
| Cookie              | 由之前服务器通过Set-Cookie（见下文）设置的一个HTTP协议Cookie |
| Content-Length      | 以8进制表示的请求体的长度                                    |
| Content-MD5         | 请求体的内容的二进制 MD5 散列值（数字签名），以 Base64 编码的结果 |
| Content-Type        | 请求体的MIME类型 （用于POST和PUT请求中）                     |
| Date                | 发送该消息的日期和时间（以[RFC 7231](https://www.nowcoder.com/tutorial/96/24304825a0c04ea9a53cdb09cb664834#section-7.1.1.1)中定义的"HTTP日期"格式来发送） |
| Expect              | 表示客户端要求服务器做出特定的行为                           |
| From                | 发起此请求的用户的邮件地址                                   |
| Host                | 表示服务器的域名以及服务器所监听的端口号。如果所请求的端口是对应的服务的标准端口（80），则端口号可以省略。 |
| If-Match            | 仅当客户端提供的实体与服务器上对应的实体相匹配时，才进行对应的操作。主要用于像 PUT 这样的方法中，仅当从用户上次更新某个资源后，该资源未被修改的情况下，才更新该资源。 |
| If-Modified-Since   | 允许在对应的资源未被修改的情况下返回304未修改                |
| If-None-Match       | 允许在对应的内容未被修改的情况下返回304未修改（ 304 Not Modified ），参考 超文本传输协议 的实体标记 |
| If-Range            | 如果该实体未被修改过，则向返回所缺少的那一个或多个部分。否则，返回整个新的实体 |
| If-Unmodified-Since | 仅当该实体自某个特定时间以来未被修改的情况下，才发送回应。   |
| Max-Forwards        | 限制该消息可被代理及网关转发的次数。                         |
| Origin              | 发起一个针对[跨域资源共享](http://itbilu.com/javascript/js/VkiXuUcC.html)的请求（该请求要求服务器在响应中加入一个Access-Control-Allow-Origin的消息头，表示访问控制所允许的来源）。 |
| Pragma              | 与具体的实现相关，这些字段可能在请求/回应链中的任何时候产生。 |
| Proxy-Authorization | 用于向代理进行认证的认证信息。                               |
| Range               | 表示请求某个实体的一部分，字节偏移以0开始。                  |
| Referer             | 表示浏览器所访问的前一个页面，可以认为是之前访问页面的链接将浏览器带到了当前页面。Referer其实是Referrer这个单词，但RFC制作标准时给拼错了，后来也就将错就错使用Referer了。 |
| TE                  | 浏览器预期接受的传输时的编码方式：可使用回应协议头Transfer-Encoding中的值（还可以使用"trailers"表示数据传输时的分块方式）用来表示浏览器希望在最后一个大小为0的块之后还接收到一些额外的字段。 |
| User-Agent          | 浏览器的身份标识字符串                                       |
| Upgrade             | 要求服务器升级到一个高版本协议。                             |
| Via                 | 告诉服务器，这个请求是由哪些代理发出的。                     |
| Warning             | 一个一般性的警告，表示在实体内容体中可能存在错误。           |

## 11.补充400和401、403状态码

(1)400状态码：请求无效产生原因：前端提交数据的字段名称和字段类型与后台的实体没有保持一致

前端提交到后台的数据应该是json字符串类型，但是前端没有将对象

JSON.stringify转化成字符串。

解决方法：

对照字段的名称，保持一致性

将obj对象通过JSON.stringify实现序列化

(2)401状态码：当前请求需要用户验证

(3)403状态码：服务器已经得到请求，但是拒绝执行

## 12.fetch发送2次请求的原因

fetch发送post请求的时候，总是发送2次，第一次状态码是204，第二次才成功？

原因很简单，因为你用fetch的post请求的时候，导致fetch 第一次发送了一个Options请求，询问服务器是否支持修改的请求头，如果服务器支持，则在第二次中发送真正的请求。

## 33.GET和POST的区别

- get参数通过url传递，post放在request body中。

- get请求在url中传递的参数是有长度限制的，而post没有。 get比post更不安全，因为参数直接暴露在url中，所以不能用来传递敏感信息。

- get请求只能进行url编码，而post支持多种编码方式

- get请求会浏览器主动cache，而post支持多种编码方式。

- get请求参数会被完整保留在浏览历史记录里，而post中的参数不会被保留。 GET和POST本质上就是TCP链接，并无差别。但是由于HTTP的规定和浏览器/ 服务器的限制，导致他们在应用过程中体现出一些不同。

- GET产生一个TCP数据包；POST产生两个TCP数据包。

- GET 参数通过 url 传递，POST 放在 body 中。（http 协议规定，url 在请求头中，所以大小限制很小）

  GET 请求在 url 中传递的参数是有长度限制的，而 POST 没有。原因见上↑↑↑

  GET 在浏览器回退时是无害的，而 POST 会再次提交请求

  **GET 产生一个 TCP 数据包；POST 产生两个 TCP 数据包**。对于 GET 方式的请求，浏览器会把 http 的 header 和 data 一并发送出去，服务器响应200（返回数据）。而对于 POST，浏览器先发送 header，服务器响应100 continue，浏览器再发送 data，服务器响应200 ok（返回数据）

## 301和302的区别

 

301MovedPermanently 被请求的资源已永久移动到新位置，并且将来任何对此资源的引用都应该使用本响应返回的若干个URI之一。如果可能，拥有链接编辑功能的客户端应当自动把请求的地址修改为从服务器反馈回来的地址。除非额外指定，否则这个响应也是可缓存的。

302Found 请求的资源现在临时从不同的URI响应请求。由于这样的重定向是临时的，客户端应当继续向原有地址发送以后的请求。只有在Cache-Control或

Expires中进行了指定的情况下，这个响应才是可缓存的。字面上的区别就是301 是永久重定向，而302是临时重定向。

301比较常用的场景是使用域名跳转。302用来做临时跳转 比如未登陆的用户访问用户中心重定向到登录页面。

## Cookie、sessionStorage、localStorage的区别

共同点：都是保存在浏览器端，并且是同源的

Cookie：cookie数据始终在同源的http请求中携带（即使不需要），即cookie 在浏览器和服务器间来回传递。而sessionStorage和localStorage不会自动把数据发给服务器，仅在本地保存。cookie数据还有路径（path）的概念，可以限制cookie只属于某个路径下,存储的大小很小只有4K左右。 （key：可以在浏览器和服务器端来回传递，存储容量小，只有大约4K左右） sessionStorage：仅在当前浏览器窗口关闭前有效，自然也就不可能持久保持， localStorage：始终有效，窗口或浏览器关闭也一直保存，因此用作持久数据； cookie只在设置的cookie过期时间之前一直有效，即使窗口或浏览器关闭。

（key：本身就是一个回话过程，关闭浏览器后消失，session为一个回话，当页面不同即使是同一页面打开两次，也被视为同一次回话）

localStorage：localStorage 在所有同源窗口中都是共享的；cookie也是在所有同源窗口中都是共享的。（key：同源窗口都会共享，并且不会失效，不管窗口或者浏览器关闭与否都会始终生效）补充说明一下cookie的作用：

1. 保存用户登录状态

> 例如将用户id存储于一个cookie内，这样当用户下次访问该页面时就不需要重新登录了，现在很多论坛和社区都提供这样的功能。
>
> cookie还可以设置过期时间，当超过时间期限后，cookie就会自动消失。因此，系统往往可以提示用户保持登录状态的时间：常见选项有一个月、三个 月、一年等。

1. 跟踪用户行为

> 例如一个天气预报网站，能够根据用户选择的地区显示当地的天气情况。如果每次都需要选择所在地是烦琐的，当利用了cookie后就会显得很人性化了，系统能够记住上一次访问的地区，当下次再打开该页面时，它就会自动显示上次用户所在地区的天气情况。
>
> 因为一切都是在后台完成，所以这样的页面就像为某个用户所定制的一样，使用起来非常方便定制页面。如果网站提供了换肤或更换布局的功能，那么可以使用 cookie来记录用户的选项，例如：背景色、分辨率等。当用户下次访问时，仍然可以保存上一次访问的界面风格。

## 14.说一下web worker

在HTML页面中，如果在执行脚本时，页面的状态是不可响应的，直到脚本执行完成后，页面才变成可响应。webworker是运行在后台的js，独立于其他脚本，不会影响页面你的性能。并且通过postMessage将结果回传到主线程。这样在进行复杂操作的时候，就不会阻塞主线程了。

如何创建web worker：

检测浏览器对于web worker的支持性

创建web worker文件（js，回传函数等）创建web worker对象

## .tcp三次握手，一句话概括

 

客户端和服务端都需要直到各自可收发，因此需要三次握手。

简化三次握手：

`src="https://user-images.githubusercontent.com/17233651/42496289-1c6d 668a-8458-11e8-98b3-65db50f64d48.png">` 从图片可以得到三次握手可以简化为：

C发起请求连接S确认，也发起连接C确认每次握手的作用：

第一次握手：S只可以确认自己可以接受C发送的报文段；

第二次握手：C可以确认S收到了自己发送的报文段，并且可以确认自己可以接受S发送的报文段；第三次握手：S可以确认 C收到了自己发送的报文段；

## ★★**在地址栏里输入一个URL,到这个页面呈现出来，中间会发生什么？**★★

1. 当发送一个 URL 请求时，不管这个 URL 是 Web 页面的 URL 还是 Web 页面上每个资源 的 URL，浏览器都会开启一个线程来处理这个请求，同时在远程 DNS 服务器上**启动一个 DNS 查询**。这能使浏览器**获得请求对应的 IP 地址**。 
2. 浏览器与远程 Web 服务器通过 **TCP 三次握手协商来建立一个 TCP/IP 连接**。该握手包 括一个同步报文，一个同步-应答报文和一个应答报文，这三个报文在 浏览器和服务器之间 传递。该握手首先由客户端尝试建立起通信，而后服务器应答并接受客户端的请求，最后由 客户端发出该请求已经被接受的报文。 
3. 一旦 TCP/IP 连接建立，浏览器会通过该连接向远程服务器**发送 HTTP 的 GET 请求**。远 程服务器找到资源并使用 HTTP 响应返回该资源，值为 200 的 HTTP 响应状态表示一个正 确的响应。 
4. 此时，Web 服务器提供资源服务，**客户端开始下载资源**。

------

输入url后，首先需要找到这个url域名的服务器ip,为了寻找这个ip，浏览器首先会寻找缓存，查看缓存中是否有记录，缓存的查找记录为：浏览器缓存-》系统缓存-》路由器缓存，缓存中没有则查找系统的hosts文件中是否有记录，如果没有则查询DNS服务器.

得到服务器的ip地址后，浏览器根据这个ip以及相应的端口号，构造一个http请求，这个请求报文会包括这次请求的信息，主要是请求方法，请求说明和请求附带的数据，并将这个http请求封装在一个tcp 包中，这个tcp包会依次经过传输层，网络层，数据链路层，物理层到达服务器.

服务器解析这个请求来作出响应，返回相应的html给浏览器.

因为html是一个树形结构，浏览器根据这个html来构建DOM树，在dom树的构建过程中如果遇到JS脚本和外部JS连接，则会停止构建DOM树来执行和下载相应的代码，这会造成阻塞，这就是为什么推荐JS代码应该放在html代码的后面，之后根据外部样式，内部样式，内联样式构建一个CSS对象模型树CSSOM树，构建完成后和 DOM树合并为渲染树，这里主要做的是排除非视觉节点，比如script，meta标签和排除display为none的节点，之后进行布局，布局主要是确定各个元素的位置和尺寸，之后是渲染页面，因为html文件中会含有图片，视频，音频等资源，在解析DOM的过程中，遇到这些都会进行并行下载，浏览器对每个域的并行下载数量有一定的限制，一般是4-6个.

当然在这些所有的请求中我们还需要关注的就是缓存，缓存一般通过Cache-Control、Last-Modify、Expires等首部字段控制。Cache-Control和Expires的区别在于Cache-Control使用相对时间，Expires使用的是基于服务器 端的绝对时间，因为存在时差问题，一般采用Cache-Control，在请求这些有设置了缓存的数据时，会先 查看是否过期，如果没有过期则直接使用本地缓存，过期则请求并在服务器校验文件是否修改，如果上一次 响应设置了ETag值会在这次请求的时候作为If-None-Match的值交给服务器校验，如果一致，继续校验 Last-Modified，没有设置ETag则直接验证Last-Modified，再决定是否返回304

## 40.cookie和session的区别，localstorage和 sessionstorage的区别

Cookie和session都可用来存储用户信息，cookie存放于客户端，session存放于服务器端，因为cookie存放于客户端有可能被窃取，所以cookie一般用来存放不敏感的信息，比如用户设置的网站主题，敏感的信息用session存储，比如用户的登陆信息，session可以存放于文件，数据库，内存中都可以，cookie 可以服务器端响应的时候设置，也可以客户端通过JS设置cookie会在请求时在 http首部发送给客户端，cookie一般在客户端有大小限制，一般为4K。下面从几个方向区分一下cookie，localstorage，sessionstorage的区别：

- 生命周期：

> Cookie：可设置失效时间，否则默认为关闭浏览器后失效
>
> Localstorage:除非被手动清除，否则永久保存
>
> Sessionstorage：仅在当前网页会话下有效，关闭页面或浏览器后就会被清除

- 存放数据：

> Cookie：4k左右
>
> Localstorage和sessionstorage：可以保存5M的信息

- http请求：

> Cookie：每次都会携带在http头中，如果使用cookie保存过多数据会带来性能问题
>
> 其他两个：仅在客户端即浏览器中保存，不参与和服务器的通信

- 易用性：

> Cookie：需要程序员自己封装，原生的cookie接口不友好其他两个：即可采用原生接口，亦可再次封装

- 应用场景：

> 从安全性来说，因为每次http请求都回携带cookie信息，这样子浪费了带宽，所以cookie应该尽可能的少用，此外cookie还需要指定作用域，不可以跨域调用，限制很多，但是用户识别用户登陆来说，cookie还是比storage好用，其他情况下可以用storage，localstorage可以用来在页面传递参数，
>
> sessionstorage可以用来保存一些临时的数据，防止用户刷新页面后丢失了一些参数。

## 41.常见的HTTP的头部

 可以将http首部分为通用首部，请求首部，响应首部，实体首部

通用首部表示一些通用信息

date表示报文创建时间，请求首部就是请求报文中独有的； cookie，和缓存相关的；

if-Modified-Since响应首部就是响应报文中独有的； set-cookie，和重定向相关的location，

实体首部用来描述实体部分

allow用来描述可执行的请求方法 content-type描述主题类型 content-Encoding描述主体的编码方式

## 42.HTTP2.0 的特性

http2.0的特性如下：

1. 内容安全，应为http2.0是基于https的，天然具有安全特性，通过http2.0 的特性可以避免单纯使用https的性能下降；
2. 二进制格式，http1.X的解析是基于文本的，http2.0将所有的传输信息分割为更小的消息和帧，并对他们采用二进制格式编码，基于二进制可以让协议有更多的扩展性，比如引入了帧来传输数据和指令； 3）多路复用，这个功能相当于是长连接的增强，每个request请求可以随机的混杂在一起，接收方可以根据request的id将request再归属到各自不同的服务端请求里面，另外多路复用中也支持了流的优先级，允许客户端告诉服务器那些内容是更优先级的资源，可以优先传输；

## 43.cache-control的值有哪些todo

cache-control是一个通用消息头字段被用于HTTP请求和响应中，通过指定指令来实现缓存机制，这个缓存指令是单向的，常见的取值有private、no-cache、 max-age、must-revalidate等，默认为private。

## 44.浏览器在生成页面的时候，会生成那两颗树？

 

构造两棵树，DOM树和CSSOM规则树

当浏览器接收到服务器相应来的HTML文档后，会遍历文档节点，生成DOM树，

CSSOM规则树由浏览器解析CSS文件生成。

## DDOS 攻击

### **什么是 DDOS 攻击**

分布式拒绝服务攻击(Distributed denial of service attack) 向目标系统同时提出数量庞大的服务请求。

### **DDOS 攻击方式**

- 通过使网络过载来干扰甚至阻断正常的网络通讯；
- 通过向服务器提交大量请求，使服务器超负荷；
- 阻断某一用户访问服务器；
- 阻断某服务与特定系统或个人的通讯。

### **如何应对 DDOS 攻击**

- 黑名单
- DDOS 清洗：对用户请求数据进行实时监控，及时发现DOS攻击等异常流量，在不影响正常业务开展的情况下清洗掉这些异常流量。
- CDN 加速
- 高防服务器：高防服务器主要是指能独立硬防御 50Gbps 以上的服务器，能够帮助网站拒绝服务攻击，定期扫描网络主节点

## http请求过程 

对www.abc.com这个网址进行DNS域名解析，得到对应的IP地址根据这个IP，找到对应的服务器，发起TCP的三次握手建立TCP连接后发起HTTP请求

服务器响应HTTP请求，浏览器得到html代码

浏览器解析html代码，并请求html代码中的资源（如js、css、图片等）（先得到html代码，才能去找这些资源）

浏览器对页面进行渲染呈现给用户

服务器关闭关闭TCP连接

### DNS 域名如何解析的？

DNS域名解析采用的是递归查询的方

先去找DNS缓存-\>缓存找不到就去找根域名服务器-\>根域名又会去找下一级，递归查找之后，找到了，给我们的web浏览器。

1.  浏览器首先搜索**自身的DNS缓存**，看缓存中是否有 www.abc.com 这个域名，有而且没有过期的话，解析结束。

2.  如果浏览器自身的缓存中没有找到，则会搜索**操作系统自身的DNS缓存**，如果找到且没有过期则停止搜索，解析到此结束。

3.  如果在操作系统的DNS缓存中也没有找到，那么尝试读取**hosts文件**，有则解析成功，解析到此结束。

4.  如果在hosts文件中也没有找到，浏览器会发起一个

DNS（Domain Name System：域名服务协议）**系统调用，向本地配置的首选DNS服务器**发起域名解析请求

（递归请求）

1.  运营商的**DNS服务器首先查找自身的缓存**，如果能找到且没有过期则解析成功。

2.  如果没有找到，则运营商的DNS代我们的浏览器发起**迭代DNS解析请求**。

3.  **运营商DNS**首先会查找根域**DNS的IP地址**（**这个DNS服务器内置13台根DNS域服务器的IP地址**），找到根域的DNS地址，就会向其发起请求（（问一下www.abc.com这个域名的ip地址是多少啊？））。根域发现这是一个com域（顶级域）的域名，于是返回**com**域的**IP**地址，然后运营商的DNS就得到com域的IP地址。

4.  **运营商的DNS**得到com域的IP地址之后又向com域的IP地址发起地址请求（问一下www.abc.com这个域名的IP地址是多少啊？）。com域这台服务器告诉运营商的DNS我不知道www.abc.com这个域名的IP地址，但是我知道abc.com这个域名的**DNS**地址，你去找它吧。

5.  运营商的DNS又向abc.com这个域名的**DNS**地址发起请求，（问一下www.abc.com这个域名的IP地址是多少？）

6.  这个时候abc.com域的DNS服务器在本地查找。

7.  把找到的结果发给运营商的DNS服务器，这个时候运营商的DNS服务器就拿到了www.abc.com对应的IP地址，并返回给Windows系统内核，内核就把这个结果返回给浏览器， 终浏览器得到这个IP地址，进行下一步动作。

### TCP三次握手

客服端首先发送一个连接试探。

服务器监听到连接请求报文后，如果同意建立连接，则向Client发送确认。

Client收到确认后还需要再次发送确认，同时携带要发送给Server的数据。

### 为什么要三次握手？

- 验证服务端和客户端是否遵循TCP/IP协议 
- 为了防止已失效的连接请求报文段突然又传送到了服务端，因而产生错误。

###  为什么HTTP协议要基于TCP来实现？

TCP是一个端到端的可靠的面相连接的协议，HTTP基于传输层TCP协议不用担心数据传输的各种问题

（当发生错误时，会重传）

###  什么是面相连接协议？面向无链接协议又是什么？

**面相连接协议定义**

> 通信双方在通信时，要事先建立好一条通信线路（虚拟的）。其过程有**建立连接、维护连接、释放（断开）连接**三个过程。

TCP是面向连接的

> **面向无链接协议定义**与面向连接相对，面向无连接是指通信双方不需要事先建立通信线路，而是把每个带有目的地址的报文分组送到线路上，由系统自主选定线路进行传输。
>
> 面向无连接只有**"传送数据"**的过程。

UDP是面向无连接的

###  **说到三次握手，那在说下四次挥手吧？**

1. 客户端进程发出连接释放报文，并且停止发送数据。
2. 服务器收到连接释放报文，发出确认报文，此时，服务端就进入了CLOSE-WAIT（关闭等待）状态。(客户端向服务器方向释放了，但是服务器发送数据，客户端依然要接受)
3. 客户端收到服务器的确认请求后，客户端就进入FIN-WAIT-2（终止等待2）状态，等待服务器发送连接释放报文（在这之前还需要接受服务器发送的 后的数据）。
4. 服务器将 后的数据发送完毕后，就向客户端发送连接释放报文，服务器就进入了LAST-ACK（后确认）状态，等待客户端的确认。
5. 客户端收到服务器的连接释放报文后，必须发出确认，客户端就进入了TIME-WAIT（时间等待）状态。
6. 服务器只要收到了客户端发出的确认，立即进入CLOSED状态。同样，撤销TCB后，就结束了这次的TCP连接。**（服务器结束TCP连接的时间要比客户端早一些。）**



####  **为什么要四次挥手**

TCP协议是一种面向连接的、可靠的、基于字节流的运输层通信协议。TCP是全双工模式，这就意味着，当主机1发出FIN报文段时，只是表示主机1已经没有数据要发送了，主机1告诉主机2，它的数据已经全部发送完毕了；但是，这个时候主机1还是可以接受来自主机2的数据；当主机2返回ACK报文段时，表示它已经知道主机1没有数据发送了，但是主机2还是可以发送数据到主机1的；当主机2也发送了FIN 报文段时，这个时候就表示主机2也没有数据要发送了，就会告诉主机1，我也没有数据要发送了，之后彼此就会愉快的中断这次TCP连接。

#### **为什么建立连接是三次握手，关闭连接确是四次挥手呢？**

建立连接的时候， 服务器在LISTEN状态下，收到建立连接请求的SYN报文后，把ACK和SYN放在一个报文里发送给客户端。 而关闭连接时，服务器收到对方的FIN报文时，仅仅表示对方不再发送数据了但是还能接收数据，而自己也未必全部数据都发送给对方了，所以己方可以立即关闭，也可以发送一些数据给对方后，再发送FIN报文给对方来表示同意现在关闭连接，因此，己方ACK和FIN一般都会分开发送，从而导致多了一次。

###  **如果已经建立了连接，但是客户端突然出现故障了怎么办？**

TCP还设有一个保活计时器。但是客户端如果出现故障，服务器不能一直等下去，白白浪费资源。服务器每收到一次客户端的请求后都会重新复位这个计时器，时间通常是设置为2小时，若两小时还没有收到客户端的任何数据，服务器就会发送一个探测报文段，以后每隔75秒发送一次。若一连发送10个探测报文仍然没反应，服务器就认为客户端出了故障，接着就关闭连接。

###  **http请求方式有哪些？**

1.  GET：请求一个指定资源的表示形式. 使用GET的请求应该只被用于获取数据。

2.  HEAD：请求一个与GET请求的响应相同的响应，但没有响应体。

3.  POST：将实体提交到指定的资源。

4.  PUT：请求有效载荷替换目标资源的所有当前表示。

5.  DELETE：删除指定的资源。

6.  OPTIONS：用于描述目标资源的通信选项。

7.  PATCH：对资源应用部分修改。

8.  CONNECT：建立一个到由目标资源标识的服务器的隧道。

9.  TRACE：沿着到目标资源的路径执行一个消息环回测试。

## TCP和UDP的区别以及应用场景 

1. **UDP**

   1.  UDP在传输层上

   2.  是面向无连接的

   3.  不需要建立可靠的连接

   4.  是面向报文

   5.  限制就是发送一些比较小的包文件，而且没有错误处理机制。包没了就是没了。可以做一些处理，比如超时重发

   6.  一对一、一对多、多对一、多对多通信

   7.  适用于实时应用

2. **TCP**

   8.  TCP在传输层上

   9.  是TCP是面向连接的

   10.  可以互相信任的进行数据发送，这样的保密性强一些

   11.  面向字节流

   12.  一对一通信

   13.  适用于可靠传输的应用

3. **应用场景**

   | UDP              | TCP          |
   | ---------------- | ------------ |
   | app应用          | web browsing |
   | DNS查找          | email        |
   | 广播传输、流媒体 | 文件传输     |
   | 线上游戏         | 线上游戏     |

   

## tcp 中拥塞避免和流量控制机制 

> 拥塞避免和流量控制这两种机制很像，但是流量控制是由接收方的接受能力也就是接收窗口所决定的，如果接收窗口够大，以动态调整发送窗口的大小调整发送速度。
>
> 拥塞避免主要由网络情况所限制，网络情况良好，则加大发送速率，网络状态差（冗余 ACK 和丢包）则降低发送速率（慢启动，拥塞控制，快恢复，快重传） RENO，BBR。

## http和https 

HTTP：(HyperText Transfer Protocol)超文本传输协议

HTTPS：(Hypertext Transfer Protocol Secure)超文本传输安全协议

### **http和https的区别**

| -**名称/区别** | HTTP                                  | HTTPS                                     |
| -------------- | ------------------------------------- | ----------------------------------------- |
| 名称           | 超文本传输协议                        | 超文本传输安全协议                        |
| 默认端口       | 80                                    | 443                                       |
| 发送方式       | 明文发送                              | 加密传输                                  |
| 安全性         | 安全性相对差 容易被监听 被伪装 被篡改 | 安全性相对较好 防止监听 防止伪装 防止篡改 |
| 响应速度       | 响应快(3个包)                         | 响应慢(12个包) tcp 3个 ssl 9个            |
| 成本           | 较低                                  | 成本较高 证书需要购买                     |
| 链接缓存       | 相对高效                              | 相对不高 会增加数据开销和功耗             |

### https的访问过程（工作原理）

1.  客户使用https的URL访问Web服务器，要求与Web服务器建立SSL连接。

2.  Web服务器收到客户端请求后，会将网站的证书信息（证书中包含公钥）传送一份给客户端。

3.  客户端的浏览器与Web服务器开始协商SSL连接的安全等级，也就是信息加密的等级。

4.  客户端的浏览器根据双方同意的安全等级，建立会话密钥，然后利用网站的公钥将会话密钥加密，并传送给网站。

5.  Web服务器利用自己的私钥解密出会话密钥。

6.  Web服务器利用会话密钥加密与客户端之间的通信。



**详细解释：**

1.  客户端发起HTTPS请求

> 用户在浏览器里输入一个https网址，然后连接到server的443端口。

2.  服务端的配置

> 就是指上述提到的数字证书；

3.  传送证书

> Web服务器收到客户端请求后，会将网站的证书信息（证书中包含公钥）传送一份给客户端。

4.  客户端解析证书

> 客户端会对证书进行判断，验证公钥是否有效，存在问题弹出会警告；若没有问题，生成一个随机值
>
> （私钥），然后用证书继续进行加密；

5.  传送加密信息

> 客户端将上加密后的随机值（私钥）提供给服务端，服务端会对其进行解密；

6.  服务端解密信息

> 服务端解密后得到随机值（私钥），然后把内容通过该值进行对称加密。对称加密就是指把要返回的信息和随机值（私钥）混合加密，这样除非知道随机值（私钥），不然无法获取数据。

7.  传输加密后的信息

> 继续将加密后的信息传递给客户端；

8.  客户端解密信息

> 客户端用之前生成的私钥（随机值）解密服务端传过来的信息，于是获取了解密后的内容。

### https的优缺点？

**优点**

- 正确发送数据到客户端 

> 使用HTTPS协议可认证用户和服务器，确保数据发送到正确的客户机和服务器

- 更安全 

> HTTPS协议是由SSL+HTTP协议构建的可进行加密传输、身份认证的网络协议，要比http协议安全，可防止数据在传输过程中不被窃取、改变，确保数据的完整性

- 增加中间人攻击的成本

> HTTPS是现行架构下 安全的解决方案，虽然不是绝对安全，但它大幅增加了中间人攻击的成本。

- 搜索排名更高

> 谷歌在2014跳转搜索算法，采用HTTPS加密的网站在搜索结果中的排名将会更高
>
> 百度也在2018年发布百度对HTTPS站点的扶持态度，表明HTTPS将作为优质特征之一影响搜索排序。

**缺点**

1.  页面渲染更耗时间

> 因为SSL的缘故，HTTPS协议握手阶段比较费时，会使页面的加载时间延长近50%；

2.  成本增加

> SSL证书需要花钱，功能越强大的证书费用越高；

3.  HTTPS连接缓存不如HTTP高效

> HTTPS连接缓存不如HTTP高效，会增加数据开销和功耗，甚至已有的安全措施也会因此而受到影响；

4.  SSL证书通常需要绑定IP

> SSL证书通常需要绑定IP，不能在同一IP上绑定多个域名，IPv4资源不可能支撑这个消耗。

5.  有局限性

> HTTPS协议的加密范围也比较有限，在黑客攻击、拒绝服务攻击、服务器劫持等方面几乎起不到什么作用。 关键的，SSL证书的信用链体系并不安全，特别是在某些国家可以控制CA根证书的情况下，中间人攻击一样可行。

### **https如何进行性能优化？**

1.  **https访问速度优化**
    1.  设置HSTS

服务端返回一个 HSTS 的 http header，浏览器获取到 HSTS 头部之后，在一段时间内，不管用户输入www.baidu.com还是http://www.baidu.com，都会默认将请求内部跳转成 https://www.baidu.com。

2.  Session resume

3.  Nginx设置Ocsp stapling

OSCP Stapling 工作原理简单来说就是浏览器发起 Client Hello 时会携带一个 certificate status request 的扩展，服务端看到这个扩展后将 OCSP 内容直接返回给浏览器，完成证书状态检查。由于浏览器不需要直接向 CA 站点查询证书状态，这个功能对访问速度的提升非常明显。

4.  使用 SPDY 或者 HTTP2

> SPDY 大的特性就是多路复用，能将多个 HTTP 请求在同一个连接上一起发出去，不像目前的 HTTP 协议一样，只能串行地逐个发送请求。 HTTP2支持多路复用，有同样的效果。

5.  False start

简单概括 False Start 的原理就是在 client\_key\_exchange 发出时将应用层数据一起发出来，能够节省一个 RTT。

2. **https计算性能优化**

   优先使用 ECC椭圆加密算术。

> ECC 椭圆加密算术相比普通的离散对数计算速度性能要强很多。

​		使用 新版的 openssl。 

> 一般来讲，新版的 OpenSSL 相比老版的计算速度和安全性都会有提升。

​		硬件加速方案。

> SSL 专用加速卡。
>
> GPUSSL 加速。

​		TLS 远程代理计算

## 6. http/2 

1.  **http/2项目设定目标**

    1.  页面加载时间 (PLT) 减少 50%。

    2.  无需网站作者修改任何内容。

    3.  将部署复杂性降至 低，无需变更网络基础设施。

    4.  与开源社区合作开发此新协议。

    5.  收集真实性能数据，验证实验性协议是否有效。

2.  **http/2特性**

<!-- -->

1.  **二进制分帧层**

> HTTP/2 所有性能增强的核心在于新的二进制分帧层，它定义了如何封装 HTTP 消息并在客户端与服务器之间传输。

![](C:/Users/qiuxueyan/Desktop/blog/prepareInterview/media/image9.jpg){width="6.17995406824147in" height="3.2306681977252842in"}

2.  **多路复用(请求与响应复用)**

> HTTP/2 中新的二进制分帧层突破了这些限制，实现了完整的请求和响应复用：客户端和服务器可以将
>
> HTTP 消息分解为互不依赖的帧，然后交错发送， 后再在另一端把它们重新组装起来。

3.  **数据流优先级**

> 将 HTTP 消息分解为很多独立的帧之后，我们就可以复用多个数据流中的帧，客户端和服务器交错发送和传输这些帧的顺序就成为关键的性能决定因素。 为了做到这一点，HTTP/2 标准允许每个数据流都有一个关联的权重和依赖关系：
>
> 可以向每个数据流分配一个介于 1 至 256 之间的整数。每个数据流与其他数据流之间可以存在显式依赖关系。

4.  **每个来源一个连接**

> 每个数据流都拆分成很多帧，而这些帧可以交错，还可以分别设定优先级。 因此，所有 HTTP/2 连接都是永久的，而且仅需要每个来源一个连接，随之带来诸多性能优势。

5.  **流控制**

> 流控制是一种阻止发送方向接收方发送大量数据的机制，以免超出后者的需求或处理能力：发送方可能非常繁忙、处于较高的负载之下，也可能仅仅希望为特定数据流分配固定量的资源。

6.  **服务器推送**

> HTTP/2 新增的另一个强大的新功能是，服务器可以对一个客户端请求发送多个响应。 换句话说，除了对 初请求的响应外，服务器还可以向客户端推送额外资源，而无需客户端明确地请求。

7.  **标头压缩**

> 每个 HTTP 传输都承载一组标头，这些标头说明了传输的资源及其属性。
>
> HTTP/2 使用 HPACK 压缩格式压缩请求和响应标头元数据，这种格式采用两种简单但是强大的技术：
>
> 这种格式支持通过静态霍夫曼代码对传输的标头字段进行编码，从而减小了各个传输的大小。
>
> 这种格式要求客户端和服务器同时维护和更新一个包含之前见过的标头字段的索引列表（换句话说，它可以建立一个共享的压缩上下文），此列表随后会用作参考，对之前传输的值进行有效编码。

## 7. 说下http缓存吧 

1.  **什么是缓存？又有什么用？** 定义：缓存是一种保存资源副本并在下次请求时直接使用该副本的技术。

> 作用：

1.  可以显著提高网站和应用程序的性能。

2.  减少了等待时间和网络流量

3.  减少了显示资源表示形式所需的时间。

4.  是页面更加响应性。

5.  缓解服务器端压力，提升性能。

<!-- -->

2.  **你知道有哪些缓存方式吗？**

    6.  浏览器缓存

    7.  代理缓存

    8.  网关缓存

    9.  CDN缓存

    10.  反向代理缓存

3.  **缓存位置**

> Service Worker Memory Cache
>
> Disk Cache
>
> Push Cache

1.  **Service Worker**

> Service Worker 的缓存与浏览器其他内建的缓存机制不同，它可以让我们自由控制缓存哪些文件、如何匹配缓存、如何读取缓存，并且缓存是持续性的。

2.  **Memory Cache (内存中的缓存)**

> 读取高效，但是持续性很短，一旦关闭 Tab 页面，内存中的缓存也就被释放了。

3.  **Disk Cache (硬盘中的缓存)**

> 读取速度慢，容量和存储时效性上有优势，

4.  **Push Cache (推送缓存)**

> push Cache 是 http/2 中的内容，只在会话（Session）中存在，一旦会话结束就被释放，并且缓存时间也很短暂。

**4）http缓存怎样生效的？** http缓存分为强制缓存和协商缓存

1.  **强制缓存**

> 强制缓存就是文件直接从缓存中获取，不需要发送请求

2.  **协商缓存**

> 协商缓存意思是文件已经被缓存了，但是否从缓存中读取是需要和服务器进行协商，具体如何协商要看请求头/响应头的字段设置。

+--------------------------+-------------------------------------------------------------------------------------------------+
| > **指令名**             | **解释**                                                                                        |
+==========================+=================================================================================================+
| > public                 | 表明响应可以被任何对象（客户端，代理服务器，等等）缓存。                                        |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > private                | 表明响应只能被单个用户缓存，不能作为共享缓存（即代理服务器不能缓存它）。                        |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > no-cache               | 强制要求缓存把请求提交给原始服务器进行验证(协商缓存验证)。                                      |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > no-store               | 不使用任何缓存。                                                                                |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > max-age=               | 设置缓存存储的 大周期。                                                                         |
| >                        |                                                                                                 |
| > \<seconds\>            |                                                                                                 |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > s-maxage=              | 覆盖max-age或者Expires头，但是仅适用于共享缓存(比如各个代理)，私有缓存会忽略它。                |
| >                        |                                                                                                 |
| > \<seconds\>            |                                                                                                 |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > max-stale \[=          | 表示多少时间内，及时缓存过期也适用缓存                                                          |
| >                        |                                                                                                 |
| > \<seconds\>\]          |                                                                                                 |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > min-fresh= \<seconds\> | 表示在多少时间内获取 新的响应                                                                   |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > must-revalidate        | 一旦资源过期（比如已经超过max-age），在成功向原始服务器验证之前，缓存不能用该资源响应后续请求。 |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > proxy-revalidate       | 与must-revalidate作用相同，但它仅适用于共享缓存（例如代理），并被私有缓存忽略。                 |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > immutable              | 表示响应正文不会随时间而改变。                                                                  |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > no-transform           | 不得对资源进行转换或转变。                                                                      |
+--------------------------+-------------------------------------------------------------------------------------------------+
| > only-if-cached         | 客户端只接受已缓存的响应，并且不要向原始服务器检查是否有更新的拷贝。                            |
+--------------------------+-------------------------------------------------------------------------------------------------+

## 

![img](https://uploadfiles.nowcoder.com/images/20190313/311436_1552454253783_37390333D14B0305EB7C111457A68979)

## 45.csrf和xss的网络攻击及防范

 CSRF：跨站请求伪造，可以理解为攻击者盗用了用户的身份，以用户的名义发送了恶意请求，比如用户登录了一个网站后，立刻在另一个ｔａｂ页面访问量攻击者用来制造攻击的网站，这个网站要求访问刚刚登陆的网站，并发送了一个恶意请求，这时候CSRF就产生了，比如这个制造攻击的网站使用一张图片，但是这种图片的链接却是可以修改数据库的，这时候攻击者就可以以用户的名义操作这个数据库。

防御方式：使用验证码，检查https头部的refer，使用token

XSS：跨站脚本攻击，是说攻击者通过注入恶意的脚本，在用户浏览网页的时候进行攻击，比如获取cookie，或者其他用户身份信息，可以分为存储型和反射型，存储型是攻击者输入一些数据并且存储到了数据库中，其他浏览者看到的时候进行攻击，反射型的话不存储在数据库中，往往表现为将攻击代码放在url地址的请求参数中，防御的话为cookie设置httpOnly属性，对用户的输入进行检查，进行特殊字符过滤

XSS防御的总体思路是：对输入(和URL参数)进行过滤，对输出进行编码。也就是对提交的所有内容进行过滤，对url中的参数进行过滤，过滤掉会导致脚本执行的相关内容；然后对动态输出到页面的内容进行html编码，使脚本无法在浏览器中执行。虽然对输入过滤可以被绕过，但是也还是会拦截很大一部分的XSS攻击。

防御CSRF 攻击主要有三种策略：验证 HTTP Referer 字段；在请求地址中添加 token 并验证；在 HTTP 头中自定义属性并验证。

## 46.怎么看网站的性能如何

1. 检测页面加载时间一般有两种方式

   被动去测：就是在被检测的页面置入脚本或探针，当用户访问网页时，探针自动采集数据并传回数据库进行分析；

2. 主动监测的方式，即主动的搭建分布式受控环境，模拟用户发起页面访问请求，主动采集性能数据并分析，在检测的精准度上，专业的第三方工具效果更佳，比如说性能极客；

## 47.介绍HTTP协议(特征)

 

HTTP是一个基于TCP/IP通信协议来传递数据（HTML 文件, 图片文件, 查询结果等）HTTP是一个属于应用层的面向对象的协议，由于其简捷、快速的方式，适用于分布式超媒体信息系统。它于1990年提出，经过几年的使用与发展，得到不断地完善和扩展。目前在WWW中使用的是HTTP/1.0的第六版，HTTP/1.1的规范化工作正在进行之中，而且HTTP-NG(Next Generation of HTTP)的建议已经提出。HTTP协议工作于客户端服务端架构为上。浏览器作为HTTP客户端通过URL向HTTP服务端即WEB服务器发送所有请求。Web服务器根据接收到的请求后，向客户端发送响应信息。

## 48.说一下对Cookie和Session的认知，Cookie有哪些限制？

1. cookie数据存放在客户的浏览器上，session数据放在服务器上。
2. cookie不是很安全，别人可以分析存放在本地的COOKIE并进行COOKIE欺骗考虑到安全应当使用session。
3. session会在一定时间内保存在服务器上。当访问增多，会比较占用你服务器的性能考虑到减轻服务器性能方面，应当使用COOKIE。
4. 单个cookie保存的数据不能超过4K，很多浏览器都限制一个站点最多保存20个cookie。

## 49.描述一下XSS和CRSF攻击？防御方法？

 

XSS, 即为（Cross Site Scripting）, 中文名为跨站脚本, 是发生在目标用户的浏览器层面上的，当渲染DOM树的过程成发生了不在预期内执行的JS代码时，就发生了XSS攻击。大多数XSS攻击的主要方式是嵌入一段远程或者第三方域上的JS代码。实际上是在目标网站的作用域下执行了这段js代码。

CSRF（Cross Site Request Forgery，跨站请求伪造），字面理解意思就是在别的站点伪造了一个请求。专业术语来说就是在受害者访问一个网站时，其 Cookie 还没有过期的情况下，攻击者伪造一个链接地址发送受害者并欺骗让其点击，从而形成 CSRF 攻击。

XSS防御的总体思路是：对输入(和URL参数)进行过滤，对输出进行编码。也就是对提交的所有内容进行过滤，对url中的参数进行过滤，过滤掉会导致脚本执行的相关内容；然后对动态输出到页面的内容进行html编码，使脚本无法在浏览器中执行。虽然对输入过滤可以被绕过，但是也还是会拦截很大一部分的XSS 攻击。

防御CSRF 攻击主要有三种策略：

(1)验证 HTTP Referer 字段；

(2)在请求地址中添加 token 并验证；

(3)在 HTTP 头中自定义属性并验证。

## 51.具体有哪些请求头是跟缓存相关

缓存分为两种：强缓存和协商缓存，根据响应的header内容来决定。

强缓存相关字段有expires，cache-control。如果cache-control与expires 同时存在的话，cache-control的优先级高于expires。协商缓存相关字段有Last-Modified/If-Modified-Since，Etag/If-None-Match

## 52.cookie和session的区别

1. cookie数据存放在客户的浏览器上，session数据放在服务器上。
2. cookie不是很安全，别人可以分析存放在本地的COOKIE并进行COOKIE欺骗考虑到安全应当使用session。
3. session会在一定时间内保存在服务器上。当访问增多，会比较占用你服务器的性能考虑到减轻服务器性能方面，应当使用COOKIE。

4. 单个cookie保存的数据不能超过4K，很多浏览器都限制一个站点最多保存20个cookie。

## 53.cookie有哪些字段可以设置

name字段为一个cookie的名称。

value字段为一个cookie的值。

domain字段为可以访问此cookie的域名。

非顶级域名，如二级域名或者三级域名，设置的cookie的domain只能为顶级域

名或者二级域名或者三级域名本身，不能设置其他二级域名的cookie，否则 cookie无法生成。

顶级域名只能设置domain为顶级域名，不能设置为二级域名或者三级域名，否则cookie无法生成。二级域名能读取设置了domain为顶级域名或者自身的cookie，不能读取其他二级域名domain的cookie。所以要想cookie在多个二级域名中共享，需要设置 domain为顶级域名，这样就可以在所有二级域名里面或者到这个cookie的值了。

顶级域名只能获取到domain设置为顶级域名的cookie，其他domain设置为二级域名的无法获取。

path字段为可以访问此cookie的页面路径。

比如domain是abc.com,path是/test，那么只有/test路径下的页面可以读取此cookie。

expires/Max-Age字段为此cookie超时时间。

若设置其值为一个时间，那么当到达此时间后，此cookie失效。不设置的话默认值是Session，意思是cookie会和session一起失效。当浏览器关闭(不是浏览器标签页，而是整个浏览器) 后，此cookie失效。

Size字段 此cookie大小。

http字段 cookie的httponly属性。若此属性为true，则只有在http请求头中会带有此cookie的信息，而不能通过document.cookie来访问此cookie。

secure 字段 设置是否只能通过https来传递此条cookie

## 54.cookie有哪些编码方式？

 

encodeURI（）



## 56.除了cookie，还有什么存储方式。说说cookie和 localStorage的区别

还有localStorage，sessionStorage，indexdDB等 cookie和localStorage的区别：

cookie数据始终在同源的http请求中携带(即使不需要)，即cookie在浏览器和服务器间来回传递

cookie数据还有路径（path）的概念，可以限制。cookie只属于某个路径下

存储大小限制也不同，cookie数据不能超过4K，同时因为每次http请求都会携带cookie，所以cookie只适合保存很小的数据，如回话标识。

localStorage虽然也有存储大小的限制，但是比cookie大得多，可以达到5M 或更大

localStorage始终有效，窗口或浏览器关闭也一直保存，因此用作持久数据； cookie只在设置的cookie过期时间之前一直有效，即使窗口和浏览器关闭。





## get请求传参长度的误区

误区：我们经常说get请求参数的大小存在限制，而post请求的参数大小是无限制的。

实际上HTTP 协议从未规定 GET/POST 的请求长度限制是多少。对get请求参数的限制是来源与浏览器或web服务器，浏览器或web服务器限制了url的长度。

为了明确这个概念，我们必须再次强调下面几点:

HTTP 协议 未规定 GET 和POST的长度限制

GET的最大长度显示是因为 浏览器和 web服务器限制了 URI的长度

不同的浏览器和WEB服务器，限制的最大长度不一样

要支持IE，则最大长度为2083byte，若只支持Chrome，则最大长度 8182byte

## 补充get和post请求在缓存方面的区别

post/get的请求区别，具体不再赘述。

补充补充一个get和post在缓存方面的区别：

get请求类似于查找的过程，用户获取数据，可以不用每次都与数据库连接，所以可以使用缓存。

post不同，post做的一般是修改和删除的工作，所以必须与数据库交互，所以不能使用缓存。因此get请求适合于请求缓存。

## Cookie如何防范XSS攻击

XSS（跨站脚本攻击）是指攻击者在返回的HTML中嵌入javascript脚本，为了减轻这些攻击，需要在HTTP头部配上，set-cookie：

httponly-这个属性可以防止XSS,它会禁止javascript脚本来访问cookie。

secure - 这个属性告诉浏览器仅在请求为https的时候发送cookie。

结果应该是这样的：`Set-Cookie=<cookie-value>.....`

## Cookie和session的区别

> HTTP是一个无状态协议，因此Cookie的最大的作用就是存储sessionId用来唯一标识用户。

## 一句话概括RESTFUL

 

就是用URL定位资源，用HTTP描述操作

## cookie sessionStorage localStorage区别

 

cookie数据始终在同源的http请求中携带(即使不需要)，即cookie在浏览器和服务器间来回传递。

cookie数据还有路径（path）的概念，可以限制。cookie只属于某个路径下。存储大小限制也不同

cookie数据不能超过4K，同时因为每次http请求都会携带cookie，所以cookie 只适合保存很小的数据，如回话标识；

webStorage虽然也有存储大小的限制，但是比cookie大得多，可以达到5M或更大；

数据的有效期不同

sessionStorage：仅在当前的浏览器窗口关闭有效；

localStorage：始终有效，窗口或浏览器关闭也一直保存，因此用作持久数据； cookie：只在设置的cookie过期时间之前一直有效，即使窗口和浏览器关闭；作用域不同

sessionStorage：不在不同的浏览器窗口中共享，即使是同一个页面； localStorage：在所有同源窗口都是共享的； cookie：也是在所有同源窗口中共享的

## cookie session区别

 

(1)cookie数据存放在客户的浏览器上，session数据放在服务器上。

(2)cookie不是很安全，别人可以分析存放在本地的COOKIE并进行COOKIE欺骗

(3)考虑到安全应当使用session。

(4)session会在一定时间内保存在服务器上。当访问增多，会比较占用你服务器的性能，考虑到减轻服务器性能方面，应当使用COOKIE。

(5)单个cookie保存的数据不能超过4K，很多浏览器都限制一个站点最多保存20个cookie。

## 介绍知道的http返回的状态码 todo





## 强缓存、协商缓存什么时候用哪个

 

因为服务器上的资源不是一直固定不变的，大多数情况下它会更新，这个时候如果我们还访问本地缓存，那么对用户来说，那就相当于资源没有更新，用户看到的还是旧的资源；所以我们希望服务器上的资源更新了浏览器就请求新的资源，没有更新就使用本地的缓存，以最大程度的减少因网络请求而产生的资源浪费。

## TCP和UDP的区别

- TCP是面向连接的，udp是无连接的即发送数据前不需要先建立链接。

2. TCP提供可靠的服务。也就是说，通过TCP连接传送的数据，无差错，不丢失，不重复，且按序到达;UDP尽最大努力交付，即不保证可靠交付。 并且因为tcp可靠，面向连接，不会丢失数据因此适合大数据量的交换。
3. TCP是面向字节流，UDP面向报文，并且网络出现拥塞不会使得发送速率降低（因此会出现丢包，对实时的应用比如IP电话和视频会议等）。

4. TCP只能是1对1的，UDP支持1对1,1对多。
5. TCP的首部较大为20字节，而UDP只有8字节。

- TCP是面向连接的可靠性传输，而UDP是不可靠的。

## WebSocket的实现和应用

### (1)什么是WebSocket?

WebSocket是HTML5中的协议，支持持久连续，http协议不支持持久性连接。 Http1.0和HTTP1.1都不支持持久性的链接，HTTP1.1中的keep-alive，将多个http请求合并为1个；

### (2)WebSocket是什么样的协议，具体有什么优点？

HTTP的生命周期通过Request来界定，也就是Request一个Response，那么在 Http1.0协议中，这次Http请求就结束了。

在Http1.1中进行了改进，是的有一个connection：Keep-alive，也就是说，在一个Http连接中，可以发送多个Request，接收多个Response。但是必须记住，在Http中一个Request只能对应有一个Response，而且这个Response是

被动的，不能主动发起。

WebSocket是基于Http协议的，或者说借用了Http协议来完成一部分握手，在握手阶段与Http是相同的。我们来看一个websocket握手协议的实现，基本是2个属性，upgrade，connection。

基本请求如下：

GET /chat HTTP/1.1

Host: server.example.com

Upgrade: websocket

Connection: Upgrade

Sec-WebSocket-Key: x3JJHMbDL1EzLkh9GBhXDw==

Sec-WebSocket-Protocol: chat, superchat

Sec-WebSocket-Version: 13 Origin: http://example.com

多了下面2个属性：

Upgrade:webSocket

Connection:Upgrade

告诉服务器发送的是websocket

Sec-WebSocket-Key: x3JJHMbDL1EzLkh9GBhXDw==

Sec-WebSocket-Protocol: chat, superchat

Sec-WebSocket-Version: 13

## HTTP请求的方式，HEAD方式

  head：类似于get请求，只不过返回的响应中没有具体的内容，用户获取报头 options：允许客户端查看服务器的性能，比如说服务器支持的请求方式等等。

## 一个图片url访问后直接下载怎样实现？

 请求的返回头里面，用于浏览器解析的重要参数就是OSS的API文档里面的返回 http头，决定用户下载行为的参数。

下载的情况下：

1）x-oss-object-type:

Normal

2）x-oss-request-id: 598D5ED34F29D01FE2925F41

3）x-oss-storage-class:

Standard

## 说一下web Quality（无障碍）

 能够被残障人士使用的网站才能称得上一个易用的（易访问的）网站。残障人士指的是那些带有残疾或者身体不健康的用户。使用alt属性：

有时候浏览器会无法显示图像。具体的原因有：

a.用户关闭了图像显示

b.浏览器是不支持图形显示的迷你浏览器

c.浏览器是语音浏览器（供盲人和弱视人群使用）如果您使用了alt 属性，那么浏览器至少可以显示或读出有关图像的描述。

## TCP建立连接的三次握手过程

 

第一次握手：起初两端都处于CLOSED关闭状态，Client将标志位SYN置为1，随机产生一个值seq=x，并将该数据包发送给Server，Client进入SYN-SENT状态，等待Server确认；

第二次握手：Server收到数据包后由标志位SYN=1得知Client请求建立连接， Server将标志位SYN和ACK都置为1，ack=x+1，随机产生一个值seq=y，并将该数据包发送给Client以确认连接请求，Server进入SYN-RCVD状态，此时操作系统为该TCP连接分配TCP缓存和变量；

第三次握手：Client收到确认后，检查ack是否为x+1，ACK是否为1，如果正确则将标志位ACK置为1，ack=y+1，并且此时操作系统为该TCP连接分配TCP 缓存和变量，并将该数据包发送给Server，Server检查ack是否为y+1，ACK 是否为1，如果正确则连接建立成功，Client和Server进入ESTABLISHED状态，完成三次握手，随后Client和Server就可以开始传输数据。

## cdn原理 

CDN的全称是Content Delivery Network，即内容分发网络。CDN的基本原理是广泛采用各种缓存服务器，将这些缓存服务器分布到用户访问相对集中的地区或网络中，在用户访问网站时，利用全局负载技术将用户的访问指向距离最近的工作正常的缓存服务器上，由缓存服务器直接响

## HTTP的头部包含哪些内容。常见的请求方法

常见的请求方法有get,post，get用来请求数据，post用来提交数据，form表单使用get时数据会以querystring形式存在url中，因而不够安全也存在数据大小限制，而post不会，post将数据存放在http报文体中，获取数据应该用 get，提交数据用post

## 请求方法head特性

 

Head只请求页面的首部，head方法和get方法相同，只不过服务器响应时不会返回消息体，一个head请求的响应中，http头中包含的元信息应该和一个get 请求的响应消息相同，这种方法可以用来获取请求中隐含的元信息，而不用传输实体本身，这个也经常用来测试超链接的有效性和可用性，

Head请求有以下特点：只请求资源的首部，检查超链接的有效性检查网页是否被修改

用于自动搜索机器人获取网页的标志信息，获取rss种子信息，或者传递安全认证信息等

## HTTP状态码，301和302有什么具体区别，200和304 的区别

 

状态码可以按照第一个数字分类：

1表示信息，2表示成功，3表示重定向，4表示客户端错误，5表示服务器错误常见的状态码有：

101切换协议，200成功，301永久重定向，302临时重定向，304未修改

301和302的区别：

301：永久移动，请求的网页已永久移动到新的位置，服务器返回此响应，会自动将请求者转到新位置；

302：历史移动，服务器目前从不同位置的网页响应请求，但请求者应继续使用原有位置来继续以后的请求；

200和304：

200表示成功，服务器已成功处理了请求，通常表示为服务器提供了请求的网页；

304表示未修改，自从上次请求后，请求的网页未修改过，服务器返回此响应时不会返回网页内容；

## 6.OSI七层模型

>  
>
> osi七层模型可以说是面试必考基础了
>
> 从上到下分别是：
>
> 应用层：文件传输，常用协议HTTP，snmp,FTP , 表示层：数据格式化，代码转换，数据加密，会话层：建立，解除会话
>
> 传输层：提供端对端的接口，tcp,udp 网络层：为数据包选择路由，IP，icmp 数据链路层：传输有地址的帧物理层：二进制的数据形式在物理媒体上传输数据

## 7.TCP和UDP的区别，为什么三次握手四次挥手

>  
>
> TCP和UDP之间的区别：
>
> OSI 和TCP/IP 模型在传输层定义两种传输协议：TCP（或传输控制协议）和UDP （或用户数据报协议）。UDP 与TCP 的主要区别在于UDP 不一定提供可靠的数据传输。 事实上，该协议不能保证数据准确无误地到达目的地。
>
> 为什么TCP要进行四次挥手呢？
>
> 因为是双方彼此都建立了连接，因此双方都要释放自己的连接，A向B发出一个释放连接请求，他要释放链接表明不再向B发送数据了，此时B收到了A发送的释放链接请求之后，给A发送一个确认，A不能再向B发送数据了，它处于 FIN-WAIT-2的状态，但是此时B还可以向A进行数据的传送。此时B向A 发送一个断开连接的请求，A收到之后给B发送一个确认。此时B关闭连接。A也关闭连接。
>
> 为什么要有TIME-WAIT这个状态呢，这是因为有可能最后一次确认丢失，如果B 此时继续向A发送一个我要断开连接的请求等待A发送确认，但此时A已经关闭连接了，那么B永远也关不掉了，所以我们要有TIME-WAIT这个状态。
>
> 当然TCP也并不是100%可靠的。

## 8.HTTP缓存机制

>  
>
> HTTP缓存即是浏览器第一次想一个服务器发起HTTP请求后，服务器会返回请求的资源，并且在响应头中添加一些有关缓存的字段如：cache-control， expires,last-modifed，ETag,Date，等，之后浏览器再向该服务器请求资源就可以视情况使用强缓存和协商缓存，
>
> 强缓存：浏览器直接从本地缓存中获取数据，不与服务器进行交互，协商缓存：浏览器发送请求到服务器，服务器判断是否可使用本地缓存
>
> ![](media/image17.jpg){width="6.27in" height="4.331666666666667in"}

## 9.websocket和ajax的区别是什么，websocket的应用场景有哪些

>  
>
> WebSocket的诞生本质上就是为了解决HTTP协议本身的单向性问题：请求必须由客户端向服务端发起，然后服务端进行响应。这个Request-Response的关系是无法改变的。对于一般的网页浏览和访问当然没问题，一旦我们需要服务端主动向客户端发送消息时就麻烦了，因为此前的TCP连接已经释放，根本找不到客户端在哪。
>
> 为了能及时从服务器获取数据，程序员们煞费苦心研究出来的各种解决方案其实都是在HTTP框架下做的妥协，没法子，浏览器这东西只支持HTTP，我们有什么办法。所以大家要么定时去轮询，要么就靠长连接------客户端发起请求，服务端把这个连接攥在手里不回复，等有消息了再回，如果超时了客户端就再请求一次
>
> ------其实大家也懂，这只是个减少了请求次数、实时性更好的轮询，本质没变。 WebSocket就是从技术根本上解决这个问题的：看名字就知道，它借用了Web的端口和消息头来创建连接，后续的数据传输又和基于TCP的Socket几乎完全一样，但封装了好多原本在Socket开发时需要我们手动去做的功能。比如原生支持wss安全访问（跟https共用端口和证书）、创建连接时的校验、从数据帧中自动拆分消息包等等。
>
> 换句话说，原本我们在浏览器里只能使用HTTP协议，现在有了Socket，还是个更好用的Socket。
>
> 了解了WebSocket的背景和特性之后，就可以回答它能不能取代AJAX这个问题了：
>
> 对于服务器与客户端的双向通信，WebSocket简直是不二之选。如果不是还有少数旧版浏览器尚在服役的话，所有的轮询、长连接等方式早就该废弃掉。那些整合多种双向推送消息方式的库（如http://Socket.IO、SignalR）当初最大的卖点就是兼容所有浏览器版本，自动识别旧版浏览器并采取不同的连接方式，现在也渐渐失去了优势------所有新版浏览器都兼容WebSocket，直接用原生的就行了。
>
> 说句题外话，这点很像jQuery，在原生js难用时迅速崛起，当其他库和原生js 都吸收了它的很多优势时，慢慢就不那么重要了。
>
> 但是，很大一部分AJAX的使用场景仍然是传统的请求-响应形式，比如获取json 数据、post表单之类。这些功能虽然靠WebSocket也能实现，但就像在原本传输数据流的TCP之上定义了基于请求的HTTP协议一样，我们也要在WebSocket 之上重新定义一种新的协议，最少也要加个request id用来区分每次响应数据对应的请求吧。
>
> ......但是，何苦一层叠一层地造个新轮子呢？直接使用AJAX不是更简单、更成熟吗？
>
> 另外还有一种情况，也就是传输大文件、图片、媒体流的时候，最好还是老老实实用HTTP来传。如果一定要用WebSocket的话，至少也专门为这些数据专门开辟个新通道，而别去占用那条用于推送消息、对实时性要求很强的连接。否则会把串行的WebSocket彻底堵死的。
>
> 所以说，WebSocket在用于双向传输、推送消息方面能够做到灵活、简便、高效，但在普通的Request-Response过程中并没有太大用武之地，比起普通的HTTP 请求来反倒麻烦了许多，甚至更为低效。
>
> 每项技术都有自身的优缺点，在适合它的地方能发挥出最大长处，而看到它的几个优点就不分场合地全方位推广的话，可能会适得其反。
>
> 我们自己在开发能与手机通信的互联网机器人时就使用了WebSocket，效果很好。但并不是用它取代HTTP，而是取代了原先用于通信的基于TCP的Socket。
>
> 优点是：
>
> 原先在Socket连接后还要进行一些复杂的身份验证，同时要阻止未验证的连接发送控制指令。现在不需要了，在建立WebSocket连接的url里就能携带身份验证参数，验证不通过可以直接拒绝，不用设置状态；
>
> 原先自己实现了一套类似SSL的非对称加密机制，现在完全不需要了，直接通过 wss加密，还能顺便保证证书的可信性；
>
> 原先要自己定义Socket数据格式，设置长度与标志，处理粘包、分包等问题，现在WebSocket收到的直接就是完整的数据包，完全不用自己处理；
>
> 前端的nginx可以直接进行转发与负载均衡，部署简单多了

## 10.TCP/IP的网络模型

>  
>
> TCP/IP模型是一系列网络协议的总称，这些协议的目的是使得计算机之间可以进行信息交换，
>
> TCP/IP模型四层架构从下到上分别是链路层，网络层，传输层，应用层
>
> 链路层的作用是负责建立电路连接，是整个网络的物理基础，典型的协议包括以太网，ADSL等，
>
> 网络层负责分配地址和传送二进制数据，主要协议是IP协议，传输层负责传送文本数据，主要协议是TCP
>
> 应用层负责传送各种最终形态的数据，是直接与用户信息打交道的层，主要协议是http，ftp等

## 11.知道什么跨域方式吗，jsonp具体流程是什么，如何实现原生Jsonp封装，优化，对于CORS，服务器怎么判断它该不该跨域呢

>  
>
> 常见的跨域方式大概有七种，大致可分为iframe、api跨域

1. JSONP，全称为json with padding，解决老版本浏览器跨域数据访问问题，原理是web页面调用JS文件不受浏览器同源策略限制，所以通过script标签可以进行跨域请求，流程如下：

> 首先前端设置好回调参数，并将其作为URL的参数
>
> 服务器端收到请求后，通过该参数获取到回调函数名，并将数据放在参数中返回收到结果后因为是script标签，所以浏览器当做脚本运行，

1. cors，全称是跨域资源共享，允许浏览器向跨源服务器发出XMLHTTPRequest 请求，从而克服了ajax只能同源使用的策略，实现cors的关键是服务器，只要服务器实现了cros接口，就可以跨域通信

> 前端逻辑很简单，正常发起 ajax 请求即可，成功的关键在于服务器 Access-Control-Allow-Origin 是否包含请求页面的域名，如果不包含的话，浏览器将认为这是一次失败的异步请求，将会调用 xhr.onerror 中的函数。
>
> Cros使用简单，支持POST方式，但是存在兼容问题
>
> 浏览器将cors请求分为两类，简单请求和非简单请求，对于简单请求，浏览器直接发出cors请求，就是在头信息之中增加一个origin字段，用于说明本次请求来自哪个协议+域名+端口，服务器根据这个值，决定是否同意本次请求，如果
>
> 服务器同意本次请求，返回的响应中会多出几个头信息字段：
>
> Access-Control-Allow-Orign：返回origin的字段或者*
>
> Access-Control-Allow-Credentials,该字段可选，是一个bool值，表示是否允许发送cookie，
>
> Access-Control-Expose-Headers
>
> 3）服务器代理：
>
> 即当你有跨域的请求操作时发给后端，让后端帮你代为请求，此外还有四中不常用的方式，也可了解下： location.hash：
>
> Window.name postMessage

## 12.怎么生成token，怎么传递

>  
>
> 接口特点汇总：

1. 因为是非开放性的，所以所有的接口都是封闭的，只对公司内部的产品有效；
2. 因为是非开放性的，所以OAuth那套协议是行不通的，因为没有中间用户的授权过程；
3. 有点接口需要用户登录才能访问；
4. 有点接口不需要用户登录就可访问；

> 针对以上特点，移动端与服务端的通信就需要2把钥匙，即2个token。
>
> 第一个token是针对接口的（api_token）；第二个token是针对用户的（user_token）；先说第一个token（api_token）
>
> 它的职责是保持接口访问的隐蔽性和有效性，保证接口只能给自家人用，怎么做到？参考思路如下：
>
> 现在的接口基本是mvc模式，URL基本是restful风格，URL大体格式如下：
>
> http://blog.snsgou.com/模块名/控制器名/方法名?参数名1=参数值1&参数名
>
> 2=参数值2&参数名3=参数值3
>
> 接口token生成规则参考如下：
>
> api_token = md5 ('模块名' + '控制器名' + '方法名' + '2017-07-18' + '
>
> 加密密钥') = 770fed4ca2aabd20ae9a5dd774711de2
>
> 其中的

1. '2013-12-18' 为当天时间，
2. '加密密钥' 为私有的加密密钥，手机端需要在服务端注册一个"接口使用者" 账号后，系统会分配一个账号及密码，数据表设计参考如下：

> ![](media/image18.jpg){width="5.7716666666666665in" height="1.8831594488188976in"}
>
> <?php
>
> 1）获取GET参数值
>
> $module = $_GET['mod'];
>
> $controller = $_GET['ctl'];
>
> $action = $_GET['act'];
>
> $client_id = $_GET['client_id'];
>
> $api_token = $_GET['api_token']; 2）根据客户端传过来的client_id，查询数据库，获取对应的client_secret。
>
> $client_secret = getclientSecretById($client_id);

1. 服务器重新生成一份api_token

> $api_token_server = md5($module.$controller.$action.date('Y-m-d', time()).$client_secret);

1. 客户端传过来的api_token与服务器生成的api_token进行校对，如果不相

> 等，则表示验证失败。
>
> if($api_token != $api_token_server){ exit('access deny');
>
> }

1. 验证通过，返回数据到客户端。

> 再说第二个token（user_token），它的职责是保护用户的用户名及密码多次提
>
> 交，以防密码泄露。
>
> 如果接口需要用户登录，其访问流程如下：
>
> 1）用户提交"用户名"和"密码"，实现登录（条件允许，这一步最好走https）； 2）登录成功后，服务端返回一个 user_token，生成规则参考如下：
>
> 服务端用数据表维护user_token的状态，表设计如下：
>
> ![](media/image19.jpg){width="5.7716666666666665in" height="2.125in"}
>
> 服务端生成user_token 后，返回给客户端（自己存储），客户端每次接口请求时，如果接口需要用户登录才能访问，则需要把 user_id 与 user_token 传回给服务端，服务端接受到这2个参数后，需要做以下几步：

1. 检测 api_token的有效性；
2. 删除过期的 user_token 表记录；
3. 根据 user_id，user_token 获取表记录，如果表记录不存在，直接返回错误，如果记录存在，则进行下一步；
4. 更新 user_token 的过期时间（延期，保证其有效期内连续操作不掉线）；
5. 返回接口数据。

> 那么token如何传递呢，ajax中传递token有以下几种方式：
>
> （1）放在请求头中：
>
> ![](media/image20.jpg){width="5.0633333333333335in" height="0.9583333333333334in"}
>
> ![](media/image21.jpg){width="5.791666666666667in" height="1.057688101487314in"}

## 13.操作系统进程和线程的区别

>  
>
> 进程，是并发执行的程序在执行过程中分配和管理资源的基本单位，是一个动态概念，竞争计算机系统资源的基本单位。
>
> 线程，是进程的一部分，一个没有线程的进程可以被看作是单线程的。线程有时又被称为轻权进程或轻量级进程，也是 CPU 调度的一个基本单位。

## 14.什么是进程 线程

>  
>
> 进程，是并发执行的程序在执行过程中分配和管理资源的基本单位，是一个动态概念，竞争计算机系统资源的基本单位。
>
> 线程，是进程的一部分，一个没有线程的进程可以被看作是单线程的。线程有时又被称为轻权进程或轻量级进程，也是 CPU 调度的一个基本单位。

## 15.线程的那些资源共享，那些资源不共享

>  共享的资源有
>
> a.堆由于堆是在进程空间中开辟出来的，所以它是理所当然地被共享的；因此 new出来的都是共享的（16位平台上分全局堆和局部堆，局部堆是独享的）

b.  全局变量 它是与具体某一函数无关的，所以也与特定线程无关；因此也是共享的

c.  静态变量虽然对于局部变量来说，它在代码中是"放"在某一函数中的，但是其存放位置和全局变量一样，存于堆中开辟的.bss和.data段，是共享的

d.  文件等公用资源 这个是共享的，使用这些公共资源的线程必须同步。Win32 提供了几种同步资源的方式，包括信号、临界区、事件和互斥体。

> 独享的资源有：

a.  栈 栈是独享的

b.  寄存器 这个可能会误解，因为电脑的寄存器是物理的，每个线程去取值难道不一样吗？其实线程里存放的是副本，包括程序计数器PC

## 16.操作系统里面进程和线程的区别

>  
>
> 进程是具有一定独立功能的程序，他是系统进行资源分配调度的一个独立单位，线程是进程的一个实体，是cpu调度分派的基本单位，线程之间基本上不拥有系统资源
>
> 一个程序至少有一个进程，一个进程至少有一个线程，资源分配给进程，同一个进程下所有线程共享该进程的资源

## 17.Linux查询进程指令，查询端口，杀进程

>  查询进程： ps 命令用于查看当前正在运行的进程。
>
> grep 是搜索
>
> 例如： ps -ef | grep java
>
> 表示查看所有进程里CMD是java的进程信息 ps -aux | grep java
>
> -aux 显示所有状态 ps
>
> 杀死进程：
>
> kill -9[PID]

## 18.进程间的通信方式有哪些？

>  总共有八种，面试中只要能大概答上三四种方式的原理就可以了

(1)无名管道：半双工的通信方式，数据只能单向流动且只能在具有亲缘关系的进程间使用

(2)高级管道：将另一个程序当作一个新的进程在当前程序进程中启动，则这个进程算是当前程序的子进程，

> (3)有名管道，：也是半双工的通信方式，但是允许没有亲缘进程之间的通信

(4)消息队列：消息队列是有消息的链表，存放在内核中，并由消息队列标识符标识，消息队列克服了信号传递信息少，管道只能承载无格式字节流以及缓冲区大小受限的缺点

(5)信号量：信号量是一个计数器，可以用来控制多个进程对共享资源的访问，它常作为一种锁机制，防止某进程正在访问共享资源时，其他进程也访问该资源，

> (6)信号：用于通知接受进程某个事件已经发生
>
> (7)共享内存：共享内存就是映射一段能被其他进程所访问的内存。这段共享内
>
> 存由一个进程创建，但是多个进程可以访问，共享内存是最快的IPC 方式，往往与其他通信机制配合使用
>
> (8)套接字：可用于不同机器之间的进程通信

## 19.Redis和 mysql

>  

1. 类型上

> 从类型上来说，mysql是关系型数据库，redis是缓存数据库

1. 作用上

> mysql用于持久化的存储数据到硬盘，功能强大，但是速度较慢 redis用于存储使用较为频繁的数据到缓存中，读取速度快

1. 需求上

> mysql和redis因为需求的不同，一般都是配合使用。

# 第八章 手写代码

## 排序算法

![img](https://images2018.cnblogs.com/blog/849589/201804/849589-20180402133438219-1946132192.png)

### 冒泡排序

- 比较相邻的元素。如果第一个比第二个大，就交换它们两个；
- 对每一对相邻元素作同样的工作，从开始第一对到结尾的最后一对，这样在最后的元素应该会是最大的数；
- 针对所有的元素重复以上的步骤，除了最后一个；
- 重复步骤1~3，直到排序完成。

```js
function bubbleSort(arr){
    var len = arr.length;
    for (var i =0;i<len;i++){
        for(var j=0;j<len-1-i;j++){
            if(arr[j]>arr[j+1]){
                var temp = arr[j];
                arr[j] = arr[j+1]
                arr[j+1] = temp;
            }
        }
    }
    return arr;
}
```

### 选择排序

首先在未排序序列中找到最小（大）元素，存放到排序序列的起始位置，然后，再从剩余未排序元素中继续寻找最小（大）元素，然后放到已排序序列的末尾。以此类推，直到所有元素均排序完毕。 

- 初始状态：无序区为R[1..n]，有序区为空；
- 第i趟排序(i=1,2,3…n-1)开始时，当前有序区和无序区分别为R[1..i-1]和R(i..n）。该趟排序从当前无序区中-选出关键字最小的记录 R[k]，将它与无序区的第1个记录R交换，使R[1..i]和R[i+1..n)分别变为记录个数增加1个的新有序区和记录个数减少1个的新无序区；
- n-1趟结束，数组有序化了

```js
function selectSort(arr){
    var len = arr.length;
    for (var i =0;i<len;i++){
        var minIndex = i;
        for (var j=i+1;j<len;j++){
            if(arr[j]< arr[minIndex]){
                minIndex = j;
            }
        }
        [arr[minIndex],arr[i]] = [arr[i],arr[minIndex]];
    }
    return arr;
}
```

### 插入排序

通过构建有序序列，对于未排序数据，在已排序序列中从后向前扫描，找到相应位置并插入。

- 从第一个元素开始，该元素可以认为已经被排序；
- 取出下一个元素，在已经排序的元素序列中从后向前扫描；
- 如果该元素（已排序）大于新元素，将该元素移到下一位置；
- 重复步骤3，直到找到已排序的元素小于或者等于新元素的位置；
- 将新元素插入到该位置后；
- 重复步骤2~5。

```js
function insertionSort(arr) {
    var len = arr.length;
    var preIndex, current;
    for(var i = 1; i < len; i++) {
        preIndex = i - 1;
        current = arr[i];
        while(preIndex >= 0 && arr[preIndex] > current) {
            arr[preIndex + 1] = arr[preIndex];
            preIndex--;
        }
        arr[preIndex + 1] = current;
    }
    return arr;
}
```

### 希尔排序

先将整个待排序的记录序列分割成为若干子序列分别进行直接插入排序

- 选择一个增量序列t1，t2，…，tk，其中ti>tj，tk=1；
- 按增量序列个数k，对序列进行k 趟排序；
- 每趟排序，根据对应的增量ti，将待排序列分割成若干长度为m 的子序列，分别对各子表进行直接插入排序。仅增量因子为1 时，整个序列作为一个表来处理，表长度即为整个序列的长度。

```js
function shellSort(arr) {
    var len = arr.length;
    for (var  gap = Math.floor(len/2);gap>0;gap = Math.floor(gap/2)){//分组
        for (var i = gap;i<len;i++){
            var j=i;
            var current = arr[i];
            while(j-gap>=0&&current < arr[j - gap]){
                arr[j] = arr[j-gap];
                j=j-gap;
            }
            arr[j] = current;
            console.log(arr)
        }
    }
    
    return arr;
}
```

### 归并排序

归并排序是建立在归并操作上的一种有效的排序算法。该算法是采用分治法（Divide and Conquer）的一个非常典型的应用。将已有序的子序列合并，得到完全有序的序列；即先使每个子序列有序，再使子序列段间有序。若将两个有序表合并成一个有序表，称为2-路归并。 

- 把长度为n的输入序列分成两个长度为n/2的子序列；
- 对这两个子序列分别采用归并排序；
- 将两个排序好的子序列合并成一个最终的排序序列。

```js
function mergeSort(arr) {
    var len = arr.length;
    if (len  < 2){
        return arr;
    }
    //分组
    var middle = Math.floor(len / 2),left = arr.slice(0,middle),right = arr.slice(middle);
    //合并
    return merge(mergeSort(left),mergeSort(right));
}
function merge(left,right){
    var res = [];
    while(left.length>0 && right.length>0){
        if(left[0]<=right[0]){
            res.push(left.shift());
        }else{
            res.push(right.shift())
        }
    }
    while(left.length){
        res.push(left.shift())
    }
    while(right.length){
        res.push(right.shift())
    }
    return res;
    
}
```

### 快速排序

通过一趟排序将待排记录分隔成独立的两部分，其中一部分记录的关键字均比另一部分的关键字小，则可分别对这两部分记录继续进行排序，以达到整个序列有序。 

- 从数列中挑出一个元素，称为 “基准”（pivot）；
- 重新排序数列，所有元素比基准值小的摆放在基准前面，所有元素比基准值大的摆在基准的后面（相同的数可以到任一边）。在这个分区退出之后，该基准就处于数列的中间位置。这个称为分区（partition）操作；
- 递归地（recursive）把小于基准值元素的子数列和大于基准值元素的子数列排序。

```js
function swap(arr,i,j){
    let temp = arr[i];
    arr[i] =  arr[j]
    arr[j] = temp;
}
function quickSort(arr,left,right){
    var len = arr.length;
    var partitionIndex,
    left = typeof(left) !="number"?0:left;
    right = typeof(right) !="number"?left+1:right;

    if(left < right){
        partitionIndex = partition(arr,left,right);
        quickSort(arr,left,partitionIndex-1)
        quickSort(arr,partitionIndex+1,right)
    }
}
function partition(arr,left,right){
    var pivot = left;
    var index = pivot+1;
    for(var i=index;i<=right;i++){
        if(arr[i] < arr[pivot]){
            swap(arr,i,index);
            index++;
        }
    }
    swap(arr,pivot,index-1);
    return index-1;
}
```

### 堆排序

利用堆这种数据结构所设计的一种排序算法。堆积是一个近似完全二叉树的结构，并同时满足堆积的性质：即子结点的键值或索引总是小于（或者大于）它的父节点。

- 将初始待排序关键字序列(R1,R2….Rn)构建成大顶堆，此堆为初始的无序区；
- 将堆顶元素R[1]与最后一个元素R[n]交换，此时得到新的无序区(R1,R2,……Rn-1)和新的有序区(Rn),且满足R[1,2…n-1]<=R[n]；
- 由于交换后新的堆顶R[1]可能违反堆的性质，因此需要对当前无序区(R1,R2,……Rn-1)调整为新堆，然后再次将R[1]与无序区最后一个元素交换，得到新的无序区(R1, R2….Rn-2)和新的有序区(Rn-1,Rn)。不断重复此过程直到有序区的元素个数为n-1，则整个排序过程完成。

```js
var len;
//交换
function swap(arr,i,j){
    let temp = arr[i];
    arr[i] =  arr[j]
    arr[j] = temp;
}
//建堆
function buildMaxHeap(arr){
    len = arr.length;
    for(var i = Math.floor(len/2);i>=0;i--){
        heapify(arr,i);
    }
}
function heapify(arr,i){
    var left = 2*i+1,
        right = 2*i+2,
        largest = i;

    if(left < len && arr[left] > arr[largest]){
        largest = left;
    }
    if(right < len && arr[right] > arr[largest]){
        largest = right;
    }
    if(largest !=i){
        swap(arr,i,largest);
        heapify(arr,largest);
    }
}

function heapSort(arr){
    buildMaxHeap(arr);
    for(var i = arr.length-1;i>0;i--){
        swap(arr,0,i);//将堆顶与无序区最后一个元素交换
        len--;
        heapify(arr,0);
    }
    return arr;
}
```

### 计数排序

计数排序不是基于比较的排序算法，其核心在于将输入的数据值转化为键存储在额外开辟的数组空间中。 作为一种线性时间复杂度的排序，计数排序要求输入的数据**必须是有确定范围的整数**。

- 找出待排序的数组中最大和最小的元素；
- 统计数组中每个值为i的元素出现的次数，存入数组C的第i项；
- 对所有的计数累加（从C中的第一个元素开始，每一项和前一项相加）；
- 反向填充目标数组：将每个元素i放在新数组的第C(i)项，每放一个元素就将C(i)减去1。

```js
function countSort(arr,max){
    var bucket =new Array(max + 1),
        sortedIndex = 0;
        arrLen = arr.length,
        bucketLen = max + 1;
 
    for(var i = 0; i < arrLen; i++) {
        if(!bucket[arr[i]]) {
            bucket[arr[i]] = 0;
        }
        bucket[arr[i]]++;
    }
 
    for(var j = 0; j < bucketLen; j++) {
        while(bucket[j] > 0) {
            arr[sortedIndex++] = j;
            bucket[j]--;
        }
    }
 
    return arr;
}
function findMax(arr){
    var min = arr[0],max = arr[0];
    var len = arr.length;
    for(var i=0;i<len;i++){
        if(max<arr[i]){
            max = arr[i];
        }
    }
    return max;
}

var arr = [1,2,3,3,3];
var max = findMax(arr)
console.log(countSort(arr,max))
```

### 桶排序

桶排序是计数排序的升级版。它利用了函数的映射关系，高效与否的关键就在于这个映射函数的确定。桶排序 (Bucket sort)的工作的原理：假设输入数据服从均匀分布，将数据分到有限数量的桶里，每个桶再分别排序（有可能再使用别的排序算法或是以递归方式继续使用桶排序进行排）。

- 设置一个定量的数组当作空桶；
- 遍历输入数据，并且把数据一个一个放到对应的桶里去；
- 对每个不是空的桶进行排序；
- 从不是空的桶里把排好序的数据拼接起来。 

```js
function bucketSort(arr, bucketSize) {
    if(arr.length === 0) {
      return arr;
    }
 
    var i;
    var minValue = arr[0];
    var maxValue = arr[0];
    for(i = 1; i < arr.length; i++) {
      if(arr[i] < minValue) {
          minValue = arr[i];               // 输入数据的最小值
      }else if(arr[i] > maxValue) {
          maxValue = arr[i];               // 输入数据的最大值
      }
    }
 
    // 桶的初始化
    var DEFAULT_BUCKET_SIZE = 5;           // 设置桶的默认数量为5
    bucketSize = bucketSize || DEFAULT_BUCKET_SIZE;
    var bucketCount = Math.floor((maxValue - minValue) / bucketSize) + 1;  
    var buckets =new Array(bucketCount);
    for(i = 0; i < buckets.length; i++) {
        buckets[i] = [];
    }
 
    // 利用映射函数将数据分配到各个桶中
    for(i = 0; i < arr.length; i++) {
        buckets[Math.floor((arr[i] - minValue) / bucketSize)].push(arr[i]);
    }
 
    arr.length = 0;
    for(i = 0; i < buckets.length; i++) {
        insertionSort(buckets[i]);                     // 对每个桶进行排序，这里使用了插入排序
        for(varj = 0; j < buckets[i].length; j++) {
            arr.push(buckets[i][j]);                     
        }
    }
 
    return arr;
}

var arr = [1,2,3,3,3];
console.log(bucketSort(arr,4))
```



## 查找算法

### 二分查找

```js
function binarySearch(arr,x,left,right){
    if(left>right) return -1;
    left = left || 0;
    right = right || arr.length-1;
    let mid = parseInt((left+right)/2);
    console.log(mid)
    if(arr[mid] == x){
        return mid;
    }else if(arr[mid]<x){
        return binarySearch(arr,x,mid+1,right)
    }else if(arr[mid]>x){
        return binarySearch(arr,x,left,mid-1)
    }
    
    return -1;
}
```



## 二叉树层序遍历



## B树的特性，B树和B+树的区 

一个m 阶的B树满足以下条件：每个结点至多拥有m棵子树；

根结点至少拥有两颗子树（存在子树的情况下）；

除了根结点以外，其余每个分支结点至少拥有m/2 棵子树；所有的叶结点都在同一层上；

有k 棵子树的分支结点则存在 k-1 个关键码，关键码按照递增次序进行排列；关键字数量需要满足ceil(m/2)-1 <= n <= m-1；

B树和B+树的区别：以一个m阶树为例。

关键字的数量不同；B+树中分支结点有m个关键字，其叶子结点也有m个，其关键字只是起到了一个索引的作用，但是B树虽然也有m个子结点，但是其只拥有 m-1个关键字。

存储的位置不同；B+树中的数据都存储在叶子结点上，也就是其所有叶子结点的数据组合起来就是完整的数据，但是B树的数据存储在每一个结点中，并不仅仅存储在叶子结点上。

分支结点的构造不同；B+树的分支结点仅仅存储着关键字信息和儿子的指针（这里的指针指的是磁盘块的偏移量），也就是说内部结点仅仅包含着索引信息。

查询不同；B树在找到具体的数值以后，则结束，而B+树则需要通过索引找到叶子结点中的数据才结束，也就是说B+树的搜索过程中走了一条从根结点到叶子结点的路径。

## 尾递归

 如果一个函数中所有递归形式的调用都出现在函数的末尾，我们称这个递归函数是尾递归的。当递归调用是整个函数体中最后执行的语句且它的返回值不属于表达式的一部分时，这个递归调用就是尾递归。

## 如何写一个大数阶乘？递归的方法会出现什么问题？

```js
function factorial(n){
    return n > 1 ? n * factorial(n-1) : 1;
}出现数字过大
```



## 把多维数组变成一维数组的方法(数组扁平化)

```js
//双重循环
function flatten(arr){
    var res = [];
    for (var i=0;i<arr.length;i++){
        if (Array.isArray(arr[i])){
            res = res.concat(flatten(arr[i]));
        }else{
            res.push(arr[i]);
        }
    }
    return res;
}

//toString（）
function flatten2(arr){
    return arr.toString().split(',').map(function(item){ return +item })
}
function flatten3(arr){
    return arr.join(',').split(',').map(item=>parseInt(item));
}

//reduce
function flatten3(arr) {
     return arr.reduce(
    function(prev, next){
        return prev.concat(Array.isArray(next) ? flatten(next) : next)
    }, []) 
}

//some
function flatten4(arr) { 
    while (arr.some(item => Array.isArray(item))) { 
        arr = [].concat(...arr); 
    }
    return arr; 
}
var data =  [1, [2, [ [3, 4], 5], 6]];
// 5
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





## 数组的去重，尽可能写出多个方法

1. 双重循环
2. `indexOf`
3. set
4. set的简化

```js
var array = [1,2,3,2,3,2,2,4,5,6]
function quchong1(arr){
    var res = [];
    for (var i =0;i<arr.length;i++){
        for(var j=0;j<arr.length;j++){
            if(res[j] == arr[i]){
                break;
            }else{
                if(j ===arr.length-1){
                    res.push(arr[i])
                }
            }

            
        }
    }
    return res;
}
//使用indexOf
function quchong2(arr){
    var res = []
    for(var i=0;len = arr.length,i<len;i++){
        var curr = arr[i];
        if(res.indexOf(curr) ===-1){
            res.push(curr);
        }
    }
    return res;
}

//set
function quchong3(arr){
    return Array.from(new Set(arr))
}
//set的简化
function quchong4(arr){
    return [...new Set(arr)]
}
```



## 如果有一个大的数组，都是整型，怎么找出最大的前10 个数

 排序数组，输出前10个

## 知道数据结构里面的常见的数据结构

常见的数据结构有链表，栈，队列，树，更深一点的就还有图，但是考的不怎么多

## 找出数组中第k大的数组出现多少次，比如数组【1，2， 4，4，3，5】第二大的数字是4，出现两次，所以返回2

>  对数组进行排序，找到第k大的数，然后看第k大的数有几个，返回

## 合并两个有序数组

> 即是采用归并排序即可



## 防抖和节流

防抖：在一定时间内，规定事件被触发的次数。触发高频事件后 n 秒后函数只会执行一次，如果n 秒内高频事件再次被触发，则重新计算时间

节流：只允许一个函数在 X 毫秒内执行一次。高频事件触发，但在 n 秒内只会执行一次，所以节流会稀释函数的执行频率。

```js
//防抖
function debounce(fn,delay){
    let timeout = null;
    return function (){
        clearTimeout(timeout)
        timeout = setTimeout(()=>{
            fn.apply(this,arguments)
        },delay)
    } 
}
//节流
function throttle(fn){
    let canRun = true;
    return function(){
        if(!canRun) return;
        canRun = false;
        setTimeout(()=>{
            fn.apply(this,arguments)
            canRun = true;
        },500)
    }
}
```



## 深拷贝、浅拷贝 

所有的基础数据类型的赋值操作都是深拷贝

通常利用上面这点，来对引用数据类型做递归深拷贝浅拷贝：Object.assign 或者 扩展运算符

深拷贝：JSON.parse(JSON.stringify(object)) 深层递归

局限性：会忽略 undefined，不能序列化函数，不能解决循环引用的对象

### 手写实现深拷贝/浅拷贝

浅拷贝

```js
function copy(obj){
    let cloneObj = {}

    for(let i in obj){
        cloneObj[i] = obj[i];
    }
    return cloneObj;
}
```

深拷贝

- 考虑基础类型引用类型

- RegExp、Date、函数 不是 JSON 安全的

- 会丢失 constructor，所有的构造函数都指向 Object 破解循环引用

```js
function deepClone(obj){
    if(typeof obj === "object"){
        var result = obj.constructor === Array? []:{};

        for (var  i in obj){
            result[i] = typeof obj[i] === "object" ? deepClone(obj[i]) : obj[i];
        }
    }else{
        var result = obj;
    }
    return result;
}
```





## 单例模式★★

## 手写promise.all和promise.race★★

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



## 模拟实现new ★

## 实现call/apply/bind ★

## 实现repeat函数，每隔一段时间执行一次函数，重复n次。

1. ```javascript
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

## 编程题：将数组转成树形结构的对象

## 实现一个正方形，拖拽窗口，正方形等比例缩放

## 编程题：判断一个字符串是否完全由某个子串重复组成

## Diff算法

## 给一段HTML，写出它的VDOM；写一个函数去解析这个VDOM，把元素添加到DOM上。

## 一个div块，设置其为两个效果，一个为渐隐效果，一个为点击空白处显示和隐藏

## ajax封装成promise

## 写一个 vue 组件，实现类[百度](https://www.nowcoder.com/jump/super-jump/word?word=百度)的搜索框，可以出现自动的下拉列表，里面出现可能的和文字相关的信息（自动补全）

## LeetCode 打家劫舍

## 斐波那契第50项

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

## CSS布局（水平竖直）

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

## 图片缩放居中

```css 
img {
    display: block;
    margin: auto;
    width: 40%;
}
```



1. 卷

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

## 给定一个整数数组和一个目标值，找出数组中和为目标值的两个数。 [算法]()要求 o(n)

(一个值只能用一次，匹配多个值，需要都返回 ，( [1，1，1，2，2，5，55] => [1,2] , [1,2] )

## 给定两个版本号，比较两个版本号的大小。.号作为分割符使用，版本号中只有数和.号。  （0.1 < 1.1.1 < 1.2 < 13.37  ）
例如：给定一个function输入两个参数 targetVersion , currentVersion，比较后返回 1， 0 ，-1 ( 大 ，等于 ，小于 )

## 用reduce写一个map方法

## CSS3写一个环形进度条

## 括号匹配

```js
function isValid(str){
    let strArr = str.split('');
    left = [];
    for(let i = 0;i<strArr.length;i++){
        if (strArr[i] == '(' || strArr[i] == '['||strArr[i] == '{'){
            left.push(strArr[i]);
        }else{
            if(strArr[i] == ')' && left.pop()!='('){
                return false;
            }
            if(strArr[i] == ']' && left.pop()!='['){
                return false;
            }
            if(strArr[i] == '}' && left.pop()!='{'){
                return false;
            }
        }
    }
    return left.length == 0;
}
```

## 全排列

```js
function fullpermutate(str) {
    var result = [];
    if (str.length > 1) {
        //遍历每一项
        for (var m = 0; m < str.length; m++) {
        //拿到当前的元素
        var left = str[m];
        //除当前元素的其他元素组合
        var rest = str.slice(0, m) + str.slice(m + 1, str.length);
        //上一次递归返回的全排列
        var preResult = fullpermutate(rest);
        //组合在一起
        for (var i = 0; i < preResult.length; i++) {
            var tmp = left + preResult[i]
            result.push(tmp);
        }
        }
    } else if (str.length == 1) {
        result.push(str);
    }
    return result;
}
```



## 手写代码：输入一个数字n，输出从1到n的所有排列，比如输入3，输出123、132、213、231、312、321

## 字符串反转

```javascript
var str="asdfghjkl";
str = str.split('').reverse().join("");

```

## 10进制转指定7进制字符（用额外的7个字符代替原先七进制的0123456）

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

## 深度优先遍历和广度优先遍历

深度优先遍历——是指从某个顶点出发，首先访问这个顶点，然后找出刚访问这个结点的第一个未被访问的邻结点，然后再以此邻结点为顶点，继续找它的下一个顶点进行访问。重复此步骤，直至所有结点都被访问完为止。 

广度优先遍历——是从某个顶点出发，首先访问这个顶点，然后找出刚访问这个结点所有未被访问的邻结点，访问完后再访问这些结点中第一个邻结点的所有结点，重复此方法，直到所有结点都被访问完为止。

```javascript
//深度优先遍历
function deepTraveral(node){
    let nodes = [];
    if (node != null){
        nodes.push[node];
        let childrens = node.children;
        for (let i=0;i<childrens.length;i++){
            deepTraveral(children[i]);
        }
    }
    return nodes;
}
function deepTraval2(node){
    let nodes = [];
    if(node!= null){
        let stack = [];
        stack.push(node)
        while(stack.length != 0){
            let item = stack.pop();
            nodes.push(item)
            let childrens = item.children;
            for(let i=childrens.length-1;i>=0;i--){
                stack.push(childrens[i])
            }
        }
    }
    return nodes;
}


//广度优先
function wideTravel(node){
    let nodes = [],i=0;
    if (node!= null){
        nodes.push(node);
        wideTravel(node.nextElementSibling)
        node = nodes[i++]
        wideTravel(node.firstChild)
    }
    return nodes;
}
//非递归写法
function wideTraveral(node){
    let nodes = [],i=0;
    while(node != null){
        nodes.push(node);
        node = nodes[i++];
        let childrens = node.children
        for(let i=0;i<childrens.length;i++){
            nodes.push(childrens[i])
        }
    }
    return nodes;

}
```



# 第九章 设计模式

## 1.设计模式：单例，工厂，发布订阅

>  单例模式：在它的核心结构中值包含一个被称为单例的特殊类。一个类只有一个实例，即一个类只有一个对象实例。
>
> 工厂模式：在创建对象时不会对客户端暴露创建逻辑，并且是通过使用一个共同的接口来指向新创建的对象。发布订阅模式：在软件架构中，发布订阅是一种消息范式，消息的发送者（称为发布者）不会将消息直接发送给特定的接收者（称为订阅者）。而是将发布的消息分为不同的类别，无需了解哪些订阅者（如果有的话）可能存在。同样的，订阅者可以表达对一个或多个类别的兴趣，只接收感兴趣的消息，无需了解哪些发布者（如果有的话）存在。

## 2.看过一些设计模式的书？你觉得设计模式怎么样？

>  
>
> JS中常用的设计模式中，我最常用的是装饰者模式，在不改变元对象的基础上，对这个对象进行包装和拓展（包括添加属性和方法），从而使这个对象可以有更复杂的功能。

# 第十章 项目

## **1.**介绍一个做过的项目

> 
>
> (1)项目涉及的技术栈和相关的技术点。
>
> (2)遇到的问题。
>
> (3)项目是否做过优化，包括了代码、开发效率、性能、体验等相关领域。
>
> (4)项目存在的一些问题。
>
> (5)这个项目达成的成果。
>
> (6)这个项目给我带来的成长。

## 2.遇到的难题，怎么解决

> 
>
> (1)难点分析,任务拆分,关联自己已有知识储备,能否解决.
>
> (2)搜索引擎查找相关博客/问答平台是否遇到并给出的解答方案.
>
> (3)咨询自己的技术上级/组内技术高手,看能否帮忙解答
>
> (4)在公司内部小组群/大群,提出自己的难点,看是否有人遇到.
>
> (5)借助QQ群/微信群/问答平台,提出相关问题来探讨.

## **3.**简单的自我介绍

> 
>
> 首先请报出自己的姓名和身份。可能应试者与面试考官打招呼时，已经将此告诉了对方，而且考官们完全可以从你的报名表、简历等材料中了解这些情况，但仍请你主动提及。这是礼貌的需要，还可以加深考官对你的印象。
>
> 其次，你可以简单地介绍一下你的学历、工作经历等基本个人情况。请提供给考官关于你个人情况的基本的、完整的信息，如：学历、工作经历、家庭概况、兴趣爱好、理想与报负等。 这部分的陈述务必简明扼要、抓住要点。例如介绍自己的学历，一般只需谈本专科以上的学历。工作单位如果多，选几个有代表性的或者你认为重要的介绍，就可以了，但这些内容一定要和面试及应考职位有关系。请保证叙述的线索清晰，一个结构混乱、内容过长的开场自，会给考官们留下杂乱无章、个性不清晰的印象，并且让考官倦怠，削弱对继续进行的面试的兴趣和注意力。

## **4.**项目的同源处理，跨越相关

>  

1. 什么是跨域？

> 跨域，是指浏览器不能执行其他网站的脚本。它是由浏览器的同源策略造成的，是浏览器对JavaScript实施的安全限制。

1. 什么是同源策略？

> 同源策略（Sameoriginpolicy）是一种约定，它是浏览器最核心也最基本的安全功能，它是由Netscape提出的一个著名的安全策略。
>
> 同源策略是浏览器的行为，是为了保护本地数据不被JavaScript代码获取回来的数据污染，因此拦截的是客户端发出的请求回来的数据接收，即请求发送了，服务器响应了，但是无法被浏览器接收。

1. 其主要限制以下几个方面：

> a.Cookie 、LocalStorage 和 IndexDB无法读取
>
> b.无法获取或操作另一个资源的DOM c.AJAX请求不能发送
>
> 那么什么是同源呢？所谓的同源，就是指两个页面具有相同的协议，主机（也常说域名），端口，三个要素缺一不可。

1. 常见跨域方案

> a.通过jsonp跨域
>
> b.document.domain+iframe跨域
>
> c.location.hash + iframe
>
> d.window.name + iframe跨域
>
> e.postMessage跨域
>
> f.跨域资源共享（CORS）
>
> g.nginx代理跨域
>
> h.nodejs中间件代理跨域
>
> i.WebSocket协议跨域

## **5.**遇到过什么安全问题，怎么解决的

前端常见的安全方面问题：

(1)iframe

(2)opener

(3)CSRF（跨站请求伪造）

(4)XSS（跨站脚本攻击）

(5)ClickJacking（点击劫持）

(6)HSTS（HTTP严格传输安全）

(7)CND劫持

1）iframe

a.  如何让自己的网站不被其他网站的 iframe 引用？ // 检测当前网站是否被第三方iframe引用// 若相等证明没有被第三方引用，若不等证明被第三方引用。当发现被引用时强制跳转百度。if(top.location!= self.location){ top.location.href = 'http://www.baidu.com'}

b.  如何禁用，被使用的 iframe 对当前网站某些操作？

sandbox是html5的新属性，主要是提高iframe安全系数。iframe因安全问题

而臭名昭著，这主要是因为iframe常被用于嵌入到第三方中，然后执行某些恶意操作。

现在有一场景：我的网站需要 iframe 引用某网站，但是不想被该网站操作DOM、不想加载某些js（广告、弹框等）、当前窗口被强行跳转链接等，我们可以设置 sandbox 属性。如使用多项用空格分隔。

allow-same-origin：允许被视为同源，即可操作父级DOM或cookie等 allow-top-navigation：允许当前iframe的引用网页通过url跳转链接或加载 allow-forms：允许表单提交 allow-scripts：允许执行脚本文件 allow-popups：允许浏览器打开新窗口进行跳转

""：设置为空时上面所有允许全部禁止

2）opener

如果在项目中需要 打开新标签 进行跳转一般会有两种方式

// 1) HTML -> <a target='_blank' href='http://www.baidu.com'>

// 2) JS -> window.open('http://www.baidu.com')

/*

- 这两种方式看起来没有问题，但是存在漏洞。
- 通过这两种方式打开的页面可以使用 window.opener 来访问源页面的

> window 对象。

- 场景：A 页面通过 `<a> `或 window.open 方式，打开 B 页面。但是 B 页面存在恶意代码如下：

> *window.opener.location.replace('https://www.baidu.com') 【此代码仅针
>
> 对打开新标签有效】

- 此时，用户正在浏览新标签页，但是原来网站的标签页已经被导航到了百度页面。 * 恶意网站可以伪造一个足以欺骗用户的页面，使得进行恶意破坏。
- 即使在跨域状态下 opener 仍可以调用 location.replace 方法。

> */

a. ` <a target="_blank" href="">`

> <a target="_blank" href="" rel="noopener noreferrer nofollow">a标签跳转url</a>

b.  window.open()

> `<button onclick='openurl("http://www.baidu.com")'>click跳转</button>`

function openurl(url) { var newTab = window.open(); newTab.opener = null;

newTab.location = url;}

3）CSRF / XSRF（跨站请求伪造）

你可以这么理解 CSRF 攻击：攻击者盗用了你的身份，以你的名义进行恶意请求。它能做的事情有很多包括：以你的名义发送邮件、发信息、盗取账号、购买商品、虚拟货币转账等。总结起来就是：个人隐私暴露及财产安全问题。

/* *

阐述 CSRF 攻击思想：（核心2和3）

- 1、浏览并登录信任网站（举例：淘宝）
- 2、登录成功后在浏览器产生信息存储（举例：cookie）
- 3、用户在没有登出淘宝的情况下，访问危险网站
- 4、危险网站中存在恶意代码，代码为发送一个恶意请求（举例：购买商品/ 余额转账）
- 5、携带刚刚在浏览器产生的信息进行恶意请求
- 6、淘宝验证请求为合法请求（区分不出是否是该用户发送）
- 7、达到了恶意目标

> */
>
> 防御措施（推荐添加token / HTTP头自定义属性）
>
> (1)涉及到数据修改操作严格使用 post 请求而不是 get 请求
>
> (2)HTTP 协议中使用 Referer 属性来确定请求来源进行过滤（禁止外域）
>
> (3)请求地址添加 token ，使黑客无法伪造用户请求
>
> (4)HTTP 头自定义属性验证（类似上一条）
>
> (5)显示验证方式：添加验证码、密码等
>
> 4）XSS/CSS（跨站脚本攻击）
>
> XSS又叫CSS（CrossSiteScript），跨站脚本攻击：攻击者在目标网站植入恶意脚本（js/html），用户在浏览器上运行时可以获取用户敏感信息（cookie/ session）、修改web页面以欺骗用户、与其他漏洞相结合形成蠕虫等。浏览器遇到 html 中的 script 标签时，会解析并执行其中的js代码。
>
> 针对这种情况，我们对特殊字符进行转译就好了（vue/react等主流框架已经避免类似问题，vue举例：不能在template中写script标签，无法在js中通过 ref或append等方式动态改变或添加script标签）
>
> XSS类型：
>
> 持久型XSS：将脚本植入到服务器上，从而导致每个访问的用户都会执行非持久型XSS：对个体用户某url的参数进行攻击
>
> 防御措施（对用户输入内容和服务端返回内容进行过滤和转译）
>
> a.现代大部分浏览器都自带 XSS 筛选器，vue/react 等成熟框架也对 XSS 进行一些防护
>
> b.即便如此，我们在开发时也要注意和小心
>
> c.对用户输入内容和服务端返回内容进行过滤和转译
>
> d.重要内容加密传输
>
> e.合理使用get/post等请求方式
>
> f.对于URL携带参数谨慎使用
>
> g.我们无法做到彻底阻止，但是能增加黑客攻击成本，当成本与利益不符时自然会降低风险

1. 、ClickJacking（点击劫持）

> ClickJacking 翻译过来被称为点击劫持。一般会利用透明 iframe 覆盖原网页诱导用户进行某些操作达成目的。
>
> 防御措施
>
> a.在HTTP投中加入 X-FRAME-OPTIONS 属性，此属性控制页面是否可被嵌入
>
> iframe 中【DENY：不能被所有网站嵌套或加载；SAMEORIGIN：只能被同域网站嵌套或加载；ALLOW-FROM URL：可以被指定网站嵌套或加载。】
>
> b.判断当前网页是否被 iframe 嵌套（详情在第一条 firame 中）

1. 、HSTS（HTTP Strict Transport Security：HTTP严格传输安全）网站接受从 HTTP 请求跳转到 HTTPS 请求的做法，例如我们输入

> "[http://www.baidu.com](https://link.zhihu.com/?target=http://www.baidu.com)"或"[www.baidu.com](www.baidu.com)"最终都会被302重定向到
>
> "[https://www.baidu.com](https://link.zhihu.com/?target=https://www.baidu.com)"。这就存在安全风险，当我们第一次通过 HTTP 或域名进行访问时，302重定向有可能会被劫持，篡改成一个恶意或钓鱼网站。
>
> HSTS：通知浏览器此网站禁止使用 HTTP 方式加载，浏览器应该自动把所有尝试使用 HTTP 的请求自动替换为 HTTPS 进行请求。用户首次访问时并不受 HSTS 保护，因为第一次还未形成链接。我们可以通过 浏览器预置HSTS域名列表或将HSTS信息加入到域名系统记录中，来解决第一次访问的问题。

1. 、CDN劫持

> 出于性能考虑，前端应用通常会把一些静态资源存放到CDN（Content Delivery Networks）上面，例如 js 脚本和 style 文件。这么做可以显著提高前端应用的访问速度，但与此同时却也隐含了一个新的安全风险。如果攻击者劫持了CDN，或者对CDN中的资源进行了污染，攻击者可以肆意篡改我们的前端页面，对用户实施攻击。
>
> 现在的CDN以支持SRI为荣，script 和 link 标签有了新的属性 integrity，这个属性是为了防止校验资源完整性来判断是否被篡改。它通过 验证获取文件的哈希值是否和你提供的哈希值一样来判断资源是否被篡改。
>
> 使用 SRI 需要两个条件：一是要保证 资源同域 或开启跨域，二是在<script> 中 提供签名 以供校验。
>
> integrity 属性分为两个部分，第一部分是指定哈希值的生成算法（例：sha384），第二部分是经过编码的实际哈希值，两者之前用一个短横(-)来分隔

## **6.**让你带领一个小团队完成一个项目，我会怎么做？

> ![](media/image22.png){width="7.0033344269466316in" height="1.1366666666666667in"} 
>
> 根据团队的技术栈，指定开发计划，然后分配任务，定人定点，推进项目的进展。

## 7.前端的项目如何进行优化，移动端呢

>  
>
> 前端性能优化有七大手段：减少请求数量，减少资源大小，优化网络连接，优化资源加载，减少重绘回流，使用性能更好的API和构建优化

1. 减少请求数量：通过减少重定向，使用缓存，不适用CSS\@import，避免使用空的src和href等手段
2. 减少资源大小：通过压缩HTML，CSS，JS，图片，此外在安卓下可以使用webp 格式的图片，它具有更优的图像数据压缩算法，能带来更小的图片体积，还可以开启gzip,gzip编码是以后总用来改进web应用程序性能的技术，
3. 优化网络连接：使用CDN，使用DNS预解析，并行连接， 4）优化资源加载，通过优化资源加载位置和时机，使用资源预加载preload和资源预读取prefetch

<!-- -->

1. 减少重绘回流，

> 避免使用层级较深的CSS选择器，以提高CSS渲染效率避免使用CSS表达式，
>
> 给元素适当的定义高度或最小高度，否则元素的动态内容载入时，会出现页面晃动，造成回流，
>
> 不要使用table布局，
>
> 能用CSS实现的效果，尽量使用CSS而不用JS实现

1. 使用性能更好的api

## **8.**项目中使用了 **iframe**，说说 **iframe** 的优缺点

>  
>
> iframe的优点：
>
> (1)iframe能够原封不动地把嵌入的网页展现出来。

(2)如果有多个网页调用iframe，只需要修改iframe的内容，就可以实现对调用iframe的每一个页面内容的更改，方便快捷。

(3)网页如果为了统一风格，头部和版本都是一样的，就可以写成一个页面，用 iframe来嵌套，可以增加代码的可重用性。

> (4)如果遇到加载缓慢的第三方内容，如图标和广告等，可以用iframe来解决。
>
> iframe的缺点：
>
> (1)会产生很多页面，不容易管理。
>
> (2)在几个框架中都出现上下、左右滚动条时，这些滚动条除了会挤占已经非常
>
> 有限的页面空间外，还会分散访问者的注意力。

(3)使用框架结构时，必须保证正确设置所有的导航链接，否则会给访问者带来很大的麻烦。比如被链接的页面出现在导航框架内，这种情况下会导致链接死循环。

> (4)很多的移动设备（PDA手机）无法完全显示框架，设备兼容性差。
>
> (5)iframe框架页面会增加服务器的http请求，对于大型网站是不可取的。

# 第十一章 职业发展

## **1.**介绍一下前端的学习经历

> 
>
> (1)原生js/html/css阶段
>
> (2)html5/css3/jquery/js进阶阶段
>
> (3)vue阶段
>
> (4) react 阶段

## **2.** 作为一个专业的前端，你觉得应该掌握哪些知识

> 
>
> (1)计算机基础（计算机网络，数据结构，算法，编译原理...）
>
> (2)前端常用的语言基础（JS，HTML，CSS）也可以看下TS

(3)上面一条的拓展。为了更好的沟通和更全面的认知最好也涉猎一下服务端/ 客户端知识

> (4)用于团队协作的工具（如：Git）
>
> (5)用于工程化建设的工程化工具（如：Webpack）

## **3.**什么时候接触前端

> 根据自身实际情况回答

## **4.**大学学过哪些编程的课

> 
>
> 《C++语言程序设计》《Java语言程序设计》，《数据结构》，《编译原理》，
>
> 《软件工程》，《算法分析与设计》，《数据库系统原理》，《计算机组成原理》，
>
> 《操作系统》，《互联网程序设计》，《汇编语言与计算机系统组成》，《计算机网络》另外还有很多选修课，就不一一列举了。

## **6.**对未来三年职业的规划

>  成为一个全栈工程师

## **7.**你一般是通过什么方式学习前端的？

>  
>
> 自学，W3school等网站，阮一峰、冴羽等大神的博客，GitHub，掘金，segmentfault 等交流平台，（根据自身实际情况回答）

## **8.**你还有什么我没问到的优势吗

> 

1. 编译原理：TypeScript、Vue3、跨端框架都强烈依赖这项技术，如果你是月薪超过 20k 的前端，一定要重温一下编译原理，才能看懂这些技术的源码.
2. 函数式编程：React 的 Hooks 用到的思想来自于函数式编程，什么是副作用，你能不能说清楚，20k 以上的前端建议重点学习一下.
3. 后端知识：前端技术已经有五年没有较大变化了，想要突破瓶颈的前端可以以 Node.js 为抓手（阿里喜欢说这个词）来进入后端编程领域，需要学的包括但不限于关系型数据库、Redis、非关系型数据库、HTTP、TCP/IP、MVC 架构等
4. 前端知识巩固：Vue 3 和 React 的源码可以了解一下

## **9.**看过什么书

> 推荐阅读：
>
> [《Head](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/25752357/) [First](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/25752357/) [HTML与CSS》](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/25752357/)、[《CSS](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/26745943/) [揭秘》](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/26745943/)、[《CSS](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/27615777/) [世界》](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/27615777/)、[《CSS权威指南](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/2308234/)（第三版）》、[《JavaScript语言精粹》](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/3590768/)、[《JavaScript高级程序设计（第三](https://link.zhihu.com/?target=https%3A//book.douban.com/subject/10546125/)版）》...

## **10.**比较厉害的技术

> 
>
> 1）前端框架和语言层面
>
> 9月份 Vue3.0 发布，声称对 TypeScript 有着更好的开发体验，通过从不同框架级别 TS 支持上，我们可以看出社区的整个风向从2019年的大家都去学习应用 TS，变成了大家如何把 TS 用的更好这个方向上来了。
>
> 所以我认为今年 TypeScript 的火热程度还是应该排名很靠前的，我今年也使用 TypeScript 重构了 Daruk 的服务框架推出了2.0版本，让 TS 开发者拥有更好的 TS 开发体验。
>
> 接下来就是两大重磅框架的更新历程对比，Vue3 前面说了一句。而 React 也在十月也发布了 React 17 的 release 版本。这两大主流框架的频繁更新，也说明了社区和作者都在一同演化。
>
> 在 Vue3中除了更好的支持 TS 外，还更新了CompositionAPI。而 React17 主要是集中精力在升级体验上，虽然没有新的 Feature 但是提升了和解决了很多之前版本潜在的问题。
>
> 要说哪个最火还是要看个人实际的使用场景和喜好，但是2020年来看还没有别的框架可以与之一战。
>
> 2）大前端相关技术栈
>
> 今年基于Chromium的微软edge浏览器也已经推出。google 在 web 端的发展产生了对开发者深刻的影响。Chrome 80+ 也已经发布多个版本，提供了一系列的新特性，比如Core Web Vitals标准，Desktop PWA等都值得我们去关注。
>
> 我们说完了浏览器相关的那点技术之后，再聊聊大前端相关的一些技术实践，比如 Flutter。
>
> 很多前端在今年已经从 web 开发转型为 Flutter 开发，学习和使用 Dart 技术来构建 UI，这是很多大厂的前端工程师正在经历的事情（包括我的部门也在尝试这个事情），这个趋势应该在未来几年还会持续。
>
> 客户端 electron 在今年也有着长足的进展，一年内多次更新版本一路到了
>
> 10.1.5。随着疫情影响，国内在线教育的又一波兴起。很多桌面软件，网课软件都在采用这个技术来进行开发，市场上的岗位也开始变多，electron 技术可以说在今年也有火的趋势。
>
> 然后我们再看看BFF 层，nestjs依然坚挺，越来越多的人开始跳过学习 express 和 koa 开始学习更丰富的 web 框架了，比如 egg 或者我的 daruk，开发者已经在慢慢形成共识，在 webframework 的路上开始越走越远，裸写 nodejsweb 服务的时代已经开始慢慢褪去。
>
> 不得不提的还有 serverless 在前端的普及，在2020年到达了一个新的高潮。
>
> 阿里云，腾讯云，头条云等等国内的互联网厂商也都开始大玩 serverless 概念。从对内服务开始转向对外服务，普及的势头很猛，也有落地的趋势和场景。今年的 D2同样也有 serverless 的专场，可见受重视程度非比寻常。
>
> 3）工程化提效和个人素质提升
>
> 再离我们近一些的推动生产力的技术，比如据我所知在用 CI/CD 和 pipeline 管理上线流程的公司越来越多，这种去年还可以出去吹一吹的东西，今年也逐步变成了业界标配基础能力，如果不会的同学可要抓紧学习了。
>
> 2019年前大家都疯狂吐槽面试刷 medium 题目没用，而2020年后大家开始默认面试某些公司都至少要刷到medium程度的题目。这对很多前端来说是一个心智和素质的提升与转变，大家在接触新技术的同时，也慢慢发现，前端整个职业环境的变化，越来越多的公司对人的整体综合素质要求变高了。

## **11.**你学前端怎么坚持下来的

> 
>
> 写博客，从总结基础姿势开始
>
> 写工具，chrome 插件，vscode 插件，开发成本都不高，重要的是想一些点子，解决一些实际问题，问题不用太大，关键是有用
>
> 写点有意思的东西，例如搞个小游戏给自己玩，写个小彩蛋什么的
>
> 学点有意思的，就是那种你觉得很有意思，学会了可以干点不一样的事情的东西，例如 app 开发，nodejs 开发等

## **12.**学过哪些框架？

> 
>
> Bootstrap：
>
> 让你的页面更简洁、直观、强悍、移动设备优先的前端开发框架,让web开发更迅速、更简单。它还提供了更优雅的HTML和CSS规范，它即是由动态CSS语言 Less写成。有着丰富的网格布局系统以及丰富的可重用组件，还有强大的支持十几的JavaScript、jQuery插件以及组件定制等。
>
> React：
>
> React 可以非常轻松地创建用户交互界面。为你应用的每一个状态设计简洁的视图,在数据改变时 React 也可以高效地更新渲染界面。
>
> vue.js：
>
> Vue.js是一个构建数据驱动的 web 界面的渐进式框架。Vue.js 的目标是通过尽可能简单的 API 实现响应的数据绑定和组合的视图组件。
>
> Angular： Angular是一款优秀的前端JS框架，已经被用于Google的多款产品当中。
>
> AngularJS有着诸多特性，最为核心的是：MVVM、模块化[、自动化双向数据绑定](https://link.zhihu.com/?target=https://www.angularjs.net.cn/tutorial/10.html)、语义化标签、[依赖注入](https://link.zhihu.com/?target=https://www.angularjs.net.cn/tutorial/17.html)等等。
>
> （前端框架还有很多，建议根据自身的实际学习情况回答）
>
> **13.**你理解的框架

# 第十二章 Hr面

## **1.**自我介绍

1. 结合招聘岗位，只讲重点。

> 简历内容这么多，实际的你，更有很多很多可以描述的东西。但时间有限，没有面试官会听你说个没完。
>
> 根据你求职的岗位，说重点即可。
>
> 其实简历制作的原则，也是一样。只是自我介绍时间更短，内容更精华。

1. 有理有据，少说空话。

> 如果你说"自己学习能力强"，这就是一句假大空的话。谁都可以说自己学习能力强。
>
> 你如果真的在这方面有突出，就要举一个例子，比如是1个月从0到1考了什么证书等。

1. 有开头有结尾，有逻辑。

> 开头问候，结尾总结。中间1、2、3条理清楚。

1. 特别提醒。

> 自我介绍中的内容，很可能是面试官后续发问的内容。所以，一是要引起重视，讲最重要的，你最想让面试官知道的内容。 而是做好准备，扬长避短，不要给自己挖坑。
>
> 比如前面你说自己学习能力强，但是没有举例子。
>
> 面试官很可能，顺着你的话问你，怎么证明你学习能力强呢？ 结果你答不上来，或者是非常普通的成绩，根本不能算是"学习能力强"。 那你就是给自己挖坑了。
>
> 其实自我介绍也是每个人各有不同，说起来也只能提供大致的思路。和你具体的求职岗位、经历、个人风格有很大的关系。

## **2.**为什么要学习前端

> 我首先是一个程序员，然后我喜欢并且擅长写javascript，再然后才是一个所谓的"前端工程师"。
>
> javascript是一个真正意义上的跨平台语言，浏览器是少有的横跨PC/移动设备的GUI平台，nodejs也是一个高性能且开发效率高的平台，我相信未来随着计算能力的不断提高，这些技术必然会生出更多炫酷的东西。

## **3.**到现在为止接触过几个项目，有在哪里实习过？

> 1）梳理之前实习的工作，按岗位相关性强弱排序 2）按照：总结-做什么-做出了什么成果进行讲述

1. 如果你的工作不方便量化成果，注重在叙述中展示你的能力。
2. 礼貌、大方，对所应聘公司有一定的了解

## **4.**让你收获最多的项目，你做了什么？

> 项目经验这块因人而异，把觉得做的有亮点的东西挑出来，从四个方面来准备：功能模块的实现达到了什么效果
>
> 遇到了什么问题，是如何解决的涉及到的相关知识点
>
> 项目经验和知识点 其实是一个双向的过程，要 试图去找到它们之间的联系：谈到项目经验的时候，可以说：做完xx之后，我还去了解了一下yy背后的原理， xxx，这里体现的是你是否有求知欲 。
>
> 谈到知识点的时候，可以说：yy的原理是这样的，在xx项目中我是如何应用它来解决问题的，这里体现的是你是否具备把知识付诸实践的能力。

## **5.**个人的优缺点

1. 不宜说自己没缺点。
2. 不宜把那些明显的优点说成缺点。
3. 不宜说出严重影响所应聘工作的缺点。 
4. 不宜说出令人不放心、不舒服的缺点。
5. 可以说出一些对于所应聘工作"无关紧要"的缺点，甚至是一些表面上看是缺点，从工作的角度看却是优点的缺点。

我的工作执行力很高，领导给我安排的任务我也能较快的完成，但是可能在工作的时候会少一些深入的独立思考，对整个工作的安排缺乏战略眼光，对于这方面能力需要我进一步的努力，我也将继续学习，通过阅读、向前辈请教等改善自己的不足。

## **6.**读不读研

> 对于大公司，可以答:
>
> 我目前没有这方面的打算，但是如果公司的发展需要我提升自己这方面的能力和学历，我会认真考虑考研，以便提高自己的职业技能和素养，更好地为公司谋取利益。
>
> 对于小公司，可以答:
>
> 我并不打算考研，对于我来说，我更加重视在社会上实际工作经验的积累，我觉得我的工作更加适合实践而不是理论，比起考研，我更加希望能跟公司一起成长，为公司做出贡献

## **7.**说说你最荣耀的事

> 作为面试官，我们希望了解你最大的闪光点，而不是你的缺点、不足。对这个问题感到很头疼的，不妨认真想想，你二十多年的人生，有为一件事努力过吗，有满腔热情去做的事情吗，有即便前路艰险也义无反顾的事吗？如果没有，你不觉得自己的人生是为别人而活，是浑浑噩噩的过日子吗？关于这个问题，你也无法用一个标准答案来回答。
>
> 我见过很多人讲到某些事情时眼睛里散发出的那种神采，也见过无数人试图编造一个故事时的眼神迷离，你真的无法在这种事情上撒谎，也没用必要在这种事情上撒谎。
