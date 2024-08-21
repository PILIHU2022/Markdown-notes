# Git 的工作区、暂存区和版本库
- 工作区：电脑中可看到的目录
- 暂存区：名为`stage`或`index`，有时也被称为索引(index)
- 版本库：工作区目录中的`.git`，这不算工作区，而是Git的版本库

# 工作区（Working Directory）
工作区是你在本地计算机上的项目目录，你在这里进行文件的创建、修改和删除操作。工作区包含了当前项目的所有文件和子目录。
特点：
- 显示项目的当前状态。
- 文件的修改在工作区中进行，但这些修改还没有被记录到版本控制中。

# 暂存区（Staging Area）
暂存区是一个临时存储区域，它包含了即将被提交到版本库中的文件快照，在提交之前，你可以选择性地将工作区中的修改添加到暂存区。
特点：
暂存区保存了将被包括在下一个提交中的更改。
你可以多次使用 git add 命令来将文件添加到暂存区，直到你准备好提交所有更改。

常用命令：
```
git add filename       # 将单个文件添加到暂存区
git add .              # 将工作区中的所有修改添加到暂存区
git status             # 查看哪些文件在暂存区中
```

# 版本库（Repository）
版本库包含项目的所有版本历史记录。
每次提交都会在版本库中创建一个新的快照，这些快照是不可变的，确保了项目的完整历史记录。
特点：
版本库分为本地版本库和远程版本库。这里主要指本地版本库。
本地版本库存储在 .git 目录中，它包含了所有提交的对象和引用。
常用命令：
```
git commit -m "Commit message"   # 将暂存区的更改提交到本地版本库
git log                          # 查看提交历史
git diff                         # 查看工作区和暂存区之间的差异
git diff --cached                # 查看暂存区和最后一次提交之间的差异
```

# 工作区、暂存区和版本库之间的关系
## 1、工作区 -> 暂存区
使用 git add 命令将工作区中的修改添加到暂存区。
```
git add filename
```
## 2、暂存区 -> 版本库

使用 git commit 命令将暂存区中的修改提交到版本库。
```
git commit -m "Commit message"
```
## 3、版本库 -> 远程仓库

使用 git push 命令将本地版本库的提交推送到远程仓库。
```
git push origin branch-name
```
## 4、远程仓库 -> 本地版本库
使用 git pull 或 git fetch 命令从远程仓库获取更新。
```
git pull origin branch-name
# 或者
git fetch origin branch-name
git merge origin/branch-name
```

# 查看版本
使用
```
git log
```
即可

# 学习资料
[廖雪峰的网站](https://liaoxuefeng.com/)
[Git游戏](https://learngitbranching.js.org/?locale=zh_CN)
[菜鸟教程](https://www.runoob.com/git/git-tutorial.html)
[Git官方文档](https://git-scm.com/docs)
[中文版ProGit](https://www.progit.cn/)
[英文版ProGit](https://git-scm.com/book)
[Git高级操作，疑难杂症](https://ohshitgit.com/zh)