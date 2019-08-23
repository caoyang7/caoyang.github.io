---
layout: post
title: "ProGit_test"
date: 2019-8-19 13:26:40
image: 'http://imgcdn.sdk.cn/article/_Yje2_hCmxAOUVmzZdKh.jpg'
description: progit考试
category: 'blog'
tags:
- 考试
- Git
introduction: progit考试
---

# Git考试 

1. 创建文件夹“兄弟会”  
ttk@ttk-X6Ti-Series-GH5KN51:~$ mkdir 兄弟会  

2. 查看列表  
ttk@ttk-X6Ti-Series-GH5KN51:~$ ls  
examples.desktop  ttk1907.github.io  曹小羊  公共的  模板  视频  图片  文档  下载  小明同学  兄弟会  音乐  桌面  

3. 进入文件夹“兄弟会”  
ttk@ttk-X6Ti-Series-GH5KN51:~$ cd 兄弟会  

4. 初始化  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git init  
已初始化空的 Git 仓库于 /home/ttk/兄弟会/.git/  

5. 创建文件  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ touch 2019-08-21-kaoshi.md  

6. 编辑文件  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ vi 2019-08-21-kaoshi.md  

7. 追踪文件   
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git add 2019-08-21-kaoshi.md  

8. 提交文件   
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git commit 2019-08-21-kaoshi.md   
[master （根提交） 38cf969] day8 ribao  
 1 file changed, 2 insertions(+)  
 create mode 100644 2019-08-21-kaoshi.md  

9. 查看状态  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git status  
位于分支 master  
无文件要提交，干净的工作区  

10. 创建远程库“兄弟会”ssh  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote add 兄弟会 git@github.com:ttk1907/github.git  

11. 查看远程仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote -v  
兄弟会	git@github.com:ttk1907/github.git (fetch)  
兄弟会	git@github.com:ttk1907/github.git (push)  

12. 创建远程仓库“兄弟会nb”http  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote add 兄弟会nb https://github.com/ttk1907/github.git  

13. 查看远程仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote -v  
兄弟会	git@github.com:ttk1907/github.git (fetch)  
兄弟会	git@github.com:ttk1907/github.git (push)  
兄弟会nb	https://github.com/ttk1907/github.git (fetch)  
兄弟会nb	https://github.com/ttk1907/github.git (push)  

14. 创建分支test  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git branch test  

15. 查看分支  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git branch  
* master  
  test  

16. 切换到test分支  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git checkout test  
切换到分支 'test'  

17. 修改文件名  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git mv 2019-08-21-kaoshi.md 2019-08-21-kaoshi-test.md  

