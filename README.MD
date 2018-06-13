
# git常用命令以及GitHub的使用

**1.新建远程仓库，包含readme文件，如何把本地内容放进去？** 
1.创建本地仓库：git init（这时候是空的）  
2.关联远程仓库：git remore add origin git@github.com:jingpingyi/how-to-use-git.git  
3.git pull origin master把远程仓库中的内容拉下来（第一次使用git pull需要添加origin master）  
4.本地文件复制到本地仓库中 

> 可能遇到的问题：
1. 本地仓库中如果先有内容再pull，会失败。因为两个不相关的branch不能merge。根本原因是远程和本地不能有两个不相关的branch。所以也可以先建立远程的空仓库然后push本地的文件。这样都只会有一个branch存在。  
2. 删除远程仓库：git remote remove origin  
3. 查看远程仓库：git remote -v 

