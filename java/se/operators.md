---
description: Operators运算符是Java语句中很重要的概念
---

# Operators

## 一：运算符的分类

新人不知道Java有哪些Operators？请按照元素的个数分类。

> 好的，按照元素个数分类，Java的Operators可以分为以下几类：
>
> 1. 一元Operators（Unary Operators）：操作一个单一的操作数，例如负数运算符“-”。
> 2. 二元Operators（Binary Operators）：操作两个操作数，例如加号“+”、“-”、“\*”、“/”、“%”等。
> 3. 三元Operators（Ternary Operators）：操作三个操作数，例如条件运算符“?:”。
> 4. 赋值Operators（Assignment Operators）：用于将右侧的值赋给左侧的变量，例如“=”、“+=”、“-=”、“\*=”、“/=”、“%=”等。
> 5. 自增自减Operators（Increment and Decrement Operators）：用于将变量的值增加或减少1，例如“++”、“--”。
> 6. 位运算Operators（Bitwise Operators）：操作二进制位，例如“&”、“|”、“^”、“\~”、“<<”、“>>”、“>>>”等。
> 7. 逻辑运算Operators（Logical Operators）：操作布尔类型的值，例如“&&”、“||”、“!”等。
>
> 需要注意的是，不同的Operators可能具有不同的优先级和结合性，因此在进行复杂的运算时，需要特别注意运算顺序。



## 二：一元运算符

也叫一目运算符。指参与操作的元素只有一个。

新人不知道Java一元运算符，请解释并且附带代码（中文注释）

> Java的一元运算符是只对一个操作数进行运算的运算符，包括正号、负号、自增、自减、逻辑非等。
>
> 下面是一些常用的一元运算符及其作用：
>
> * 正号（+）：表示正数，一般不进行实际的计算，仅为了明确表达式中某个操作数是正数。
> * 负号（-）：表示负数，可以用于将数字取反或求相反数。
> * 自增（++）：将变量的值加1，分为前缀和后缀两种形式，前缀表示先自增再使用变量的值，后缀表示先使用变量的值再自增。
> * 自减（--）：将变量的值减1，同样分为前缀和后缀两种形式，前缀表示先自减再使用变量的值，后缀表示先使用变量的值再自减。
> * 逻辑非（!）：对操作数取反，如果操作数是true，则返回false，如果操作数是false，则返回true。
>
> 下面是一些示例代码：
>
> ```java
> public class UnaryOperatorDemo {
>     public static void main(String[] args) {
>         int a = 10;
>         int b = -a; // 取反
>         int c = ++a; // 前缀自增
>         int d = a--; // 后缀自减
>         boolean flag = true;
>         boolean result = !flag; // 逻辑非
>         System.out.println("b = " + b); // 输出：b = -10
>         System.out.println("c = " + c); // 输出：c = 11
>         System.out.println("d = " + d); // 输出：d = 11
>         System.out.println("result = " + result); // 输出：result = false
>     }
> }
> ```



## 三：二元运算符

新人不知道Java二元运算符，请解释并且附带代码（中文注释）

> 好的，以下是Java中常见的二元运算符，附带中文注释的代码示例：

### 1：算术运算符

```java
public class Main {
    public static void main(String[] args) {
        int a = 10, b = 3;
        int c = a + b; // 加法
        int d = a - b; // 减法
        int e = a * b; // 乘法
        int f = a / b; // 整数除法
        int g = a % b; // 取模运算（余数）
        
        System.out.println("c = " + c);
        System.out.println("d = " + d);
        System.out.println("e = " + e);
        System.out.println("f = " + f);
        System.out.println("g = " + g);
    }
}

```



### 2：赋值运算符

```java
public class Main {
    public static void main(String[] args) {
        int a = 10, b = 3;
        int c = 0;
        c = a + b; // 算术运算符和赋值运算符的组合
        System.out.println("c = " + c);
        
        int d = 10;
        d += 3; // 等价于 d = d + 3;
        System.out.println("d = " + d);
    }
}

```



### 3：关系运算符