18. 把test分支推到远程库的test分支，冒号是新建的意思   
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git push -u 兄弟会 test:test  
^[[A对象计数中: 3, 完成.  
写入对象中: 100% (3/3), 248 bytes | 248.00 KiB/s, 完成.  
Total 3 (delta 0), reused 0 (delta 0)  
To github.com:ttk1907/github.git  
 * [new branch]      test -> test  
分支 'test' 设置为跟踪来自 '兄弟会' 的远程分支 'test'。  

19. 切换到master分支  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git checkout master  
A	2019-08-21-kaoshi-test.md  
D	2019-08-21-kaoshi.md  
切换到分支 'master'  

20. 把test分支拉到兄弟会仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git fetch 兄弟会 test  
来自 github.com:ttk1907/github  
 * branch            test       -> FETCH_HEAD    

21. 查看差异  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git diff test  
diff --git a/2019-08-21-kaoshi.md b/2019-08-21-kaoshi-test.md  
similarity index 100%  
rename from 2019-08-21-kaoshi.md  
rename to 2019-08-21-kaoshi-test.md  

22. 合并test到兄弟会仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git merge 兄弟会/test  
已经是最新的。  

23. 把master分支推到兄弟会仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git push -u 兄弟会 master  
Total 0 (delta 0), reused 0 (delta 0)  
remote:   
remote: Create a pull request for 'master' on GitHub by visiting:  
remote:      https://github.com/ttk1907/github/pull/new/master  
remote:   
To github.com:ttk1907/github.git  
 * [new branch]      master -> master  
分支 'master' 设置为跟踪来自 '兄弟会' 的远程分支 'master'。  

24. 创建标签  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git tag v1.0  

25. 把v1.0标签推到兄弟会仓库    
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git push -u 兄弟会 v1.0  
Total 0 (delta 0), reused 0 (delta 0)  
To github.com:ttk1907/github.git  
 * [new tag]         v1.0 -> v1.0  

26. 查看远程仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote -v  
兄弟会	git@github.com:ttk1907/github.git (fetch)  
兄弟会	git@github.com:ttk1907/github.git (push)  
兄弟会nb	https://github.com/ttk1907/github.git (fetch)  
兄弟会nb	https://github.com/ttk1907/github.git (push)  

27. 创建工作区分支并切换到
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git checkout -b 工作区  
A	2019-08-21-kaoshi-test.md  
D	2019-08-21-kaoshi.md  
切换到一个新分支 '工作区'  

28. 编辑文件  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ vi 2019-08-21-kaoshi-test.md  

推上去  

29. 创建标签v2.0   
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git tag v2.0  

30. 追踪  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git add .  

31. 提交  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git commit -m"sdg"  
[工作区 a13daaf] sdg  
 2 files changed, 3 insertions(+), 2 deletions(-)  
 create mode 100644 2019-08-21-kaoshi-test.md  
 delete mode 100644 2019-08-21-kaoshi.md  

32. 推到远程库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git push -u 兄弟会 v2.0  
^[Total 0 (delta 0), reused 0 (delta 0)  
To github.com:ttk1907/github.git  
 * [new tag]         v2.0 -> v2.0  

33. 查看提交历史  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git log  
commit a13daaf00ab9f007f2702d0eb840e404973f74ad (HEAD -> 工作区)  
Author: ttk1907 <ttk1907@163.com>  
Date:   Wed Aug 21 14:37:00 2019 +0800

    sdg  

commit 38cf969f3b2a46a3057b5f9accd2e448a4fbb472 (tag: v2.0, tag: v1.0, 兄弟会/test, 兄弟会/master, test, master)  
Author: ttk1907 <ttk1907@163.com>  
Date:   Wed Aug 21 14:12:23 2019 +0800  

    day8 ribao  

34. 版本回退  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git reset --hard 38cf969f3b2a46a3057b5f9accd2e448a4fbb472  
HEAD 现在位于 38cf969 day8 ribao  

35. 查看分支  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git branch  
  master  
  test  
* 工作区  

36. 在兄弟会仓库新建回滚分支，并把工作区推上去  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git push -u 兄弟会 工作区:回滚  
Total 0 (delta 0), reused 0 (delta 0)  
remote:   
remote: Create a pull request for '回滚' on GitHub by visiting:  
remote:      https://github.com/ttk1907/github/pull/new/%E5%9B%9E%E6%BB%9A  
remote:   
To github.com:ttk1907/github.git  
 * [new branch]      工作区 -> 回滚  
分支 '工作区' 设置为跟踪来自 '兄弟会' 的远程分支 '回滚'。  

37. 编辑文件  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ vi 2019-08-21-kaoshi-test.md  

38. 撤销修改  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git checkout .

39. 删除兄弟会仓库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote rm 兄弟会  

40. 查看库  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git remote -v  
兄弟会nb	https://github.com/ttk1907/github.git (fetch)  
兄弟会nb	https://github.com/ttk1907/github.git (push)  

41. 修改注释  
ttk@ttk-X6Ti-Series-GH5KN51:~/兄弟会$ git commit --amend  
[工作区 4d6fa23] day8 ribao  lalalala
 Date: Wed Aug 21 14:12:23 2019 +0800
 1 file changed, 2 insertions(+)
 create mode 100644 2019-08-21-kaoshi.md



 