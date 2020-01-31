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

4. 工作区与暂存区、仓库对比变化
$ git diff readme.txt
$ git diff HEAD -- readme.txt

5. 添加到暂存区
$ git add readme.txt

6. 提交暂存区所有修改到仓库
$ git commit -m "added the readme.txt"

7. 查看提交记录
$ git log

8. 查看所有仓库修改记录
$ git reflog

9. 本地仓库版本重置(HEAD仓库最新版本，HEAD^上一版本，HEAD^^上上版本，HEAD~10上10个版本，
还可指定版本号)
$ git reset --hard HEAD^
$ git reset --hard 308a216

10. 打回暂存区文件所有修改到工作区
$ git reset HEAD readme.txt

11. 撤销工作区文件所有修改（替换、工作区文件删除还原）,回到最近一次git add或git commit
$ git checkout -- readme.txt

12. 删除文件(工作区删除、暂存区删除、本地仓库删除)
$ rm test.txt
$ git rm test.txt
$ git commit -m "remove test.txt"