```java
public class Main {
    public static void main(String[] args) {
        int a = 10, b = 3;
        boolean c = a > b; // 大于
        boolean d = a < b; // 小于
        boolean e = a >= b; // 大于等于
        boolean f = a <= b; // 小于等于
        boolean g = a == b; // 等于
        boolean h = a != b; // 不等于
        
        System.out.println("c = " + c);
        System.out.println("d = " + d);
        System.out.println("e = " + e);
        System.out.println("f = " + f);
        System.out.println("g = " + g);
        System.out.println("h = " + h);
    }
}

```



### 4：逻辑运算符

```java
public class Main {
    public static void main(String[] args) {
        boolean a = true, b = false;
        boolean c = a && b; // 逻辑与
        boolean d = a || b; // 逻辑或
        boolean e = !a; // 逻辑非
        
        System.out.println("c = " + c);
        System.out.println("d = " + d);
        System.out.println("e = " + e);
    }
}

```



### 5：位运算符

结合上一个对话，请继续回答位运算符，并且附带代码

> 位运算符是对二进制位进行操作的运算符，常用的有按位与（&）、按位或（|）、按位异或（^）、按位取反（\~）、左移位（<<）、右移位（>>）和无符号右移位（>>>）。下面是对每个位运算符的说明和示例代码：

#### ①：按位与（&）

> 两个操作数中，位都为1则结果为1，否则结果为0。

```java
int a = 3;        // 0011
int b = 6;        // 0110
int c = a & b;    // 0010

System.out.println(c);    // 输出结果为2

```



#### ②：按位或（|）

> 两个操作数中，位都为0则结果为0，否则结果为1。

```java
int a = 3;        // 0011
int b = 6;        // 0110
int c = a | b;    // 0111

System.out.println(c);    // 输出结果为7

```



#### ③：按位异或（^）

> 两个操作数中，位相同则结果为0，否则结果为1。

```java
int a = 3;        // 0011
int b = 6;        // 0110
int c = a ^ b;    // 0101

System.out.println(c);    // 输出结果为5

```



#### ④：按位取反（\~）

> 对操作数的每个二进制位取反。

```java
int a = 3;        // 0011
int b = ~a;       // 1100

System.out.println(b);    // 输出结果为-4

```



#### ⑤：左移位（<<）

> 将操作数向左移动指定的位数，并在右侧补0。

```java
int a = 3;        // 0011
int b = a << 2;   // 1100

System.out.println(b);    // 输出结果为12

```



#### ⑥：右移位（>>）

> 将操作数向右移动指定的位数，并在左侧补上符号位的值。

```java
int a = -12;      // 11111111 11111111 11111111 11110100
int b = a >> 2;   // 11111111 11111111 11111111 11111101

System.out.println(b);    // 输出结果为-3

```



#### ⑦：无符号右移位（>>>）

> 将操作数向右移动指定的位数，并在左侧补0。

```java
int a = -12;      // 11111111 11111111 11111111 11110100
int b = a >>> 2;  // 00111111 11111111 11111111 11111101

System.out.println(b);    // 输出结果为1073741821

```



## 四：三元运算符

新人不知道Java三元运算符，请解释并且附带代码（中文注释）

> Java的三元运算符是一种特殊的运算符，它有三个操作数，语法结构如下：
>
> ```
> 条件表达式 ? 表达式1 : 表达式2
> ```
>
>
>
> 如果条件表达式的结果为 true，则返回表达式1的结果，否则返回表达式2的结果。
>
> 以下是一个简单的示例代码，演示了如何使用三元运算符：
>
>
>
> ```java
> public class Main {
>     public static void main(String[] args) {
>         int a = 10;
>         int b = 5;
>         int max = (a > b) ? a : b; // 如果a>b则max=a，否则max=b
>         System.out.println("最大值为：" + max); // 输出结果为10
>     }
> }
> ```
>
>
>
> 在上述代码中，三元运算符 `(a > b) ? a : b` 用于比较变量 `a` 和 `b` 的值，如果 `a` 大于 `b`，则返回 `a` 的值，否则返回 `b` 的值，最终结果赋值给变量 `max`，然后使用 `System.out.println()` 方法输出变量 `max` 的值。



纯新手可以跳过位运算，其他的均要学习并且掌握。
