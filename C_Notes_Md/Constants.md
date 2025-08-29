这可以固定某个变量的值不被修改，并且是只读的
```c
const int num = 1;
```
然而如果你使用
```c
const int num;
num = 1;
```
这是错误的用法。

**推荐将const的变量全部大写**
如
```c
const int NUM = 1;
```
