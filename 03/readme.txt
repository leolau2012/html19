笔记
==================================================
不兼容
html5 		没有多特别。其实还是html。
css3 		没有多特别。其实还是css。
==================================================
HTML页面有文档头
HTML5
	<!doctype html>

=================================================
html5新增
获取元素
	document.querySelectorAll('选择器');
	document.querySelector('选择器');默认获取第0个
=================================
class的操作
	obj.classList 		class列表对象
				.add() 		添加
				.contains()	检测是否包含某个class
				.length 	长度
				.remove() 	删除
				.toggle() 	切换

=====================================
关于自定义属性
	向后兼容
		自定义属性
			data-xxx

		dataset 		自定义属性的集合

=============================================
CSS3 			新样式
css3中的选择器
属性
	E[index] 		有index属性的
	E[index=a] 		index属性值就是a
	E[index~=a] 	index属性只要包含a
	E[index^=a] 	index属性以a开头
	E[index$=a] 	index属性以a结尾
	E[index|=a] 	index属性就是a或者以a-开头
==============================================
伪类选择器
E:nth-child(位置){}
E:nth-child(odd) 		奇数行
E:nth-child(even) 		偶数行

文本选择器
E:first-line 			第一行
E:first-letter 			第一个字
E::selection 			选中文字
E::before 				前面
E::after 				后面

===============================================
css3
圆角
	border-radius:px %;

	border-radius: 一个值; 	四个角
	border-radius: 左上右下 右上左下;
	border-radius: 左上 右上左下 右下;
	border-radius: 左上 右上 右下 左下;

运动:
	transition:	1s  	all  	ease;
				时间 	选项 	运动类型

浏览器前缀
-webkit-transition 		Chrome、Safari、Opera
-moz-transition 		Firefox
-ms-transition 			IE
-o-transition 			Opera
transition 				不加前缀

js写
-webkit-transition 		WebkitTransition
-moz-transition 		MozTransition
-ms-transition 			msTransition
-o-transition 			OTransition
transition 				transition

一般只管-webit-和标准就ok了.
=========================================
阴影
box-shadow:x y blur color;

box-shadow:[inset] x y blur [范围] color;

阴影可以叠加
box-shadow:x y b c,x y b c,x y b c......;

文字阴影
text-shadow:x y blur color;


ev.clientX+scrollLeft 			ev.pageX
ev.clientY+scrollTop 			ev.pageY
========================================
颜色:
	单词
	十六进制
	rgb(r,g,b)
	rgba(red,green,blue,alpha)

===========================================
单位:
	deg 		° 		角度
渐变
线性渐变
	-webkit-linear-gradient(c,c....);
	-webkit-linear-gradient(方向,c,c....);
	-webkit-linear-gradient(角度,c,c....);

	-webkit-linear-gradient(c s,c e,c s,c e....);

	-webkit-repeating-linear-gradient();



动画
	定义：
		@keyframs 名字{
			from{}
			to{}
		}
	调用：
	-webkit-animation-name: 		名字
	-webkit-animation-duration: 		时间
	-webkit-animation-timing-function: 	类型
	-webkit-animation-iteration-count: 	次数
							infinite 	无限
	-webkit-animation-direction: 		方向
							alternate 	交替
	-webkit-animation-delay: 			延迟
