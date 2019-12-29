# front-end-study-notes
前端学习笔记

# Git简单操作
1.在GitHub上新建一个New repository远程仓库后(比如front-end-study-notes)，在本地文件夹里打开命令窗口，将远程仓库克隆到本地：
git clone git@github.com:jingfeidi/front-end-study-notes.git

#2.进入front-end-study-notes文件夹
cd front-end-study-notes 

#3.查看工作区和暂存区的当前状态
git status

#4.添加文件到本地暂存区
git add TN-front-end 

或者添加到本地暂存区
git add .

#5.提交到本地仓库
git commit -m "修改的原因说明"  

#6.将本地仓库推送到远程
git push git@github.com:jingfeidi/front-end-study-notes.git

