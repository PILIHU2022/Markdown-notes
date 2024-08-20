# Git revert操作
<!-- `revert`是一个当我们想使用上一个`commit`并且添加它作为一个新的`commit`，保持`log`的完整 -->
`git revert` 通过创建一个新的提交来撤销旧提交，同时保留项目的提交历史。

## 注意
如果你想丢弃工作目录中所有未提交的更改，请参阅[[Reset]]
## 语法
```
git revert [--[no-]edit] [-n] [-m <parent-number>] [-s] [-S[<keyid>]] <commit>

git revert (--continue | --skip | --abort | --quit)
```
