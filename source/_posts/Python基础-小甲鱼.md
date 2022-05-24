---
title: Python基础-小甲鱼
date: 2022-03-31 15:03:14
tags: Python
categories: Python
---
<meta name="referrer" content="no-referrer" />

# 变量

## 变量的赋值传递通过引用

改变x的值，y的值也变

![image-20220301182457639](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301182457639.png)

## 拷贝

### 浅拷贝——复制表层（默认，更快）

对于一维列表：拷贝整个列表对象。修改原本不影响副本。功能相当于深拷贝

![image-20220301183640129](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301183640129.png)

对于嵌套列表：只拷贝外层对象，而内层对象拷贝的是引用

❌：![image-20220301183801810](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301183801810.png)副本也被修改，此时需要用深拷贝

下面的B即浅拷贝：![image-20220301182029476](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301182029476.png)

### 深拷贝——完全复制

![image-20220301192743827](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301192743827.png)

copy：浅拷贝

deepcopy：深拷贝，拷贝每个子对象

## 交换两个变量

`x, y = y, x`

# 随机数攻击

![image-20220228135938403](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228135938403.png)

# 浮点数操作

![image-20220228140901342](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228140901342.png)

# 复数

![image-20220228141028918](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228141028918.png)

# 数字操作

![image-20220228141329175](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228141329175.png)

# 短路逻辑

![image-20220228145427316](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228145427316.png)

![image-20220228145356993](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228145356993.png)

# 运算符优先级

![image-20220228145712407](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228145712407.png)

# 流程图

![image-20220228150258641](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228150258641.png)

# 条件表达式

![image-20220228205259446](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228205259446.png)

## 判断素数

![image-20220228214753918](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220228214753918.png)

# 列表

## 切片

![image-20220301123541533](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301123541533.png)

## 方法

### 增

- append/extend：在末尾添加一个元素/可迭代对象

- 用切片的方法在末尾添加：![image-20220301123939996](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301123939996.png)

- insert(pos, element)：![image-20220301124059320](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301124059320.png)

### 删

remove：只删除第一个，没有就报错

pop：删除指定下标元素

clear

### 改

指定下标替换元素原理：![image-20220301124839542](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301124839542.png)

排序、倒序：![image-20220301125130513](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301125130513.png)

### 查

count、index函数：![image-20220301130724895](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301130724895.png)

## 列表推导式

![image-20220301194221719](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301194221719.png)

速度比循环快。

循环修改原来的列表，列表推导式创建新的列表然后赋值。

![image-20220301194450781](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301194450781.png)

![image-20220301200335888](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301200335888.png)

![image-20220301200405843](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301200405843.png)

用列表推导式创建嵌套列表（这样各个子列表互不影响）：![image-20220301201224163](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301201224163.png)

![image-20220301201248960](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301201248960.png)

![image-20220301201357615](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301201357615.png)

### 列表推导式的嵌套

![image-20220301201635082](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301201635082.png)

实现 笛卡尔乘积：![image-20220301201819007](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301201819007.png)

![image-20220301201844779](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301201844779.png)

kiss原则：![image-20220301202022045](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301202022045.png)

# 元组

打包解压

不可修改

![image-20220301202350750](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301202350750.png)

没有元组推导式，有生成器：![image-20220301202525280](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301202525280.png)

生成只有一个元素的元组：![image-20220301202643020](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301202643020.png)

序列类型对象的打包解包（多重赋值的实现原理）：![image-20220301202841517](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301202841517.png)

![image-20220301202924746](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301202924746.png)

元组内的可变元素是可变的：![image-20220301203301289](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301203301289.png)

# 字符串

## 回文数判断

![image-20220301203448296](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301203448296.png)

## 方法

![image-20220301203559166](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301203559166.png)

![image-20220301204538404](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301204538404.png)

![image-20220301204715307](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301204715307.png)

![image-20220301204743673](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301204743673.png)

![image-20220301204923816](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301204923816.png)

![image-20220301205346736](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301205346736.png)

![image-20220301205419832](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220301205419832.png)

