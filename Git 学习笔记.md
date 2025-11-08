## Git 学习笔记（含进阶）

###### 记录人：冯礼盈

##### Git Bash是命令行操作。

### Git定义

##### Git是目前世界上最先进的分布式版本控制系统，是Linus自己用C写的。

### Git作用

##### 可以方便与他人进行合作，可以协同编辑，不用将文件传来传去，每一次改动也可以清晰地查看，相比于集中式版本控制系统，作为分布式的git安全性要高很多，因为每个人电脑上都有完整的版本库，而且不必联网。

### 如何安装和配置Git（以 Windows为例）

##### 1.直接从Git官网下载安装程序 (https://git-scm.com/install/windows) ，然后按默认选项安装即可。若右键可以找到Open Git Bush Here，蹦出命令窗口，则证明安装成功。

##### 2.在使用git前需要配置用户信息，这样才能告诉机器你是谁，才能在协作中知道是谁修改了哪些文件。

##### 设置用户名和邮箱地址 
*$ git config --global user.name "Your Name"*

*$ git config --global user.email "  "*
###### （注意在输入时==前面的空格，一开始因为这个问题始终没有成功，设置时尽量保证与GitHub上一致）

### 仓库设置

##### 1.创建新的本地仓库

#####  选择合适的地方创建空目录。

##### 创建空目录

*$ mkdir learngit*

*$ cd learngit*

*$ pwd*
*/Users/michael/learngit*


###### （注意确保目录名不包含中文，避免不必要的麻烦）

##### 在当前目录下创造一个新的Git仓库。

##### 创造git仓库

*$ git init
Initialized empty Git repository in /Users/michael/learngit/.git/*

###### （注意到.git的目录，不要随意改动）

##### 2.远程仓库

##### 在本地仓库下运行命令：

##### 远程仓库添加

*$ git remote add origin git@github.com:michaelliao/learngit.git*

##### 添加后远程库的名字就是origin，可以用*git push*命令把本地库的内容推送到远程，每次本地提交后可以使用命令git push origin master推送最新修改。如果添加的时候地址写错了，或者就是想删除远程库，可以用git remote rm <name>命令。

##### 用命令*git clone*将远程库克隆一个本地库，可以用ssh，也可以用https。

### 工作区和暂存区

##### 工作区（Working Directory）就是你在电脑里能直接看到的目录。


##### *git add*：将文件修改添加到暂存区。

##### *git commit*：把暂存区的所有内容提交到当前分支。

##### *git status*：查看一下状态。

### 回退、修改、删除

##### *HEAD*：指向当前版本。

##### *$ git reset --hard HEAD*：版本回退。

##### *git log*:命令查看提交历史记录（回退过去）。

##### *git reflog*：查看命令历史（回到未来）。

##### *git checkout -- file*：丢弃工作区的修改（注意--的使用）。


##### *git rm*：删除一个文件。

### 提交方式
##### 除了可以用Git Bash提交外，还可以使用图形化工具以及集成开发环境（IDE）来进行提交，更加清晰方便。
##### 1.TortoiseGit 2，VisualStudioCode（本人目前在用的一款） 3.IntelliJIDEA 等




