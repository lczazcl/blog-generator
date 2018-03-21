---
title: JS里的数据
date: 2018-03-21 15:14:43
tags:
---
### JS的历史
1994年，Netscape公司发明一款浏览器叫做Netscape Navigator，它有一个重磅的功能就是支持脚本语言。管理层暂定这门语言叫做Mocha，同时也决定脚本语言的语法要接近Java。
1995年，Netscape公司雇佣了程序员Brendan Eich开发这种网页脚本语言。
1995年5月，Brendan Eich只用了10天，就设计完成了这种语言的第一版。

### JS有7中数据类型：
数字、字符串、布尔、Symbol（符号）、未定义、null、对象
number、string、boolean、Symbol、undefined、null、Object（包含array、function）

### 数据的表示方式：
#### number：
十进制(1,2,3)，小数(1.1，.1)，科学计数法(1.23e2)
二进制(0b1,0b10)
八进制(011,)，存电话号码的方式应该是：'01012345'
十六进制(0x11)

#### string：
'你好'，"你好"，''，""，" "
空字符串长度为0
空格字符串长度为1
```
var a = "'"     显示一个单引号
var a = '\''    \转义符
var n = '\n'    显示一个回车
var t = '\t'    显示一个制表符（q左边的按键）
var b = '\\'    一个\
var s = '12345\     字符串换行
        67890'
var s2 = '12345'+   好读的语法
        '67890'
var s3 = `12345     es6的多行字符串
67890`                
```

#### boolean：
* 乔治·布尔
乔治·布尔是英格兰数学家和哲学家、数理逻辑学先驱。
由于其在符号逻辑运算中的特殊贡献，很多计算机语言中将逻辑运算称为布尔运算，将其结果称为布尔值。
1864年，布尔冒着大雨步行两英里走到讲台，身着打湿的衣服为学生们授课。不久后，他就病倒了，得了重度感冒还发高烧。其妻错误地相信疾病需要用致病因子施救，因为布尔是淋雨水而感冒的，妻子于是用桶子装水淋到他身上。结果湿气进一步加剧了他的病情。1864年，12月8日，布尔死于肺部积水。
* boolean 的取值
只有两个值：true 和 false
a && b 在 a 和 b 都为 true 时，取值为 true；否则为 false
a || b 在 a 和 b 都为 false 时，取值为 false；否则为 true

#### null 和 undefined：
这是JS的一个bug，都表示什么也没有（有一些区别）。
&emsp;&emsp;i、（规范）如果一个变量没有被赋值，那么这个变量的值就是 undefiend
&emsp;&emsp;ii、（习俗）如果你想表示一个还没赋值的对象，就用 null。如果你想表示一个还没赋值的字符串/数字/布尔/symbol，就用 undefined（但是实际上你直接 var xxx 一下就行了，不用写 var xxx = undefined）

#### OBject：
又叫做哈希表。前面的都是基本类型（简单类型），Object是复杂类型，复杂类型由上面几种简单类型（无序地）组合在一起。
```
var person = {
    name : '李四',
    age : 18,
    gender : male,
    married : false,
    wife : undefined,
    children : null,
    '':'lcz'
}
```
* object 的 key 一律是字符串，不存在其他类型的 key
* object[''] 是合法的
* object['key'] 可以写作 object.key
* 注意 object.key 与 object[key] 不同
* delete object['key']
* 'key' in object

#### typeof:
![](http://ww1.sinaimg.cn/large/9b135823ly1fpklt50ct9j20ng02w3yl.jpg)



