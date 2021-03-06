# Python来历

名字是monty python's flying circus 

# Python解释器



# 基本数据类型

## 数字

你可以像使用计算机一样使用它们 + - × / ，也可以使用括号 () 提升他们的优先级顺序

2+3   -> 5

50 - 5*6   -> 20

(50 - 5*6)  / 4   -> 5.0

8 / 5    -> 1.6

5 和 20 是 int 类型 5.0 和 1.6 是 float 类型

division返回的总是一个浮点数，想得到一个整数结果的话你得使用 //, 如果想要得到余数的话，还可以使用 %

17 / 3    -> 5.66666666666666666667

17 // 3    -> 5

17 % 3    -> 2

5*3 + 2    -> 17

还可以使用 ** 运算符来计算幂

5 ** 2    -> 25

2 ** 7    -> 128

至于等号，则表示赋值

width = 20

height = 5 * 9

width * height    -> 900

- 如果变量没定义你使用它的话，它会抛出一个NameError的异常

含有浮点数的运算结果会转化为浮点数

4 * 3.75 - 1    -> 14.0 

除了 int 和 float ，Python还支持其他类型的数字，例如 Decimal 和 Fraction。Python还内置了对复数的支持，并使用 j 或者 J 后缀来表示虚部分

### 字符串

除了数字，Python还可以操作字符串，这可以通过多种方式表达。他们可以用单引号 ('.....') 或双引号 ("......") 括起来, 如果想在字符串中间输入单引号或双引号则可以使用 \ 进行转义。

```'Hello'    -> 'Hello'```

```'Hello \' World '```single quotes出现在了字符串中

```"Hello \" World"``` double quotes也可以出现在字符串中

在single quotes中如果想使用引用那么请使用double quotes

if 你不想把 \ 当做转义字符理解，那么需要在字符串前面加 r

print(r'c:\windows\nginx')  # 这里有一个 \n 所以你要是不加 r 的话就会被理解为换行

if 你想让字符串跨行的话可以在结尾加上 \ ，也可以使用 '''......''' ,

字符串可以做连接操作

'Hello' + 'World'    -> 'HelloWorld' 

'Hello' 'World'    -> 'HelloWorld'  # 空格会让相邻的字符串自动合并成 一个字符串

PEP8规范中有一条，单行不能超过79个字符，那么我们就可以

```python
print('......第79个字符'
	  '第80个字符')  # 自动连接的事情Python会替你搞定的
```
可是 if 你想让变量和字符串做这种操作的话，就必须使用 + 了

如果你想让字符串重复拼接

'Hello' * 3    -> 'HelloHelloHello'

字符串可以被索引(找到)，Python中即使只有一个字符，那么它也被称为字符串

word = 'Python'

我们可以看到 word 由6个字符组成，关于这一点我们可以用 len() 来进行验证

把 word 当做参数传递给 len() 结果就会返回6

if 你想查看 word 中的第一个字符，那么可以使用 word[0] ,它会输出'P', 因为 index 是从0开始的

那么最后一个字符就是'n', 它的索引是5

不仅可以用5来找到它，你还可以倒着数，倒着数第一个就是它，那么猜猜它的 index 是几吧，

因为0已经被第一个字符给占了，所以它的 index 是 -1，你可以使用 word[-1] 来得到它

除了 Index 操作，你还可以使用切片功能(就是你可以要其中一部分)

such as I 想要后面4个 'thon' 那么我使用 word[2, 6] 明明按照 index 是第5位为什么要写6 呢，

because 切片的规矩就是前面的包括后面的不包括，(前闭后开，前包后不包)

因为这四个字符刚好到了最后，so you 也 can 使用 word[2:] 后面你不写，就可以到最后，

such as you 秀逗了下 写成了 word[2: -1] 那么后面的 'n' 可是不会在里面的哦

如果你想拿下整个 word 那么可以用 word[:] ，这样就表示，韩信带兵有多少给我多少

if you want 隔一个要一个那么就这样 word[::2]    -> Pto 这个2表示间隔，

你还可以让他们打道回府，后队变前队，word[::-1], -1表示倒着走

索引不可以超越界限，但是切片可以

#### 在Python中字符串属于不可变对象，因此你不能给字符串中的索引赋值

if you need a new string, then(那么) please 自行 create 吧



### 列表

列表是一种有序可变的顺序结构(有序就以为这可以通过索引找到它)，相当于其他语言中的数组,

像字符串一样列表也可以被索引和切片

if you对a list使用了切片操作，then就会return a new list

与 string 不同的是 list 是一个可变的顺序结构，so you 可以任意修改当前索引位置上的数据

you can use list() or [] initial a empty list     -> []

you can use [].append() 把参数传递给append来给列表尾巴上增加数据

you can 把一个空列表赋值给当前列表，来清空列表中的数据

跟字符串一样， 你还是可以用 len() 来查看 list 中有几个元素

list 中还可以嵌套另一个 list ，其实不只是 list，还可以嵌套数字等其他数据结构



# 流程控制

### 判断语句 if

### 循环

- while 循环
- for 循环
- range

### 退出循环

- continue
- break

# 数据结构





# 模块





# 输入输出



# 异常处理



# 虚拟环境

