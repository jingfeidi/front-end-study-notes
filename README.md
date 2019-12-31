# front-end-study-notes
前端学习笔记

## 用Git将本地文件夹上传到GitHub的操作
 ###### 1.在GitHub上新建一个New repository远程仓库后(比如front-end-study-notes)，在本地文件夹里打开命令窗口，将远程仓库克隆到本地：<br>
 ```
 git clone git@github.com:jingfeidi/front-end-study-notes.git
 ```

 ###### 2.进入front-end-study-notes文件夹<br>
 ```
 cd front-end-study-notes 
 ```

 ###### 3.查看工作区和暂存区的当前状态<br>
 ```  
 git status
 ```

 ###### 4.添加文件夹到本地暂存区<br>
  ```
  git add TN-front-end 
  ```

 ###### 把所有修改过的文件全部添加到暂存区<br>
 ```
 git add .
  ```
 ###### 5.提交到本地仓库<br>
 ```
 git commit -m "修改的原因说明"  
 ```

 ###### 6.将本地仓库推送到远程<br>
 ```
 git push git@github.com:jingfeidi/front-end-study-notes.git
 ``` 

 ## 第二天，将本地仓库新增的文件夹上传给远程仓库
 ###### 将远程库与本地同步（如果远程仓库里面有文件等内容需要执行以下这一步）<br>
 ```
 git pull --rebase origin master
 ```
 
 ###### 查看工作区和暂存区的当前状态<br>
 ```
 git status
 ```
 
 ###### 把所有修改过的文件全部添加到暂存区<br>
 ```
 git add .
  ```

 ###### 提交所有更新过的文件<br>
 ```
 git commit -m "commit message"
 ```
 
 ###### 把本地内容推送到远程库 使用 git-push<br>
 ```
 git push -u origin master
 ```
 ```
 或者 git push git@github.com:jingfeidi/front-end-study-notes.git
 ```