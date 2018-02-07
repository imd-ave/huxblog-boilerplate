---
layout:     post
title:      " Java学习笔记之递归"
subtitle:   "life"
date:       2018-2-07 
author:    "阿东"
header-img: 
tags:
 
---
 ```

```

###  Java学习笔记之递归
- - - - 
递归方法就是一种直接或通过其他方法间接调用自己的方法。
著名例子:斐波那契（Fibonacci)数列
  1,1,2,3,5,8,13.....

(注：相邻两个数相比收敛于1.618.. 。被称为黄金分割比，还有人认为黄金分割能够产生美的效果。)

public class Test {

	public static void main(String[] args) {
		System.out.println(f(5));

	}

	public static int f(int i) {
		if(i==1||i==2)
			return 1;
		else
		return f(i-1)+f(i-2);
	}
}
这里只是计算了第五个的值。
  ###   与迭代的区别
终止测试：

迭代在循环条件失败时终止。

递归则是在识别到基本情况后终止。

然而任何用递归可以解决的问题同样可以用迭代解决，不过迭代方法不够直观。

递归浪费时间，而且还占用大量的内存。
但是递归可以更加自然的反映问题，并且产生的程序易于调试和理解。
