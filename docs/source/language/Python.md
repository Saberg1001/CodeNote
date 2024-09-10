# Python教程

## Python中基础数据类型
  - 整数（int） 
  - 小数（float） 
  - 布尔值（bool） 包含 true 和 false
  - 字符串（str）
   
### 读取数据类型 使用type()函数
```python
print(type(123))
# class 'int'
```

### 数据类型之间相互转换
```python
str(123)  #把123的数据类型变为字符串
```

## Python中的运算
### 四则运算
- 加减乘除 + - * /
- 整除 // 只保留整数部分
- 模 % （求余）
- 幂运算 ** 比如2的n次方 2**n
- 括号 （） 有括号先算括号

### 比大小 
返回一个布尔值（真/对 True假/错 False）
- 大于 >
- 小于 <
- 等于 ==（备注：一个等号是赋值）
- 大于等于 >=
- 小于等于 <=
- 不等于 ！=

### and or not

0， 空的，表示没有， 都为False 
- and  一假即假

找到并返回第一个False（假）/找到并返回最后一个True（真）
- or   一真即真

找到并返回第一个True（真）/找到并返回最后一个False（假）

优先级：not > and > or

## python中变量与赋值

 ### 命名规则

- 常用规则
1. 变量中只能出现字母 数字 下划线 中文
2. 变量名第一个字符不能是数字

- 驼峰命名

 变量名由一堆单词组成，第一个单词首字母小写，其余单词首字母大写。bigDog

- 类ruby命名

变量名由一堆单词组成，单词间用下划线连接，单词首字母小写。big_dog

### 变量赋值
```
varA = a
```

## if 语句
```python
if x > y:
    x = x
elif x = y:
    x = 0
else:
    x = y
```

## python中的类及类的继承

- 定义父类和子类
  
  定义一个普通的类，这个类自动成为其他类可以继承的父类。
  
  子类通过在类定义时在括号中指定父类的名字来实现继承。

```python
class Animal:
    def___init___(self, name):
        self.name = name
    def speak(self):
            return "some sound"
class Dog(Animal)
    def speak(self):
        return "woof"
```
- 添加和修改子类的属性和方法：

  子类不仅可以重写父类的方法，还可以添加新的属性和方法。
    
- super()函数

  在子类中，可以使用super()函数来调用父类的方法。
```python
super().__init__(name)

```

## 列表
### 列表乘法
```python
>>> ["a","b"]*2
["a","b","a","b"]
```
### 列表表达式
variable = [元素操作 for 元素 in 列表 if 元素满足某种条件]
```python
list1 = [2*i for i in list2 if i>2]
```
zip函数：将可迭代的对象作为参数，将对象中的元素打包成为一个元组，然后返回由这些元组组成的列表
### 列表的扁平化
sum(参数a，参数b) 参数啊：可迭代对象；参数b：起始值，默认为0
```python
>>> sum([['C','C'],['O'],[]])
['C','C','O']
```