# Git合并分支的方法

## Merge

`git merge` 无法保持线性的提交记录，多次`merge`后会出现`git log`很混乱。
用法：

```bash
git merge <source_branch>
```

注：这里需要源分支提交更改后才能被`merge`

### 冲突

#### `mergetool`

当文件存在冲突时，`merge`会被暂停
执行如下命令来使用`mergetool`解决冲突

```bash
git mergetool
```

然后手动解决。

#### 或者

1. 选择取消`merge`，

```bash
git merge --abort
```

2. 手动解决冲突
Git会将冲突写入文件，然后对照，编辑文件。解决冲突后可使用

```bash
git commit
```

或

```bash
git merge --continue # 会检查是否有合并正在进行
```

## Rebase

`git rebase`可以保持线性的提交记录，多数都偏向于使用该命令
执行

```bash
git rebase <target_branch>
```

注：你需要切换到源分支，然后执行以上命令才能将源分支的commit合并到目标分支

## Squash

应该属于`merge/rebase`的一个功能？将多个commit合并为一个commit。

### Merge

执行

```bash
git merge --squash
```

注：这会压缩commit，并不会包含原有的commit历史

> 如果在开发分支上提交非常随意，甚至写成微博体，那么一定要使用--squash选项。版本历史记录的应该是代码的发展，而不是开发者在编码时的活动。

### Rebase

执行

```bash
git rebase -i
```

然后根据打开的文件的注释查看方法
