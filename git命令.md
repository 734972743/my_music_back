git clone 项目地址名称 从服务器上将代码给拉下来

查看类命令

git branch 查看本地所有分支
git status 查看当前状态
git commit 提交
git branch -a 查看所有的分支
git branch -r 查看远程所有分支
查看哪些分支已经合并到当前分支：git branch --merged;
git checkout -b <branch-name> <remote-name>/<branch-name>，如git checkout -b serverfix origin/serverfix 在远程分支的基础上创建新的本地分支
git remote show 查看远程库
git remote show origin 显示远程库origin里的资源
git ls-files 看已经被提交的
git diff 查看尚未暂存的更新
git diff --cached 或 $ git diff --staged 查看尚未提交的更新
git log 查看你的commit的日志
git config --list 查看用户信息
添加类命令

git add . 文件全部添加
git add [file name] 添加一个文件到git index
git checkout [file name] 恢复误删除的文件
新建合并分支类命令

git checkout -b dev 建立一个新的本地分支dev
git checkout dev 切换到本地dev分支
git checkout --track origin/dev 切换到远程dev分支
git merge origin/dev 将分支dev与当前分支进行合并
删除类命令

git branch -D master develop 删除本地库develop

git rm --cached <file> 从暂存区中删除文件，但是工作区依然还有该文件

git rm 文件名(包括路径) 从git中删除指定文件

git rm -f a.a 强行移除修改后文件(从暂存区和工作区中删除)

推送到远端

如果是将本地分支的内容上传到远端服务器，第一次需要使用 git push -u origin branch_name 命令，其中 -u 是 --set-upstream 的缩写。

git push origin master 将文件给推到服务器上

git stash push 将文件给push到一个临时空间中

git stash pop 将文件从临时空间pop下来

修改本地git密码

进入控制面板 -->选择用户账户 -->选择管理你的凭据 -->选择Windows凭据 -->选择git保存的用户信息 -->选择编辑或者进行删除操作 -->完成
