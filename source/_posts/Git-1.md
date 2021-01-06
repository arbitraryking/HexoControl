---
title: Git_1
date: 2021-01-06 16:51:46
tags: [Git,Tutorial]
---
# Basic Git operations in Git bash
## 使用本地文件生成git库
在当前文件夹<br>
`$ git init //初始化后生成.git
 $ git add . //添加文件到暂存区
 $ git commit`

## 本地代码库上传到远程代码服务器
`$ git remote add origin 库地址`
第一次推送<br>
`$ git push -u origin master`
后续推送<br>
`$ git push origin master`

查看当前git状态<br>
`$ git status`    
暂存修改<br>
`$ git add <file/dir>`    
取消暂存文件<br>
`$ git reset HEAD <file>`    
提交修改<br>
`$ git commit -a -m 'description of this commit'`    
`$ git commit --amend //提交暂存代替上一次的提交`    

## 移除文件
`$ git rm //从工作目录删除文件，并从暂存区移除`    
`$ git rm -f //文件已经被修改过或已放到暂存区`    
`$ git rm --cached //从Git仓库中抹去，但本地文件夹中留下`    

## 分支
分支创建<br>
`$ git branch branch_name`    
分支切换<br>
`$ git checkout branch_name`    
分支创建并切换(尽可能保证分支处于干净状态)<br>
`$ git commit`    
`$ git checkout -b branch_name`    
删除分支(删除失败使用 -D 强制删除)<br>
`$ git branch -d branch_name`    
分支合并<br>
`$ git checkout branch_name //合并后保留的分支`    
`$ git merge branch2bmerge`    
