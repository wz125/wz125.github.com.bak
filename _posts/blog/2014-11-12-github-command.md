---
layout: post
title: 'GitHub操作流程'
category: blog
tags: man
---

第一次提交 :  
====
**方案一 : 本地创建项目根目录, 然后与远程GitHub关联, 之后的操作一样;**
 + 初始化git仓库`git init`
 + 提交改变到缓存 : `git commit -m 'description'`
 + 本地git仓库关联GitHub仓库 :` git remote add origin git@github.com:han1202012/TabHost_Test.git `
 + 提交到GitHub中 : `git push -u origin master `

**方案二 : 方案二就是不用关联GitHub仓库, 直接从GitHub冲克隆源码到本地, 项目根目录也不用创建;**
 + 从GitHub上克隆项目到本地 :git clone git@github.com:han1202012/NDKHelloworld.git , 注意克隆的时候直接在仓库根目录即可, 不用再创建项目根目录 ;
 + 添加文件 :`git add ./* `, 将目录中所有文件添加;
 + 提交缓存 :`git commit -m '提交'`
 + 提交到远程GitHub仓库 : `git push -u origin master`
之后修改提交 : 
 + 与GitHub远程仓库同步 : `git pull `
 + 查看文件变更 : ` git status `
 + 提交代码到本地缓存 : `git commit -m 'description'`
 + 提交代码到远程GitHub仓库 : `git push `;

**Git标签操作 : 轻量级标签, 带注释标签;**
--查看标签 :git tag ;
--添加标签 : 轻量级标签git tag tagName , 带注释标签git tag -a tagName -m 'description' ;
--删除标签 :git tag -d tagName ;
--提交标签到GitHub中 : git push origin --tags ;

**Git分支操作: **
创建分支后, 分支操作不会影响master分支, 但是master分支改变会影其它分支;
--列出分支 :git branch ;
--切换分支 :git checkout master ;
--提交分支 : git push origin branchName ;
--删除分支 : git branch -d branchName , 强制删除分支 git branch -D branchName ;
--合并分支 : git merge branchName ;

``` bash
git config --global user.name "wz125" 
git config --global user.email "wzs125@gmail.com

touch README.md  
git init  
git add README.md  
git commit -m "first commit"  
git remote add origin git@github.com:han1202012/TabHost_Test.git 
git push -u origin master 

##Push an existing repository from the command line : 
git remote add origin git@github.com:han1202012/TabHost_Test.git 
git push -u origin master  

```
>[GIT参考手册](http://gitref.org/zh/index.html)
>[help blog](http://blog.csdn.net/vipzjyno1/article/details/22098621)
