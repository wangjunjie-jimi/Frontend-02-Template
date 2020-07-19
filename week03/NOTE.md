## 编程语言通识

### 运算符和表达式

1. Member 运算
   - a.b
    - a[b]
    - foo`string`
    - super.b, super['b']
    - new.target
    - new Foo()

2. New 
3. Call 
    - foo()
    - super()
    - foo()['b']
    - foo().b
    - foo()`abc`

例子：new a()['b'] 先new一个a对象，然后访问其b属性

4. 左右手运算
   - a.b = c √ 左手表达式
   - a + b = c × 右手表达式

  只有左手表达式可以放到左边

5. Update 
    - a ++
    - a --
    - -- a
    - ++ a

6. Unary 单目运算
    - delete a.b
    - void foo()
    - typeof a
    - \+ a
    - \- a
    - ~ a 位运算
    - ! a
    - await a

7. ** 
    - 乘方 唯一一个又结合运算
    - 2\*\*3\*\*4 = 2\*\*(3\*\*4)

8. 加减乘除

9. Equality 相等运算
   - ==
   - !=
   - ===
   - !==
10. Bitwise 按位运算
    - &^|

11. Logical 逻辑运算
    - && 
    - ||

12. Conditional 
    - ?: 唯一的三目运算

### 类型转换
- 基本间的转换

|     |  Number   |   String  |    Boolean |   Undefined  | Null    | Object    | Symbol    |
| --- | --- | --- | --- | --- | --- | --- | --- |
|   Number  |  -   |      |  0 false    | x    |   x  |   Boxing  |  x   |
|   String  |     |  -   | "" false    |  x   |   x  |   Boxing  |  x   |
|   Boolean  |  true 1<br> false 0   |  'true'<br>'false'   |   -  |  x   |  x   |  Boxing   |   x  |
|   Undefined |  NaN   |  'Undefined'   |  false   | -    |  x   |  x   |   x  |
|   Null  |   0  |  'null'   | false    |  x   | -    |   x  |   x  |
|   Object  |  valueOf   |   valueOf <br> toString() |  true   |  x   |  x   |  -   |   x  |
|   Symbol  |   x  |   x  |  x   |   x  |  x   |  Boxing   |  -   |

- 拆箱转换 Unboxing

  - 把Object转换为基本类型
  - ToPremitive
    - toString 
    - valueOf 加法会先调用valueOf
    - Symbol.toPrimitive 定义了这个会忽略其他

- 装箱转换 Boxing

| 类型    | 对象    | 值    |
| --- | --- | --- |
|   Number  |   new Number(1)  |  1   |
|   String  |   new String('1')  | '1'    |
|   Boolean  |  new Boolean(true)   |  true   |
|   Symbol  |   new Object(Symbol('a'))  | Symbol('a')    |

typeOf 区分

...
