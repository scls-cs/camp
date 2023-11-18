---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
rise:
  start_slideshow_at: beginning

kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

上一章我们学习了控制结构的第一种：分支结构。这一章我们会见到控制结构的第二种，也是最后一种结构：循环结构。不管程序有多么复杂，它都可以分解为顺序结构、分支结构和循环结构。

也就是说学完这章后，你就可以开始写更复杂的程序了。

# While Loop I #

while循环的语法如下：
```python
while(condition):    #循环条件
    statements       #循环体
```
这句话的意思是：只要循环条件为真，就一直反复执行循环体里语句。当括号里的条件为假时，则停止循环，继续执行while循环后面的语句。

如果第一次循环条件就不成立，那么循环体里的语句就不会执行。

while和if看起来比较相似，但if里的语句最多只会执行一次，而while可以执行多次。

```python
if(x < 3):
    x = x+1   #只会执行一次

while(x < 3):
    x = x+1   #会执行多次
```

# 循环设计的四个步骤 #

计数控制循环是最简单的循环方式。通过设置一个计数器(counter)作为循环变量(loop control variable)，可以决定循环的次数。

下面以计数控制循环为例，来介绍循环设计的"四部曲"：

1. 循环变量初始化：一般设置为0
2. 设置循环条件：通常是包含循环变量的布尔表达式
3. 编写循环体
4. 更新循环变量

```{code-cell} python3
count = 0                #1.循环变量初始化

while(count < 10):       #2.循环条件
    print(count)         #3.循环体
    count = count + 1    #4.更新循环变量
```


# 练习 #

Ex1：下面程序打印的第一个和最后一个数字分别是多少？
```python
value = 10

while(value < 15):
    print(value)
    value = value+1
```

Ex2：下面程序打印结果是什么？

```python
count = 5

while(count < 50):
  count = count * 2
  count = count+1

print(count)
```

Ex3：调用函数的结果是什么？

```python
def sum(n):
  i = 1
  t = 0
  while(i<=n):
    t=t+i
    i=i+1
  return t

print(sum(10))
```
Ex4：编写函数star(n)，实现打印1~n的功能.

```{code-cell} python3
def star(n):
  print(n)

star(10) # 1 2 3 4 ... 8 9 10(每行打印一个数）
```


Ex5：用循环的方式编写函数f(a,b)，使函数可以返回a的b次方

```{code-cell} python3
def f(a,b):
  total = 1
  #add your code here
  
  
  
  return total

print(f(2,3))   #8
print(f(3,4))   #81
```

## 作业 ##

1. Write a while loop that will print the numbers from 1 to 100 (inclusive), one number per line.
i = 1
while(i<=100):
  print(i)
  i=i+1

2. Write a while loop that will print the numbers from 50 to -50 (inclusive), one number per line.

3. Given some positive number n, write a while loop that will print the odd numbers from -n to n (inclusive), one number per line. The given number may be even or odd.

    
4. 给出一个小球从100米的高度自由落体，每次碰到地面后都会反弹到原来高度的90%。计算球在高度小于1米后，总共弹跳了多少次。

5. 设想你每月向银行账户存入100元，银行年利率为2%。计算需要多少个月，你的银行账户的余额才能达到5000元。

## 课件 ##

课件下载：{download}`Loops I <While循环.pptx>`