use_git
=======

使用 Git：专门用于学习和实验的 Git 仓库  

推送数据到远程：`git push origin <local_branch_name>:<remote_branch_name>`  
删除远程分支：`git push origin :dev`  

我的提交策略：  
1、创建并切换到临时分支  

    git checkout -b temp
    等同于：
    git branch temp
    git checkout temp

2、基于分支做修改  
3、提交到本地  

    git add .
    git commit -m '...'  

4、切换到主分支

    git checkout master

5、合并

    git merge temp --no-ff

6、推送到远程（比如：GitHub）

    git push origin master  


