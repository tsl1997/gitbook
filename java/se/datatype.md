---
description: Java基本数据类型，一切数据由此开始
---

# DataType

本文档引用部分是ChatGPT的回答。

新手不知道Java的数据类型，向他解释Java的八大数据类型。并且附带代码案例，代码请用中文注释。

> Java的八大基本数据类型包括四种整型、两种浮点型、一个字符型和一个布尔型。它们的具体数据类型和占用内存如下：
>
> * byte：1字节，范围是-128到127。
> * short：2字节，范围是-32768到32767。
> * int：4字节，范围是-2147483648到2147483647。
> * long：8字节，范围是-9223372036854775808到9223372036854775807。
> * float：4字节，范围是3.4e-45到3.4e38，精度为6\~7位小数。
> * double：8字节，范围是4.9e-324到1.8e308，精度为15位小数。
> * char：2字节，表示一个字符，范围是0到65535。
> * boolean：1位，只有true和false两个值。
>
> 下面是一个使用Java基本数据类型的示例代码：
>
> ```java
> public class DataTypeExample {
>     public static void main(String[] args) {
>         byte a = 127;
>         short b = 32767;
>         int c = 2147483647;
>         long d = 9223372036854775807L;
>         float e = 3.1415926f;
>         double f = 2.718281828459;
>         char g = 'A';
>         boolean h = true;
>
>         System.out.println("byte类型：" + a);
>         System.out.println("short类型：" + b);
>         System.out.println("int类型：" + c);
>         System.out.println("long类型：" + d);
>         System.out.println("float类型：" + e);
>         System.out.println("double类型：" + f);
>         System.out.println("char类型：" + g);
>         System.out.println("boolean类型：" + h);
>     }
> }
> ```
>
> 在代码中，我们使用了各种基本数据类型，并将它们的值打印到控制台上。可以通过运行程序来验证代码的正确性。

数值（整数）：byte、short、int、long

浮点（小数）：float、double

字符（单个）：char

布尔值：boolean（表示真或者假）

除上述八种基本类型外，其他数据类型均为引用类型。
