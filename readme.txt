git init 初始化git仓库

add 添加
commit 提交       提交时要写一段描述！！！！
git status命令可以让我们时刻掌握仓库当前的状态
git diff顾名思义就是查看difference

用cat 来显示内容
	例如：cat readme.txt

git利用指针，快速实现版本退回
git log 查看各次操作
	head为当前版本，上一版本为head^......以此类推
git reset命令退回前面的版本
	例如：git reset --hard HEAD^
git reflog用来记录你的每一次命令，以便“回到未来”

git checkout -- file  可以丢弃工作区的修改   （）
命令git checkout -- readme.txt意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
总之，就是让这个文件回到最近一次git commit或git add时的状态。
git checkout -- file命令中的--很重要，没有--，就变成了“切换到另一个分支”的命令

git reset HEAD <file>可以把暂存区的修改撤销掉（unstage），重新放回工作区
git reset命令既可以回退版本，也可以把暂存区的修改回退到工作区。当我们用HEAD时，表示最新的版本。