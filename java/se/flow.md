---
description: Flow流程，Java中有三种流程。
---

# Flow

Java中三种流程分别为：顺序结构、选择结构、循环结构。

新人不知道java的流程控制，请解释一下有几种流程控制。

> Java中有三种基本的流程控制结构，分别是：
>
> 1. 顺序结构：程序按照代码的顺序依次执行。
> 2. 选择结构：根据条件的真假来执行不同的代码分支。Java中的选择结构主要有if语句和switch语句。
> 3. 循环结构：根据循环条件来重复执行某段代码。Java中的循环结构主要有while循环、do-while循环和for循环。
>
> 这些基本的流程控制结构可以组合使用，实现复杂的程序逻辑。



## 一：选择结构

新人不知道Java选择结构，请用代码说明（中文注释）

> 好的，以下是Java中的选择结构代码示例，包括 if 语句和 switch 语句：

### 1：if语句

```java
int x = 10;
if (x > 0) {
    System.out.println("x是正数");
} else if (x < 0) {
    System.out.println("x是负数");
} else {
    System.out.println("x是零");
}

```

> 在 if 语句中，如果条件成立，则执行 if 语句块中的代码，否则执行 else 语句块中的代码。else if 语句可以用来添加更多的条件分支。

### 2：switch语句

```
int x = 2;
switch (x) {
    case 1:
        System.out.println("x是1");
        break;
    case 2:
        System.out.println("x是2");
        break;
    case 3:
        System.out.println("x是3");
        break;
    default:
        System.out.println("x不是1、2、3中的任何一个");
        break;
}

```

> 在 switch 语句中，将要被匹配的值被放在 switch 关键字之后的括号中。每一个 case 子句包含一个要匹配的值和对应的执行语句。如果没有任何一个 case 与要匹配的值相等，则执行 default 语句块中的代码。注意每个 case 子句都需要使用 break 关键字来结束当前的代码块，否则代码将会继续执行下一个 case 子句。



## 二：循环结构

新人不知道Java循环结构，请用代码说明（中文注释）

> 以下是 Java 中常见的循环结构，附有相应的代码和注释：

### 1：while 循环

```java
int i = 1; // 初始化循环变量
while (i <= 5) { // 循环条件
    System.out.println("这是第" + i + "次循环"); // 循环体
    i++; // 循环变量更新
}

```



### 2：do-while 循环

```java
int i = 1; // 初始化循环变量
do {
    System.out.println("这是第" + i + "次循环"); // 循环体
    i++; // 循环变量更新
} while (i <= 5); // 循环条件

```



### 3：for 循环

```java
for (int i = 1; i <= 5; i++) { // 初始化循环变量; 循环条件; 循环变量更新
    System.out.println("这是第" + i + "次循环"); // 循环体
}

```



### 4：增强型 for 循环

> （适用于遍历数组或集合）

```java
int[] nums = {1, 2, 3, 4, 5};
for (int num : nums) { // 将 nums 数组中的每个元素赋值给 num
    System.out.println(num); // 循环体
}

```



> 以上是 Java 中常见的循环结构，它们可以让程序执行特定的任务，提高代码的效率和可读性。
