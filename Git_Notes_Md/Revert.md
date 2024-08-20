# Git revert操作
<!-- `revert`是一个当我们想使用上一个`commit`并且添加它作为一个新的`commit`，保持`log`的完整 -->
`git revert` 通过创建一个新的提交来撤销旧提交，同时保留项目的提交历史。用于还原一些现有的提交。
## 语法
```
git revert [--[no-]edit] [-n] [-m <parent-number>] [-s] [-S[<keyid>]] <commit>

git revert (--continue | --skip | --abort | --quit)
```
## 注意
如果你想丢弃工作目录中所有未提交的更改，请参阅[[Reset]]
## 使用须知
- `revert`需要给定一个或多个存在的`commit`，来恢复到相关补丁引进的改变。然后记录一些新的`commit`来记录它们
- 你需要一个干净的工作区（在HEAD的`commit`中没有修改）
- `revert`是用于记录一些新的提交，来重置之前的提交（通常是错误的提交）