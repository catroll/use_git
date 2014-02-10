Use Git  
=======  
  
使用 Git：专门用于学习和实验的 Git 仓库  
  
### 开始  
  
**初始化版本库**  
  
    git init  
  
**Clone 版本库**  
默认就是关联到 origin 分支。  
  
    git clone <remote_repo_address>  
  
### 修改与提交  
  
**添加**  
  
    git add <file_name>  
    git add .  
    git add -u  
  
**删除**  
  
    git rm <file_name>  
  
如果不想删除文件，只是不再跟踪，可以使用 -cached 参数。  
  
**重命名**  
  
    git mv <old_file_name> <new_file_name>
  
**提交**  
  
    git commit -m "some comments"  
  
### 推送（push）与获取（pull）  
  
**推送数据到远程**  
  
    git push <remote_repo_name> <local_branch_name>:<remote_branch_name>  
  
如果不填本地分支名称就表示删除远程分支，如：  
  
    git push origin :dev  
  
### 远程  
  
**显示远程版本库列表**  
  
    git remote -v  
  
**添加远程版本库**  
  
    git remote add <remote_repo_name> <remote_repo_address>  
  
### 分支  
  
**显示分支列表**  
  
    git branch -r（远程）  
    git branch -l（本地，默认）  
  
**分支切换**  
  
    git checkout <local_branch_name>  
  
如果加上一个 -b 参数可以实现如果分支不存在就按照指定名称创建一个的效果。  
  
### 其他  
  
    查看历史记录：`git log`  
  
    修改最后一次的提交记录：`git commit --amend`  
  
我的提交策略  
=======  
  
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
  
  
