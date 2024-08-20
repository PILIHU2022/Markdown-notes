# Git rebase操作
git rebase 命令用于将一个分支上的更改移到另一个分支之上。它可以帮助保持提交历史的线性，减少合并时的冲突。

## 变基当前分支到指定分支
```
git rebase branchname
```
- 交互式变基
```
git rebase -i commit
```
交互式变基允许你在变基过程中编辑、删除或合并提交。常用选项包括：
- pick：保留提交
- reword：修改提交信息
- edit：编辑提交
- squash：将当前提交与前一个提交合并
- fixup：将当前提交与前一个提交合并，不保留提交信息
- drop：删除提交