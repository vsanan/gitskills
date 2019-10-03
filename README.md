# gitskills
这是一个说明文件

Creating a new branch is quick.


0.github ssh加密传输密钥设置
	 a.用户主目录下 .ssh文件夹 dirctory(如果没有请创建)
	 b.github setting > setting key > 添加key  (把.ssh/id_rsa.pub下的公钥复制到里面，其它选项默认设置即可).
1.本地连接github 
	a.右上角新建项目 new repo.
	b.本地连接github $ git remote add origin git@github.com:vsanan/learngit.git  (vsanan github即用户名).
	c.第一次推送 $ git push -u origin master.
	d.调整后提交 $ git push origin master
2. 从github上克隆（clone）
	a.github上新建仓库并钩选 Initialize this repository with a README  (会默认创建 README.md 文件)
	b.从远程克隆 $ git clone git@github.com:vsanan/gitskills.git
		a)github 也可用 https://github.com/michaelliao/gitskills.git 这样的地址克隆.
		b) 默认的git://使用ssh，也可以使用https等其他协议:如a)
		c) 使用https除了速度慢以外，还有个最大的麻烦是每次推送都必须输入口令，但是在某些只开放http端口的公司内部就无法使用ssh协议而只	能用https。
3.创建分支 $ git checkout -b dev  相当于 $ git branch dev+ $ git checkout dev（即创建并切换到新创建的分支）
	a.查看所有分支 git branch（当前分支前面会标一个*号）
	b.测试分支 添加内容并提交，然后切换到master分支 $ git checkout master （刚添加的内容不见了）
	c.合并分支 $ git merge dev （内容回来了）
	d.删除分支 $ git branch -d dev 
	e.用分支调整更安全。


	查看分支：git branch

	创建分支：git branch <name>

	切换分支：git checkout <name>或者git switch <name>

	创建+切换分支：git checkout -b <name>或者git switch -c <name>

	合并某分支到当前分支：git merge <name>

	删除分支：git branch -d <name>
	