---
title: 面向对象-java类以及类的成员
date: 2017-05-26 12:12:57
categories: java基础
tags:
- java
---



### java类以及类的成员:属性,方法,构造器;代码块,内部类

![image-20221110162529295](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544484.png)

## 面向过程与面向对象

![image-20221110164953202](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544177.png)

![image-20221110165951763](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544854.png)

![image-20221110170031878](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281544863.png)

### java语言的基本元素:类与对象

![image-20221110170335418](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545183.png)

![image-20221110170559944](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545291.png)

![image-20221110170706319](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545069.png)

### 类的结构:属性与方法

![image-20221110171238179](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545680.png)

![image-20221113151740802](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545651.png) 

![image-20221113151947760](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545813.png)

## 创建类的对象



![image-20221113152239822](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545767.png)

```java
person p = new person;
//创建类的对象=类的实例化=实例化类
//调用对象的结构:属性,方法
//调用属性:"对象.属性"
```

![image-20221113152826043](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545640.png)

![image-20221113153114797](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281545636.png)

```
p1成为了类的实例,并且属性就是成员变量
```

![image-20221113160220957](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546891.png)

#### 如果创建了一个类的多个对象,那么每个对象都独立的拥有一套类的属性



![image-20221113161151863](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546429.png)

地址值是相同的,至于为什么 p3=p1,大概是因为类型是相同的所以省略了后缀吧

## 对象的内存解析

 ![image-20221113161354349](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546055.png)

这是对象的具体内存结构

![image-20221113161824120](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546399.png)

## 属性与局部变量的对比

![image-20221113164125220](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546783.png)

属性可以声明权限

![image-20221113164142504](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546408.png)

其实就是变量一类的东西放的位置不同,他的功能也就不同,

![image-20221113164403247](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546928.png)

局部变量在调用时都必须赋值

形参在调用时赋值即可

### 局部变量与属性加载的位置不同

![image-20221113193414879](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546212.png)

## 方法举例与格式的说明

![image-20221115163831432](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546559.png)

```
void表示没有返回值
有string的表示返回值为string
()内写的是形参

```

 ![image-20221115164258700](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546229.png)

![image-20221115164343471](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546343.png)

### 方法的声明

```
权限修饰符 返回值类型 方法名(形参列表){方法体}
```

![image-20221115164555548](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546716.png)

#### 权限修饰符

```
private.public,缺省,protected--封装性再细说,默认都先使用public
```

#### 返回值类型

```
如果有返回值,必须在方法声明时,指定返回值的类型.同时方法中需要使用return来返回指定类型的变量或者常量
```

![image-20221115165041333](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546529.png)

第一个时变量,第二个是常量

每一个可以输出的地方或者结果的地方都需要返回值

```
如果方法没有返回值,则在方法声明时,使用void来表示,通常情况下不用return,但是可以使用return;来结束此方法
return后不可以声明表达式
 
```

### 小结1

![image-20221115165652260](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546640.png)

![image-20221115165702139](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281546009.png)

### 方法名

```
方法名属于标识符,要使用规范,遵循所见即所得原则

```

### 形参列表

```
可以声明一个或多个形参
格式 :数据类型 形参,数据类型 形参.....
只声明不赋值
```

![image-20221116101717887](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547054.png)

![image-20221116101841712](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547407.png)

### 一些注意点

类内部的方法可以调用类的属性

方法内部可以调用方法

递归就是方法自己调用自己

方法中不能定义方法

### 传输接受与返回

![image-20221117101910110](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547610.png)

多理解理解

当然如果没有返回那直接写个sout也可以

#### 传参数的问题

![image-20221117102137790](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547934.png)

![image-20221117102144642](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547451.png)

```java
如果方法会调用类的属性,那么修改类,也可以更改参数

如果用形参,传入数据,也是修改参数的一种方法

但是这两种方法一旦弄混了,那就会出现各种奇怪的bug
```

### 对象与static的错误

![image-20221117102529665](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547872.png)

如果你建方法时不用static,那么就必须造一个对象去调用,否则会出错,这里涉及到的点之后回去详细说明

### 关于方法声明的一些练习

![image-20221117145702406](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547085.png)

![image-20221117145749766](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547737.png)

如果直接调用method方法,那么就必须把static给补上

![image-20221117150418016](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547102.png)

先强化造对象的过程再说别的

![image-20221117150645874](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547778.png)

虽然说里边是个方法,但是实际上返回值是变量,也就是最终结果是变量,所以可以放

### 属性与形参

![image-20221117152023865](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547084.png)

这个代码已经说明的很清楚了

![image-20221117152148621](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547621.png)

形参的调用

### 重点好题⭐

![image-20221117152920791](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547603.png)

![image-20221117153215395](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547877.png)

**也就是说,数组里面啥都能装,可以装数字型,也能把对象给装进去.**

![image-20221117154558648](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547890.png)

换句话说这个数组的类是student类,的

具体原理参见柞与堆

![image-20221117153528207](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547105.png)

![image-20221117153642066](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547563.png)

还可以利用类里面的方法进行编辑

![image-20221117154213954](https://markdown-langxecho-save.oss-cn-hangzhou.aliyuncs.com/img/202301281547499.png)

数组之间的使用必须是同类型的.

