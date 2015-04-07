# web前端快速入门


> web前端技术涉及的知识量很大很广（水很深），不可能一下就掌握住，这里主要说下我的学习经验，方便快速入门。
当然也就是入门，后续的需要你们大量做项目去掌握它。目前web前端主要分两块：PC端＋移动端。
PC端前端就是在PC浏览器里面去浏览网页所用到的技术主要工作是切图(div+css)+js网页特效＋前端表单验证＋后端ajax交互。
移动端主要是用html5+css3技术实现的网页，在手机终端中用的比较多，用到的技术和工作流程大致和Pc 端是一样的。只不过，用到了最新的技术h5+css3。可以不用管IE系列浏览器。PC端受浏览器版本和IE系列浏览器的束缚，不能大规模的用新技术。所以目前主流的做法PC端一套代码，然后移动端又是一套代码。其实PC端大部分时间都在做兼容性工作，虽然移动端可以用最新的技术，但目前的移动端浏览android 和 IOS两大平台系统中，啃还是有的～～～～


> 可以看到：只要把切图(div+css)＋js学会了。你的前端基本上就入门了，然后在学习下当下流行的js框架，走几个项目就ok了。
接下来说切图了，有人说切图很简单，用ps切片工具，把想要图片切下来就可以了，没错，其实切图是一门艺术，切得好，网站性能好，切得不好，网站就很慢。这就需要根据实际情况，实际分析了。



具体流程如下：

## 学会photoshop切片工具，能用photoshop导出你想要的图片就可以了。
* 了解网页常用的图片格式，目前主流的png、jpg 、gif
* 了解半透明和全透明格式，png8和png24
* ie6不支持透明格式
* 了解同一张图片存为不通格式的体积的大小
* 移动端主要用png格式多些

## [学习常见的html标签(平时用的比较多的标签)](http://www.w3school.com.cn/html/html_basic.asp)
### 块级元素
* div、p、ul、table、dl、form、h1、h2、h3、h4、h5、h6、hr、fieldset###块级元素
### 内敛元素
* span、a、label、em、i、br、img、input、strong

* 把这些标签一个个自己敲一遍，看看在网页里面是长成啥样的？知道各个标签的具体含义(语义化)
  思考:同一个布局即可以用div实现，又可以用p实现，那到底是用div还是用p？

## [学习css基础知识点](http://www.w3school.com.cn/css/css_syntax.asp)
* 理解盒模型(很重要的知识点)
* 理解什么叫浮动及如何清除浮动
* 理解定位position（relative,absolute）
* 理解元素和内敛元素相互转化display
* [参考学习资料](http://www.blueidea.com/tech/site/2006/3358_4.asp)	
* 建议看下  **css那些事儿**  书籍里面讲解很清楚(看第1部分 CSS入门篇、第2部分 CSS页面布局篇、第17章 谈谈清除浮动)
* ** css权威指南 ** 

## [网页布局实战](http://www.baidu.com)
要求：
1. 利用之前学习的html＋css技术实现山寨版本百度(纯静态页面)
2. 必须手写代码，严禁用DW生成代码
3. 要求至少兼容ie8。


## [移动网页开发](https://github.com/jtyjty99999/mobileTech)

1. [学习下常见的html5新标签](http://www.w3school.com.cn/html5/index.asp)
	header、footer、nav、menu、aside、section、article	
2. [学习下常用的css3属性](http://www.w3school.com.cn/css3/index.asp)
	border-radius、shadow、RGBA、box-shadow、
	transform、transition、animation、
	box-sizing、background-size
3. [学习下viewport](http://davidbcalhoun.com/2010/viewport-metatag/)

## 移动网页布局练习
  练习:绑定银行卡送礼页面.html






