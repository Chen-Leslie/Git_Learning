Git常用命令

- git常用命令

  - git config -global user.name <username> 		设置用户签名
  - git config -global user.email <email>                 设置用户签名
  - git init                                                                          初始化本地库
  - git status                                                                      查看本地库状态
  - git add <fileName>                            将本地库内容添加至暂存区
  - git rm --cache <fileName>                          从暂存区中删除文件
  - git commit -m "日志信息" <fileName>  从暂存区提交到本地库
  - git reflog                                                              查看简要日志
  - git log                                                                   查看详细日志
  - git reset --hard <版本号>                                 回滚版本

- git分支操作

  - git branch -v										查看分支
  - git branch <branchName>              创建分支
  - git checkout <branchName>          切换分支
  - git merge <branchName>          把指定的分支合并到当前分支
  - 正常合并 git merge <branchName>
  - 冲突合并 
    - git merge <branchName>
    - 手动修改冲突内容
    - 添加到暂存区
    - 执行提交(此时git commit不能带文件名)

- git删除操作

  - rm    														删除工作区文件
  - git add <fileName>                           添加到暂存区
  - git commit                                             提交到本地库

  ​	删除的文件未修改，与当前版本库文件内容相同

  - git rm 												删除工作区文件并放入暂存区
  - git commit 

  ​	删除的文件已经修改过，即与当前版本库文件内容不相同

  - git rm -f					删除工作区和暂存区文件，并放入暂存区
  - git commit

- git远程仓库操作

  - git remote -v 			查看当前所有远程地址别名
  - git remote add <alies>  <remoteAddress>  起别名
  - git push <alies> <branchName>  推送本地分支上的内容到远程仓库
  - git clone <remoteAddress> 将远程仓库的内容克隆到本地
  - git pull <remoteAddress> <remoteBranchName>  将远程仓库对于分支最新内容拉下来后与当前本地分支直接合并









