# 从一个commit中恢复特定文件
`--source=<commit_id>` 将某个commit作为源来恢复文件
`--staged` 指定该option将会仅仅恢复暂存区
若`--worktree`和`--staged`都不指定，则是将工作区中的指定文件还原，默认是将工作区的文件还原至**暂存区对应文件的内容**

**注：**若恢复一个文件夹，文件夹结构和文件状态如下：
```
1
├── test_2.py # 被跟踪，已编辑
├── test_1.py # 未跟踪，已编辑
└── test.py # 被跟踪
```
若你将`test_1.py`跟踪，然后执行`git restore --source=<commit_id> 1`，若commit中并没有`test_1.py`，那么它将会删除`test_1.py`，并且你执行`git restore --staged test_1.py`是无法恢复`test_1.py`的
