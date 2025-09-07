# C语言判断
## if
示例
```C
#include <stdio.h>

int main() {
  int a = 10;
  if (a < 20) {
    printf("a < 20\n");
  }
  printf("value: %d", a);
  return 0;
}
```

```C
if(<条件>)
{
  ...
}
```

### else
示例
```C
#include <stdio.h>

int main() {
  int a = 30;
  if (a < 20) {
    printf("a < 20\n");
  } else {
    printf("value: %d", a);
  }
  return 0;
}
```

```C
if(<条件>)
{
  ...
}
else if(<条件>)
{
  ...
}
else
{
  ...
   }
```

## switch
switch 语句是一种有限制的控制流语句，它用于根据表达式的值执行不同的代码块。

一个 switch 语句允许测试一个变量等于多个值时的情况，每个值称为一个 case，且被测试的变量会对每个 switch case 进行检查。

示例
```C
#include <stdio.h>

int main() {
  int a = 30;
  switch (a) {
    case 20:
    printf("Value is 20");
    case 30:
    printf("Value is 30");
  }
  return 0;
}
```

```C
switch(...){
  case ...:
    ...
  case ...:
    ...
}
```
