# JavaScript学习笔记

###### 简称JS，是一种轻量级、解释型、面向对象的客户端脚本语言，可以直接嵌入HTML，主要用于在网页上实现动态效果，增加交互性，语法比较灵活。

###### -冯礼盈

## 学习背景

##### 对JavaScript进行了解和学习。

## 学习内容的目录

- [JavaScript的作用](#JavaScript的作用)
- [JavaScript的导入方式](#JavaScript的导入方式)
- [JavaScript的基本语法](#JavaScript的基本语法)
- [DOM（Document Object Model）](#DOM（Document Object Model）)

## 学习内容

### JavaScript的作用

- ##### 客户端脚本：用于在浏览器中执行，实现动态效果和增强用户交互。

- ##### 网页开发：与HTML和CSS协同开发网页。

- ##### 后端开发：使用Node.js,JavaScript可以在服务器端运行，从而实现开发。

### JavaScript的导入方式

- ##### 内联式：在HTML文件中直接嵌入JS代码，放在script标签内，而script标签可以在head部分也可以在boby部分。

- ##### 外部引入：把JS代码保存在单独的外部文件中，通过script标签的src属性引入（scr="./文件夹/文件名"）。

##### console.log('输入内容')，也可以通过log加Tab键快速生成

###### console是控制台，浏览器中F12

##### alert——弹窗

### JavaScript的基本语法

#### 变量

- ##### var（全名variable）：声明正常变量，具有函数作用域，尽量避免使用。

- ##### let：声明正常变量，具有块级作用域，更安全更灵活。

- ##### const：声明常量，一般不会轻易改变。

#### 数据类型

- ##### undefind：表示变量声明但没有初始化或对象属性不存在或函数无返回值，变量可能在将来被赋值或者某个值还没有被计算出来。

- ##### null：表示变量被明确赋值为空或者不存在了，是一个被赋予的值，表示空对象引用或者没有对象值。

#### JavaScript的控制语句

- ##### 条件语句：使用if、else if（用于在上一个if语句条件为假，可以有多个）、else三个关键字。

- ##### 循环语句：for循环、while循环、break和continue

#### 函数

###### 一段可重复使用的代码块，接受输入、执行并返回输出。

- ##### function：声明一个函数	

  ###### function 函数名（参数1，参数2…）//参数可以不写，表示不传参{

###### 	return 返回值；

###### 	}

- ##### 作用域：全局作用域（函数外部声明）和局部作用域（函数内部声明）

#### 事件

###### 文档或浏览器窗口中发生的特定瞬间

|    事件     |       描述       |
| :---------: | :--------------: |
|   onClick   |     点击事件     |
| onMouseOver |     鼠标经过     |
| onMouseOut  |     鼠标移出     |
|  onChange   | 文本内容改变事件 |
|  onSelect   |    文本框选中    |
|   onFocus   |     光标聚集     |
|   onBlur    |     移开光标     |

##### 事件绑定

- ##### HTML属性

- ##### DOM属性

- ##### addEventListener方法

### DOM（Document Object Model）

##### 当页面被加载时，浏览器会创建页面的文档对象模型DOM，DOM为HTML提供了一个编程接口（DOM API），允许开发者通过JS与HTML文档进行交互改变。

#### DOM获取元素节点

##### getElementByID（获取元素唯一）、getElementsByClassName、getElementsByName、getElementsByTagName、getElementsByTagNAmeNS

## 参考资料

#### DOM对象常用方法

| 方法              | 描述                             |
| ----------------- | -------------------------------- |
| appendChild()     | 把新的子节点添加到指定节点。     |
| removeChild()     | 删除子节点。                     |
| replaceChild()    | 替换子节点。                     |
| insertBefore()    | 在指定子节点前面插入新的子节点。 |
| createAttribute() | 创建属性节点。                   |
| createElement()   | 创建元素节点。                   |
| creatTextNode()   | 创建文本节点。                   |
| getAttribute()    | 返回指定的属性值。               |

## 参考资料

##### B站视频[3小时前端入门教程（HTML+CSS+JS）](https://www.bilibili.com/video/BV1BT4y1W7Aw?spm_id_from=333.788.player.switch&vd_source=a78069782a9aa4e8a2dd04738f67b492&p=8)