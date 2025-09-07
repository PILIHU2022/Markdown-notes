# 循环
## while
示例
```C
#include <stdio.h>

int main() {
  int a = 1;
  while (a == 1) {
    printf("A == 1");
  };
  return 0;
}
```

```C
while (<条件>) {
  ...
}
```

## for
示例
```C
#include <stdio.h>

int main() {
  int a = 1;
  for (; a <= 10; a++) {
    printf("a == 1");
  }
  return 0;
}
```

```C
for ( <定义值>; <条件>; <增量> )
{
  ...
}
```

注：定义值可以省略，仅仅只需要将`;`保留，同理，增量也可以省略
如：
```C
for (; <条件>;)
```

## do...while
示例
```C
#include <stdio.h>

int main() {
  int a = 1;
  do {
    printf("Value: %d\n", a);
    a += 1;
  } while (a < 10);
  return 0;
}
```

```C
do {
  ...
}while(<条件>)
```
先执行`do {}`中的代码块，然后再`while`判断是否符合条件，若符合则继续执行`do {}`中的代码，若不符合，则下一步

形象的表达：
> while:
> 你欠我钱，我走路上，前面一人，我先看清楚这个人是不是你，不是就不打。
> do...while:
> 你欠我钱，我走路上，前面一人，我不管这个人是不是你，先打再说。