![image-20220302133034825](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302133034825.png)

![image-20220302133249814](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302133249814.png)

拆分：

![image-20220302134058044](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302134058044.png)

拼接：join比+快

![image-20220302142015805](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302142015805.png)

## 格式化字符串

![image-20220302145045514](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302145045514.png)

![image-20220302143226504](C:\Users\cc188\AppData\Roaming\Typora\typora-user-images\image-20220302143226504.png)

![image-20220302143611321](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302143611321.png)

![image-20220302143808099](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302143808099.png)

## f-string 

python 3.6

![image-20220302145009710](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220302145009710.png)

# 序列——列表 元组 字符串

- 列表：可变序列 

- 元组 字符串：不可变序列

可变序列和不可变序列的身份证（id）区别：![image-20220303134128230](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220303134128230.png)

同一性运算符：is 和 isnot。检测id是否相等，判断两个对象是否一样![image-20220303141016983](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220303141016983.png)

in / not in ：是否包含

del：![image-20220303141458651](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220303141458651.png)![image-20220303141606227](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220303141606227.png)

## 方法

![image-20220304141630675](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304141630675.png)

![image-20220304150916887](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304150916887.png)

![image-20220304151219916](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304151219916.png)

![image-20220304151232333](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304151232333.png)

![image-20220304151522024](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304151522024.png)

![image-20220304151539174](C:\Users\cc188\AppData\Roaming\Typora\typora-user-images\image-20220304151539174.png)

![](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304151627980.png)

# 迭代器 vs 可迭代对象

前者一定是后者

前者：一次性

后者：可重复使用

![image-20220304152617986](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304152617986.png)

# 字典

python中唯一实现映射关系的内置类型

摩斯密码![image-20220304153009630](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304153009630.png)

快速初始化：<img src="https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304155511836.png" alt="image-20220304155511836 " style="zoom:200%;" />

删除：pop、popitem（3.7之前随机，3.7之后删除最后一个，因为3.7之后字典有序）、del、clear

修改：update（同时修改多个）

查：![image-20220304163507782](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304163507782.png)

视图对象：![image-20220304163629933](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304163629933.png)

字典推导式：![image-20220304164058958](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304164058958.png)

# 集合

不重复、无序

元素可hash。字典的键同样

判断列表是否有重复：![image-20220304172044770](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304172044770.png)

集合运算：![image-20220304172717528](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304172717528.png)

# 函数

参数：位置参数、关键字参数、默认参数、收集参数、解包参数

## 收集参数

（打包成元组or字典）

打包为元组：

![image-20220304181535388](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304181535388.png)![image-20220304181224851](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304181224851.png)

![image-20220304181718643](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304181718643.png)

打包成字典：![image-20220304181816625](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304181816625.png)

混合（format函数）：![image-20220304181916228](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304181916228.png)

返回多个值：元组打包

##  解包参数 

解包元组

![image-20220304182230642](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304182230642.png)

解包关键字参数

![image-20220304182326483](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220304182326483.png)

## 作用域

变量默认全局

1. 如果要在函数内修改外层变量，需用global声明

   `global num  # 使用global声明num，在函数中就可以修改全局变量的值`

2. nonlocal语句：内部函数修改外部函数的变量值

## 闭包

使用nonlocal，记住外层函数中变量的状态，返回内层函数

![image-20220305141018523](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220305141018523.png)

## 装饰器

有参数比无参数：添加一次调用把参数传进去

无：![image-20220305143002797](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220305143002797.png)

有：![image-20220305143012070](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220305143012070.png)

## lambda表达式

![image-20220305144937120](https://gitee.com/chrislion/typora_image_repo/raw/master/img/image-20220305144937120.png)

## 生成器

在迭代的同时生成元素

和 return 相比，yield 除了可以返回相应的值，还有一个更重要的功能，即每当程序执行完该语句时，程序就会暂停执行。不仅如此，即便调用生成器函数，[Python](http://c.biancheng.net/python/) 解释器也不会执行函数中的代码，它只会返回一个生成器（对象）。

实现：生成器表达式 or yield

