---
layout: post
title: "ProGit"
date: 2019-8-19 13:26:40
image: 'http://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_760/v1504807239/morpheus_xdzgg1.jpg'
description: 相信你能做好，你就能做好！
category: 'blog'
tags:
- 版本控制
- Git分支
introduction: 2019年8月15日上午11点，我正式加入了兄弟会。喜欢C罗，始于自律，忠于坚定！要做一个像他一样的人啊！
---
 
### 一、开始一个工作区（参见：git help tutorial）  

1. `clone`      克隆仓库到一个新目录
	- $ git clone https://github.com/caoyang7/caoyang7.github.io
2. `init`       创建一个空的 Git 仓库或重新初始化一个已存在的仓库
	- $ git init


### 二、在当前变更上工作（参见：git help everyday）  

1. `add`        添加文件内容至索引
	- $ git add *.c
	- $ git add README
	- $ git add .
	- $ git remote add pb git://github.com/paulboone/ticgit.git
	- $ git add README test.rb LICENSE
	- $ git remote add local_proj /opt/git/project.git
	- $ sudo adduser git
	- $ git remote add origin git@gitserver:/opt/git/project.git
	- git daemon --reuseaddr --base-path=/opt/git/ /opt/git/
	- git add --patch
	- git commit -am 'add reset task'
	- $ git remote add myfork (url)
2. `mv`         移动或重命名一个文件、目录或符号链接
3. `reset`      重置当前 HEAD 到指定状态
4. `rm`         从工作区和索引中删除文件


### 三、检查历史和状态（参见：git help revisions）  

1. `bisect`     通过二分查找定位引入 bug 的提交
2. `grep`       输出和模式匹配的行
3. `log`        显示提交日志
4. `show`       显示各种类型的对象
5. `status`     显示工作区状态


### 四、扩展、标记和调校您的历史记录  

1. `branch`     列出、创建或删除分支
2. `checkout`   切换分支或恢复工作区文件
3. `commit`     记录变更到仓库
4. `diff`       显示提交之间、提交和工作区之间等的差异
5. `merge`      合并两个或更多开发历史
6. `rebase`     在另一个分支上重新应用提交
7. `tag`        创建、列出、删除或校验一个 GPG 签名的标签对象


### 五、协同（参见：git help workflows）  

1. `fetch`      从另外一个仓库下载对象和引用
2. `pull`       获取并整合另外的仓库或一个本地分支
3. `push`       更新远程引用和相关的对象


命令 `git help -a` 和 `git help -g` 显示可用的子命令和一些概念帮助。
查看 `git help <命令>` 或 `git help <概念>` 以获取给定子命令或概念的
帮助。


#### 详情请见: [progit](https://gitee.com/progit/) 