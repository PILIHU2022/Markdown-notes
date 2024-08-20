# Git restore操作
用于恢复或撤销对文件的更改，可以用于恢复工作区、暂存区中的文件，也可以用于丢弃未提交的更改。
## 恢复暂存区的文件到工作区
```
git restore filename
```
## 从指定提交恢复文件
从某个提交（例如 HEAD\~1）中恢复文件：
```
git restore --source=HEAD~1 file.txt
```
*注：会丢弃工作区中未提交的改动*
## 丢弃未提交的更改
```
git restore --staged filename
```