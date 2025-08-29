# 引号
## 双引号
一般来说，都是要用双引号的
```diff
#include <stdio.h>
int main() {
+ printf("Hello! C-lang");
- printf('Hello! C-lang');
  return 0;
}
```
如上，有双引号的不会报错

## 单引号
一般是用于类型为`char`的单个字符
```C
#include <stdio.h>
int main() {
  char a = 'a';
  printf("%c", a);
  return 0;
}
```
