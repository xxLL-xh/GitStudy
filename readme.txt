git init 初始化git仓库

add 添加
commit 提交       提交时要写一段描述！！！！
git status命令可以让我们时刻掌握仓库当前的状态
git diff顾名思义就是查看difference


git利用指针，快速实现版本退回
git log 查看各次操作
	head为当前版本，上一版本为head^......以此类推
git reset命令退回前面的版本
	例如：git reset --hard HEAD^
git reflog用来记录你的每一次命令，以便“回到未来”

