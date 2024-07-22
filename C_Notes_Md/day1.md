# 学习C语言第一天
## printf
printf是一个打印命令,这类似于Python的print,如下:
``` C
// ~/C_study/print.c
// C语言中每行代码结束都必须带上分号!不是中文字符

#include<stdio.h> //引入stdio.h库
int main() //main不可修改,唯一的
{
    printf("Hello!"); //打印命令
    return 0; // 强烈建议读者养成在main() 函数中保留return 语句的好习惯
}
```
### 是的,你没有看错,这就是一个简单的打印程序,与Python的打印相比,代码多得多
```Python
print ("Hello!")
```
## 注释
```C
// 有几种方式,如下:

/* 注释 */

/* 注释1,
    注释2. */

/*
    注释
*/

//注释(单行)
```

## 变量
设置变量,如下:
```C
int num; // num为变量名,变量名不可是C语言中的关键字
num = 1; // 给变量赋值
```
若想将用户输入的值存放到变量中,如下:
```C
int number;
printf("input a number: ");
scanf("%d", &number);
printf("%d", number); //验证是否将输入的值存放到变量中
```
若想使用两个变量,并且运算,如下:
```C
int day, age;
//该行不可以声明day,否则无法运算 (day = age *365)
printf("Input your age: ");
scanf("%d", &age); //将输入的值存放进变量age中
day = age * 365; //在这里声明变量day,即可运算,代码是从上往下运行的
printf("Days: %d", day); //此处的%d为变量day的值
```
