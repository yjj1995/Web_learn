- TS是JS的超集
- 新增了类型系统和**完整的面向对象**
- 使用ts编写的项目更加健硕
- 新增的语法，浏览器和nodejs都无法识别
- 需要一个工具，将TS代码转化为浏览器和nodejs识别的js代码
## TS基础
### 环境安装
- npm：是nodejs包管理器
- tsc的作用：负责将TS代码转为浏览器，nodejs识别- 的js代码
### 总结
- 1. 在后缀名为.ts的文件中书写typescript代码
- 2. 使用tsc工具将typescript代码编译为浏览器，nodejs识别的js代码
- 3. 在浏览器或者nodejs中执行js代码
- 安装ts-node 使用ts-node 文件名.ts
### 数据类型

1. 变量(var js)
TS规定，声明的时候必须指定变量的数据类型
2. 语法
let 变量名：变量类型；

let age: number;
let myName: string;

- 赋值符号 '=' 可以赋予变量类型
    let age: number;
    age = 18; // 正确的
    age = 'jack'; //就是错误的。
- 有变量类型限制 

### Ts兼容JS所有的数据类型
- 在javascript中，undefined和null都是变量的值，undefined代表一个未初始化的变量的值，null代表变量指向1个空对象
- 在ts中，undefined和null也是一种数据类型undefined类型的变量，只有存储undefined值null类型的变量，只有存储null值。

### undefined与null
如果一个变量的类型是undefined类型，那么这个变量的值只能取undefined
如果一个变量的类型是null类型，那么这个变量的值只取null

- 因为undefined和null是其它类型的子类，所以这两个变量的值可以赋值给其他类型的变量。

### 联合类型
- let 变量名 数据类型|数据类型2;
变量的取值，可以是两种类型中的任意一种。
'let result: string | number'

### any 类型
any 类型的变量，可以存储任意类型的数据。

