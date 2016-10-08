html5
---------------------------------------------
html5重点还是学js，默认情况下我们都在服务器情况下开发
html5内容
基础应用	日常小的知识
图形开发	canvas vml svg Raphael JS 
移动应用	移动端布局等 flex等
游戏开发	webworker websocket  webGl
---------------------------------------------
html5新标签 新属性
	新标签：有用，国外  ->自己去网上找
	'没用':header、nav
	相当有用：pc 都是flash
		video
		audio  播声音  mp3
		canvas 画图
	文档头：<!doctype html>
	页面编码：<meta charset="utf-8">
------------------------------------------，

pc：  IE6+  chrome  FF

移动端： webkit （chrome）
	
	phone,pad,tv..  大小不一
	

不兼容：

----------------------------------------
语义化：
	1. 用户(程序员)
	2. seo (搜索)
		google  语义化
		baidu   钱

-----------------------------
标签：
	head：头部
	nav:  导航
	footer： 底部
	section： 块
	aside： 
		相关阅读，广告
	article
		文章

	time  时间
	mark	标记(默认背景色)
	address  地址（默认斜体）

	details  简介(属性：open)
		配合summary
		请默认： outline:none
	....

	datalist
		必须配合： 
			<input list="id">
			datalist id="id"

	progress
		value
		min
		max
	meter
		value
		min
		max

<!--[if lt IE9]> 
	<script src="html5shiv.js"></script>
<![endif]-->
只处理标签
-----------------
<!--[if lt IE9]>
	小于IE9
<![endif]-->

<!--[if gt IE9]>
	大于IE9
<![endif]-->

------------------
audio /  video  / canvas..
----------------------------------------------
js:

1. 选择器   IE8+
		document.querySelector();
			默认选择 第一个
		document.querySelectorAll();

	***必须是document.querySelector()
	oBox.querySelector()	

	querySelector('.box .red:nth-child(1)')


2.  
	操作(自定义)属性
	.
	[]
	setAttribute
	dataset:
		写自定义属性的时候：
			index--->data-index
			abc --->data-abc
			xxx --- > data-xxx

	获取:
		Ele.dataset.属性名

	设置：
		Ele.dataset.属性名=值

	删除：
		delete Ele.dataset.属性名

****data-index-abc
	
	获取： Ele.dataset.indexAbc

循环：
	for(var name in Ele.dataset)


1. dataset性能 高于Attribute
	不高
console.time('xxx');
//code
console.timeEnd('xxx');


3. classList

	classList.contains('class名')
		有：true
		没有： false

	classList.add('') 
		每次只能添加一个

	classList.remove('')
		删除

	classList.toggle('')
		切换
4. 
cookie： 32k  封装

localStorage： 5M 直接用 没有过期时间 
	兼容： IE7+
	**在测试IE 必须在服务器环境下

存：
	localStorage.aaa='bbb';

取：
	localStorage.aaa

删：
	delete localStorage.aaa

全删：
	for(var name in localStorage){
		delete localStorage[name]
	}


标准方法:

存：
	localStorage.setItem('userName','aaa');

取：
	localStorage.getItem('userName');

删：
	localStorage.clear();
	全删

----------------------------------------
事件： onstorage

window.onstorage=function(){};

-------------------------------------
.div
#div

css3:
	选择器：

http://www.w3cplus.com/css3/attribute-selectors
属性选择器：
	
	*E[name]   有 name属性的元素(标签)

	*E[name=aaa]  有 name属性而且值是aaa的元素(标签)

	E[name$=aaa] 以aaa结尾的元素

	E[name^=aaa] 以aaa开头的元素

	E[name|=aaa]  -前面是 aaa的元素

	E[name*=aaa] 整个属性值里面 包含aaa的元素

	E[name~=aaa] 指定属性名，并且具有属性值，此属性值是一个词列表，并且以空格隔开，其中词列表中包含了一个value词，而且等号前面的“〜”不能不写；

结构选择器： 
n是从0开始计数的，
但是html标签是从1开始计数的

	*E:nth-child(序号){}

	E:nth-child(2n){}

	E:nth-child(2n+1){}


	E:nth-last-child(序号){} 倒着数


	*E~F{}  E后面的所有F元素

	*E+F{}	 E后面的第一个F元素

	*E>F{}  E下面的第一层F子级

	E:nth-of-type(序号)

	E:nth-last-of-type()

伪类选择器：
	:after 
		三角：
		div:after{
			position: absolute;
			top:0;
			right:0;
			content:'';
			width:0;
			height:0;
			border:8px solid #ccc;
			border-color:#ccc transparent transparent transparent ;
		}
	:before

	:hover
	:active
		点击
	E::selection
		选中文字
		改变背景色
			字体颜色
	::after
	::before
	:empty
	:link
	:target
	:first-line
	:first-letter
	...

------------------------------------


