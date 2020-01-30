Git 介绍
Git is a version control system.
Git is a free software.

安装完Git后
1. 打开git bash
$ git config --global user.name "windlike"
$ git config --global user.email "windlike@example.com"
2. 新建一个目录并且cd到该目录，将该目录初始化为git目录
$ git init
3. 查看git状态
$ git status
4. 与暂存区对比变化
$ git diff readme.txt
5. 添加到暂存区
$ git add readme.txt
6. 提交暂存区所有修改到仓库
$ git commit -m "added the readme.txt"
7. 查看提交记录
$ git log
8. 查看所有仓库修改记录
$ git reflog
9. 版本重置(HEAD仓库最新版本，HEAD^上一版本，HEAD^^上上版本，HEAD~10上10个版本，
还可指定版本号)
$ git reset --hard HEAD^
$ git reset --hard 308a216
