# Git reset
语法格式
```
git reset [--soft | --mixed | --hard] [HEAD]
```
## `--mixed`是默认的，可以不用带该参数，用于重置暂存区的文件与上一次的提交(commit)保持一致，工作区文件内容保持不变。
```
git reset HEAD
```
示例
```
$ git reset HEAD^            # 回退所有内容到上一个版本  
$ git reset HEAD^ filename   # 回退某文件的版本到上一个版本  
$ git reset  052e            # 回退到指定版本
```
## `--soft`参数用于回退到某个版本(可用于修改`commit`消息)
```
git reset --soft HEAD # 必须用`HEAD`! 否则会回退失败
```

## `--hard` 参数撤销工作区中所有未提交的修改内容，将暂存区与工作区都回到上一次版本，并删除之前的所有信息提交：
```
git reset --hard HEAD~3           # 回退上上上一个版本  
git reset –hard bae128            # 回退到某个版本回退点之前的所有信息。 
git reset --hard origin/master    # 将本地的状态回退到和远程的一样 
```
*注意：谨慎使用 –-hard 参数，它会删除回退点之前的所有信息。*

## HEAD 说明：
```
HEAD 表示当前版本
HEAD^ 上一个版本
HEAD^^ 上上一个版本
HEAD^^^ 上上上一个版本
以此类推...
```

可以使用 ～数字表示
```
HEAD~0 表示当前版本
HEAD~1 上一个版本
HEAD^2 上上一个版本
HEAD^3 上上上一个版本
以此类推...
```
