---
title: 分支语句2switchcase结构
date: 2017-05-26 12:12:57
categories: java基础
tags:
- java
---



## switch-case结构

![image-20221017184121486](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281543383.png)

![image-20221017184256181](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281543794.png)

如果上面的case都没有执行,那就default

### 与if else不同,swichcase结构在锁定条件之后会继续执行被满足条件的下面的语句,如:

![image-20221017184712683](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281543278.png)

输出结果为   two   three  other 

![image-20221017184802142](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544057.png)

![image-20221017184912163](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544167.png)

switch 结构中的表达式只能是如下的六种类型之一

![image-20221017185011210](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544265.png) 

case之后只能声明常量,不能声明范围

 ![image-20221017185436123](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544029.png)

像这种就是错的

break词缀是可选的

default相当于if,else中的else,并且位置是可选的,放哪都行,但是没有break还是会向下执行,一般就写在最后一行就行

如果多个case的执行语句相同,可以进行合并

![image-20221017185947105](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544274.png)

其实就是相当于没写break



### 试题:请输入2019年的day和month,问这是第几天

![image-20221017190407826](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544177.png)

如果这么写,就冗余了

解决冗余的方法:

![image-20221017190628512](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544348.png)

## switchcase与ifelse转换的说明

- switchcase结构如果要判断的表达式太多,一般用整除的方法

![image-20221017191156918](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544268.png)