#git与github

### git是什么?

	git一个版本控制的工具。

### github是什么?

	github:网站、代码托管、远程仓库、存放静态资源的博客域名地址。

###	git与github相关联

	1.把创建好的项目方到本地

	2.进入盘符:cd

	3.ls或ll查看目录（可以按Tab键补全文件名）

	4.退回:cd..  清屏：clear

	5.克隆：git clone github地址

	6.工作区添加了一个文件

###	git的存放
	
	1.从工作区到暂存区 

			git add 文件名

	2.从暂存区到版本区

			git commit -m "注释"

	3.形成版本之后要把代码放到远程仓库

			git push origin master

### git对比

	1.工作区与暂存区的区别 

			git diff

	2.暂存区与版本区的区别

			git diff --cached

	3.工作区与版本区的区别

			git diff master


###	git撤销

	  ***  git reset HEAD 文件名

	可以将暂存区的文件撤销回暂存区(绿色变红色)

	  *** git checkout --文件名
	  *** git commit -m "注释" --amend

	工作区代码还原暂存区或版本去

###	git删除

	1.如果手动删除了工作区的文件,也想在git中吧它删除.

		git rm 文件名

	2.一次性把工作区与暂存区的文件都删除

		git rm -f 文件名

	3.只删除暂存区,不删除工作区

		git rm --cached 文件名

	4.删除整个文件夹

		git rm -rf 文件名


###	git恢复

	指定文件还原
		git checkout 历史记录编码 文件名(要恢复的文件名)
	回滚历史版本
		git reset --haard HEAD^[1,2,3,4]

	提示：

		如果说 git log 找不到历史ID,
		可以通过 git reflog 去查看操作过的历史记录。

