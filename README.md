# Git使用方法

在github上创建项目，拿到地址，然后clone到本地



设置用户名和邮箱地址。这两个值是作为上传时记录的值。输入命令：
git config --global user.name "用户名"
git config --global user.email "邮箱"
查看目前设置可以用：git config --global user.name



## 初始化本地仓库：git init
此目录下会创建一个.git的文件（此文件可能会隐藏，笔者是windows8.1系统，该文件就隐藏，还以为没有生成）
## 将原有的项目文件放在该目录下，然后将该项目纳入.git版本控制中
git add . (一定要注意add和.之间是有空格的，否则会报错的)
## 将所有更改放到本地暂存区域，等待上传。
git commit -m "此次上传的说明"（对自己的项目做一些说明）
## 连接远程仓库
git remote add origin "https://github.com/GitHub用户名/代码仓库名称.git"
可以通过git remote -v 查看本地链接到的远程仓库
## 从远程仓库拉取所有更新（每次上传项目都要操作）
git pull origin master
## 将本地的更新上传至代码仓库
git push origin master


