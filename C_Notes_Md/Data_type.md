## 类型
### int
整数类，全部都是数字，与`Python`类似
```c
int num = 123 //整数类
```
### float
浮点数，含小数点，与`Python`类似
```c
float num = 12.3 //浮点数
```
### double
与`float`类似，但更精确，可有15位小数
```c
double num = 123.324454
```
### 其中，`float`和`double`类型都是可以使用`.`来指定显示到几位数。如：

```c
printf("%.1f",num)
printf("%.1lf",num)
```

### char

存储**单个**字符，如`a`、`b`，应当使用`''`包裹
```c
char a = 'a' //字符
```
### strings
存储字符串
```c
char text[] = "Hello"
```

## 调用
### 用于整数类
```c
printf("%d",var_name)
```
或
```c
printf("%d",123)
```
### 用于浮点数
```c
printf("%f",var_name)
```
或
```c
printf("%f",12.3)
```
### 用于double
```c
printf("%lf",var_name)
```
或
```c
printf("%lf",12.3)
```
### 用于char
```c
printf("%c",var_name)
```
或
```c
printf("%c",'D')
```
### 用于string
```c
printf("%s",var_name)
```
或
```c
printf("%s","Hello")
```
## 查看数据大小
使用
```c
printf("%zu",sizeof(var_name))
```
这个可以帮助你预估程序所需的运行内存
