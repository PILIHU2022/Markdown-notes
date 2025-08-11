# Git reset

## reset有三种模式，`soft`,`mixed`,`hard`。然而，这三种模式都是将HEAD（commit后）移动到commit之前。

`--soft` 不会更改`工作区`和`暂存区`的对应文件，仅仅是将文件状态从HEAD转移到待commit状态。（可用于更改commit消息）

`--mixed` 直接将文件从HEAD转移至未暂存状态，这可以允许你将前一个commit更改的文件更新再commit。（无冲突时）

`--hard` **高危** 会将对应文件直接恢复至commit时的状态，在commit之后的状态都会被删除！！！

### 同理，可用于更改commit消息或者对commit后未push的文件进行修改。

```Bash
git reset --soft HEAD~1 # 将HEAD中的文件状态更改为未提交
git reset --soft HEAD~2 # 直接将HEAD中的文件状态更改为未暂存
```

同样的，你也可以使用`--mixed`

```Bash
git reset --mixed HEAD~1 #直接将HEAD中的文件状态更改为未暂存
```

#### commit后未push

```Bash
git reset --soft HEAD~1
```

#### commit且push

没救了 
