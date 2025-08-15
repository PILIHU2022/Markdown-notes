# HEAD
`HEAD` 是一个对当前commit的象征化的名字。其本质上是你在它之上工作的commit，它总是指向最近的commit。
通常`HEAD`是指向分支名的。当你commit的时候，分支的状态已经改变，并且可以通过`HEAD`可视化该变化。

## 移动
### `^`
```bash
git reset HEAD^ #向上移动一个commit。
git reset HEAD^^ #向上移动两个commit。
...
```
### `~`
后面可加入数字
```bash
git reset HEAD~num
```
