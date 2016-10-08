很多人觉得html5很难，其实它简单的很，比原生js学起来难度小的多。很多人不信，
那我就出一套系列教程 19天学会html5，要把让html5学习像写个选项卡一样简单。
所有源代码开源在 https://github.com/leolau2012/html19 里面
技术只有不断地开源，才能进步。抱残守缺，敝帚自珍，没什么好处。
htm5教程01 30分钟玩转 svn和git
SVN
	集中式管理
	checkout  地址 用户名，密码
	原则 先 update，再commit
	常用工具tortoiseSVN	
	提交到SAE（免费）
	个人推荐 ucloud 地址 http://www.ucloud.cn/
	SVN缺点：
		局域网，离开功能室没法工作
		速度非常慢
----------------------------------------------------------------
git
	分布式
	安装客户端
	git-scm
git-scm用法
	1.图形界面 太土了
	2.命令行 原理 linux 右键 git-bash
常用linux命令 没有提示就是成功
	linux			 
	ls			 
	cd..返回上一级		 
	cd 目录名		 
	创建文件touch 文件名	 
	删除 rm		 
	编辑
		a).vi 文件名
		b).按i
		c).esc-> :wq回车
	clear 清屏			clear
	创建目录	mkdir
	删除		rmdir
快捷方式
	创建并输入内容
	echo 内容 >b.txt
--------------------------------------------------------
正式说git玩法
	本地目录如何变仓库（目录=git目录 =仓库）
右键git-bash
cd->html19
	1.本地目录变成git目录	git init
	2.查看此时git 状态	git status
	3.工作区文件添加到缓存区 git add
	4.缓存区添加到仓库	git commit
-------------------------------------------------------
配置git
1.生成本地秘钥
	ssh-keygen -t rsa -C  "leolau2012"

	C:\Users\leolau\.ssh
	id_rsa	私有
	id_rsa.pub 公共
	登录 git ->settings ->sshkey ->粘贴完事儿。连接上了
2.配置一下我是谁
	git config -l 查看当前配置
	配置用户名和密码
	git config –global user.email “xxx@xx.com”
	git config –global user.name “xxxxx”	

-------------------------------------------------------
github类似于新浪app 跟git半毛钱关系没有
玩git就两件事
上传
	第一次 动作有点难，人生都有第一次
	跟github建立关系
	git remote add origin https://github.com/leolau2012/html19.git
	git push -u origin master
	以后
	git push
下载
	下载
	git clone https://github.com/leolau2012/html19.git
-------------------------------------------------------	 
github搭建
	建一个与用户名同名仓库 提交完事儿
-------------------------------------------------------
以上所有代码 下载地址
https://github.com/leolau2012/html19



