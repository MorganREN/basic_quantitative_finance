# 量化投资与Python

## 怎样用Python做量化分析

### 为什么选择Python
其他选择：Excel、SAS/SPSS、R

量化投资实际上就是分析数据从而做出的决策的过程

Python数据处理相关模块：
    - Numpy：数据批量计算
    - pandas：灵活的表计算
    - Matplotlib：数据可视化

### 如何使用Python进行量化投资
自己编写：NumPy + pandas + Matplotlib...

在线平台：聚宽、优矿、米筐、Quantopian、...

开源框架：RQAlpha、QUANTAXIS、...



## IPython命令行介绍
### 安装与使用
skip

### IPython高级功能
TAB键自动补全

?: 内省、命名空间搜索

!: 执行系统命令

丰富的快捷键




## Numpy模块介绍
### Numpy简介
Numpy是高性能科学计算和数据分析的基础包。他是pandas等其他各种工具的基础。

Numpy的主要功能：
    - ndarray，一个多维数组结构，高效且节省空间
    - 无需循环对整组数据进行快速运算的数学函数
    - 线性代数、随机数生成和傅里叶变换功能

安装与导入
    -skip

### 为什么要用Numpy
- 例1：已知若干家跨国公司的市值（美元），将其换算成RMB
- 例2：已知购物车中每件商品的价格与商品件数，求总金额

### ndarray-多维数组的对象
创建ndarray：np.array(array_like)

数组与列表的区别：
    - 数组对象内的元素类型必须相同
    - 数组大小不可改变】

### ndarray-常用属性
T - 数组的转置（对高维数组而言）

size - 数组元素的个数

ndim - 数组的维度

shape - 数组的维度大小

dtype - 数组元素的数据类型

### ndarray-创建
- array()      将列表转换为数组，可选择显式指定dtype
- arange()     range的numpy版，支持浮点数
- linspace()   类似arange()，第三个参数为数组长度
- zeros()     根据指定形状和dtype创建全0数组
- ones()      根据指定形状和dtype创建全1数组
- empty()     根据指定形状和dtype创建空数组（随机值）
- eye()       根据指定边长和dtype创建单位矩阵

### ndarray-批量运算
- 数组和标量之间的运算：
    - a+1   a*3   1//a   a**0.5   a>5

-同样大小数组之间的运算
    - a+b   a/b   a**b   a%b   a==b
    
### ndarray-索引
一维数组的索引：a[5]
多维数组的索引：
    - 列表式写法：a[2][3]
    - 新式写法: a[2, 3]
    
### ndarray-切片
一维数组的切片：a[5:8]   a[4: ]    a[2:10]=1

多维数组的切片：a[1:2, 3:4]   a[:, 3:5]   a[:,1]

数组切片与列表切片的不同：数组切片时并不会自动复制（而是创建一个视图），在切片数组上的修改会影响原数组

copy()方法可以创建数组的深拷贝









## pandas模块介绍




## Matplotlib模块介绍