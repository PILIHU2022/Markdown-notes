# Git分区有“工作区”“暂存区(index)”“本地仓库”

## 工作区

你工作的文件夹，在里面写代码

### 暂存区(index)

在工作区执行

```Bash
git add <file>
```

后文件状态，已被暂存。

### 本地仓库

在文件被暂存后，执行

```Bash
git commit -m '<message>'
```

文件就会进入到本地的仓库，后续可执行

```Bash
git push <remote> <branch>
```

以提交至远程仓库。