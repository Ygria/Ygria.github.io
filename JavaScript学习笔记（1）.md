---
title: JavaScript学习笔记（1）
tags:
- 编程
- 2018
---
写在前面：
不管容易还是简单
总要尝试才知道答案
## JavaScript初探
JavaScript：**轻量级脚本语言**，是可插入HTML页面的编程代码。
将JavaScript插入HTML页面后，可由所有的现代浏览器执行。
## 对变量进行声明
\`\`\`javascript
var mood,age;
var mood;
var age;
var mood = "happy";
var age = 33;
var mood = "happy",age = 33;
\`\`\`
JavaScript不需要进行类型声明，因此它时一种**弱类型（weekly typed）**
### 字符串
单引号与双引号毫无区别，若字符串中包含单引号，则一般使用双引号。
var mood = "don't ask";
若要使用单引号，则需要对特殊符号进行**转义**：
var mood = 'don\\'t ask';
作为一个好的编程习惯，**不管选择用双引号还是单引号，都应当在整个脚本中保持一致**。
### 数值
如果想给一个变量赋数值，不用限定它必须是一个整数，JavaScript允许使用带小数点的数值，并且允许任意位小数，这样的数成为浮点数（floating-point number）：
var age = 33.25;
var temperature = -20;
var temperature = -20.3333333
### 布尔值
另一种重要的数据类型时布尔（boolean）类型
var sleeping = true;
var married = true;
### 数组
**字符串、数组和布尔值都有标量（scalar）**，如果某个变量时标量，它在任意时刻都只能有一个值，若需
var beatles = Array(4);
无法预知某个数组有多少个元素，JavaScript根本不要求在声明数组时必须给出元素个数时，可以在声明数组时不给出元素个数：
var beatles = Array();
根据这个位置都有这个元素的下标（index），数组里一个元素的一个下标，下标必须用方括号括起来：
array\[index\] = element;
声明方式：
（1）
var beatles = Array(4);
beatles\[0\] = "John";
beatles\[1\] = "Paul";
beatles\[2\] = "George";
beatles\[3\] = "Ringo";
（2）
var beatles = Array("John","Paul","George","Ringo");
var years = \[1940,1941,1942,1942\];
var lennon = \["John",1940,false\];
数组中还可以存储
var lennon = Array();
lennon\["name"\] = "John";
lennon\["year"\] = 1940
lennon\["living"\]= false
### 对象
var lennon = \{name:"John",year:1940,living:false\};
**用对象来代替传统数组，可以通过元素的名称而不是下标数字来引用它们，大大提高了脚本的可读性。**
## 操作
### 算数操作符
\+
相加或字符串拼接
在数值与
## nodeType
nodeType属性总共有12种可选值，但其中仅有3种，它们是：元素节点（1），属性节点（2），文本节点（3）。
## 学习JavaScript/前端应当注意：
### 平稳退化
借鉴CSS，在禁用了JavaScript的情况下也能正确显示
### 合理分离
将JavaScript与表现分离
### 向后兼容
### 性能考虑
## 同源协议
### 定义及用处
协议相同
域名相同
端口相同
用途：信息安全
### 限制范围:
（1）Cookie、LocalStorage、IndexDB无法读取
（2）DOM无法获得
（3）AJAX请求不能发送
## CSS-DOM
### 三位一体的网页
   
我们在浏览器中看到的网页其实是由
