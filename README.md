# play gitflow 分支测试
wahahahahsadasdasdasdasda
asd
as
da
sd
asd
feature start
第一次

git branch（分支命令的使用
http://hbiao68.iteye.com/blog/2055493

 

0.可以通过git branch -r 命令查看远端库的分支情况

 

1,从已有的分支创建新的分支(如从master分支),创建一个dev分支

git checkout -b dev

2,创建完可以查看一下,分支已经切换到dev

git branch

    * dev

    master

3.建立本地到上游（远端）仓的链接 --这样代码才能提交上去

git branch --set-upstream-to=origin/dev 

取消对master的跟踪

git branch --unset-upstream master

 

git 创建分支提交远程分支 - oppotvr
https://my.oschina.net/u/219482/blog/285584

 

以下两个应该是同一个意思，=upstream : 上游码流的意思
git branch --set-upstream-to=master
git branch --set-upstream-to=original/master


git help branch
git branch [--set-upstream | --track | --no-track] [-l] [-f] <branchname> [<start-point>]
git branch (--set-upstream-to=<upstream> | -u <upstream>) [<branchname>]
git branch --unset-upstream [<branchname>]

git branch --set-upstream-to=original/master new
git branch --set-upstream debug origin/debug //其中debug为创建的分支

 

提交该分支到远程仓库
git push origin dev

将develop分支的代码同步到private，步骤：

git checkout private

git merge develop

git push