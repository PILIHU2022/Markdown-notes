# Git Reset
`reset`用于更新你的分支，移动tip来实现从`branch`中添加或移除`commit`。这个操作将改变`commit`历史。也适用于恢复暂存区，与`git restore`类似。

# Git restore
`restore`用于还原从暂存区或其他`commit`中还原工作区的文件。这个命令不会更新你的分支。这个命令也可以用于从其他`commit`还原暂存区的文件。
# Git Revert
`revert`是一个通过创建一个新的`commit`来恢复通过其他`commit`所制造的变化。