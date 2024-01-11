[**回到主页**](http://localhost:3000)
[**回到目录**](./README.md)

# JAVA

## 命名规则

1. 不能出现空格、@，关键字:48 个关键字：abstract、assert、boolean、break、byte、case、catch、char、class、continue、default、do、double、else、enum、extends、final、finally、float、for、if、implements、import、int、interface、instanceof、long、native、new、package、private、protected、public、return、short、static、strictfp、super、switch、synchronized、this、throw、throws、transient、try、void、volatile、while
2. 区分大小写
3. 可以使用$

## 基本语法

- 方法名应该都以小写字母开头
- 类名的首字母应该大写
- 大小写敏感
- 所有的 Java 程序由 public static void main(String[] args) 方法开始执行
- 方法定义：访问修饰符 返回值 方法名（参数列表）{方法体}

## 数据类型

### 基本数据类型

#### 数值型

- 整数（byte，short，int，long）
- 十进制整数
- 十六进制整数：以 0x 或 0X 开头
- 八进制整数：以 0 开头
- 长整型数：在数字的后面加上 L 或 l

#### 浮点（float，double）

- 表示 float 型要在数字后加 f 或 F
- 表示 double 型要在数字后加 d 或 D，带小数点默认是- 双精度，d 可省略

#### 字符型（char）

#### 布尔型（boolean）

- 占 4 个字符

#### 数据类型间的优先关系：

    byte<short<char<int<float<double

```
//由低到高会自动转化
int i；
double j = i //将 i 转为 double
// 由高到低需要强制转化
int i = 12;
byte b = (byte)i;//把 i 强制转化为 byte
```

#### 其他类型转换

##### 字符串转数字：

Integer.parseInt(String s);//转换成整型的数值

##### 数字转字符串:

1. Byte.toString(byte b);//字节转字符串
2. String.valueOf(各种类型的数值变量)
3. 用空字符串连接数字，将数字转换为字符串
   eg：“”+25

### 引用数字类型

#### 类（class）

#### 接口（interfaxe）

#### 数组

##### 一维数组

###### 声明：

类型 数组名[ ] 或类型 [ ] 数组名

eg： `int intArray[ ];//定义一个整型数组 ps：声明数组时不能指定数组中元素个数`

###### 初始化：

**法 1：定义数组时就为元素赋值**

eg：`int intArray[ ] = {1,2,3,4}`

**法 2：用 new 创建**

```
int a[ ];
a = new int[2];//创建一个有两个元素的 a 数组
a[0] = 1;
a[1] = 2; //为数组赋值
```

##### 二维数组

###### 声明：

`类型 数据名[ ][ ];或类型 [ ][ ] 数组名`

###### 初始化：

与一维类似

java 中允许数组维度不同

##### 枚举（enum）

###### 声明：

`enum 枚举名{ 常量列表 }`

## 控制语句

- if else 同 c 类似
- swich 同 c 类似
- for 同 c 类似
- while 同 c 类似
- do while 语句 同 c 类似
- continue： 跳出本次循环，进入下一个循环；break：结束循环
