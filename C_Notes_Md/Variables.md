## 声明
声明变量,如下:
```c
int num; // num为变量名,变量名不可是C语言中的关键字
num = 1; // 给变量赋值
```
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
### char
存储**单个**字符，如`a`、`b`，应当使用`''`包裹
```c
char a = 'a' //字符
```

## 调用
### 用于整数类
```c
printf("%d",var_name)
```
### 用于浮点数
```c
printf("%f",var_name)
```
### 用于double
```c
printf("%lf",var_name)
```
### 用于char
```c
printf("%c",var_name)
```
