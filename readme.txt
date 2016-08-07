推荐！手把手教你使用Git http://blog.jobbole.com/78960/

在被 git 管理的目录中删除文件时，可以选择如下两种方式来记录删除动作：
一、rm + git commit -am "abc"
二、git rm + git commit -m "abc"
另外，git add . 仅能记录添加、改动的动作，删除的动作需靠 git rm 来完成。
最后，rm 删除的文件是处于 not staged 状态的，
也就是一种介于 “未改动” 和 “已提交过” 之间的状态。


git checkout . #本地所有修改的。没有的提交的，都返回到原来的状态
git stash #把所有没有提交的修改暂存到stash里面。可用git stash pop回复。
git reset --hard HASH #返回到某个节点，不保留修改。
git reset --soft HASH #返回到某个节点。保留修改


一般 git clean都是配合git reset 使用的 
如果你有的修改以及加入暂存区的话 
那么 
git reset --hard 
git clean -xdf 
如果没有加入暂存区的话 git checkout . && git clean -xdf


git checkout -f //checkout该文件所有的文件