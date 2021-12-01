## JSON教程

### 什么是JSON
- JSON是JavaScript Object Notation的简称，中文含义为“JavaScript 对象表示法”，它是一种数据交换的文本格式，而不是一种编程语言。
- JSON 是一种轻量级的数据交换格式，它基于 ECMAScript (w3c制定的js规范)的一个子集，采用完全独立于编程语言的文本格式来存储和表示数据。简洁和清晰的层次结构使得 JSON 成为理想的数据交换语言。易于人阅读和编写，同时也易于机器解析和生成，并有效地提升网络传输效率。

### JSON特点  
- JSON 主要具有以下特性，这些特性使它成为理想的数据交换语言：
  * JSON 是轻量级的文本数据交换格式
  * JSON 具有自我描述性，更易理解
  * JSON 采用完全独立于语言的文本格式：JSON 使用 JavaScript 语法来描述数据对象，但是 JSON 仍然独立于语言和平台。JSON 解析器和 JSON 库支持许多不同的编程语言。 目前常见的动态编程语言（PHP，JSP，.NET）都支持JSON。
  * JSON 是存储和交换文本信息的一种语法，它与XML具有相同的特性，是一种数据存储格式，却比 XML 更小、更快、 更易于人编写和阅读、更易于生成和解析。

### 类似于 XML 的特性：

  * JSON 是纯文本
  * JSON 具有“自我描述性”（人类可读）
  * JSON 具有层级结构（值中存在值）
  * JSON 可通过 JavaScript 进行解析
  * JSON 数据可使用 AJAX 进行传输

### 相比 XML 的不同之处：

  * 没有结束标签
  * 更短
  * 读写的速度更快
  * 能够使用内建的 JavaScript eval() 方法进行解析
  * 使用数组
  * 不使用保留字

## JSON语法  
- JSON 语法是 JavaScript 语法的子集。

## JSON 语法规则  
- JSON 语法是 JavaScript 对象表示语法的子集。  
* 数据在名称/值对中
* 数据由逗号分隔
* 大括号 {} 保存对象
* 中括号 [] 保存数组，数组可以包含多个对象

## JSON 名称/值对  
- JSON 数据的书写格式是:  
`key : value`  
- 名称/值对包括字段名称（在双引号中），后面写一个冒号，然后是值：  
`"name" : "abc"`

## JSON 值  
- JSON 值可以是:  
* 数字（整数或浮点数）
* 字符串（在双引号中）
* 逻辑值（true 或 false）
* 数组（在中括号中）
* 对象（在大括号中）
* null

## JSON 数字  
- JSON 数字可以是整型或者浮点型:  
`{ "age":30 }`

## JSON 对象  
- JSON 对象在大括号 {} 中书写:  
`{key1 : value1, key2 : value2, ... keyN : valueN }`  
- 对象可以包含多个名称/值对:  
`{ "name":"abc" , "url":"def" }`  

## JSON 对象语法  
- 实例
```
{ "name":"jsontools", "alexa":10000, "site":null }
```
* JSON 对象使用在大括号({})中书写。
* 对象可以包含多个 key/value（键/值）对。
* key 必须是字符串，value 可以是合法的 JSON 数据类型（字符串, 数字, 对象, 数组, 布尔值或 null）。
* key 和 value 中使用冒号(:)分割。
* 每个 key/value 对使用逗号(,)分割。

## JSON 数组
- JSON 数组在中括号 [] 中书写：

数组可包含多个对象：
```
[
    { key1 : value1-1 , key2:value1-2 }, 
    { key1 : value2-1 , key2:value2-2 }, 
    { key1 : value3-1 , key2:value3-2 }, 
    ...
    { keyN : valueN-1 , keyN:valueN-2 }, 
]
```
```
{
    "sites": [
        { "name":"jsontools" , "url":"www.jsontools.com" }, 
        { "name":"google" , "url":"www.google.com" }, 
        { "name":"微博" , "url":"www.weibo.com" }
    ]
}
```
在上面的例子中，对象 sites 是包含三个对象的数组。每个对象代表一条关于某个网站（name、url）的记录。

## JSON 语法数组  
- 实例
```
[ "Google", "jsontools", "Taobao" ]
```
* JSON 数组在中括号中书写。
* JSON 中数组值必须是合法的 JSON 数据类型（字符串, 数字, 对象, 数组, 布尔值或 null）。
* JavaScript 中，数组值可以是以上的 JSON 数据类型，也可以是 JavaScript 的表达式，包括函数，日期，及 undefined。

## JSON 对象中的数组
- 实例
```
{
    "name":"网站",
    "num":3,
    "sites":[ "Google", "jsontools", "Taobao" ]
}
```
- 也可这样写
```
{
    "name":"网站",
    "num":3,
    "sites":[ 
        "Google", 
        "jsontools", 
        "Taobao" 
    ]
}
```

## JSON 布尔值  
- JSON 布尔值可以是 true 或者 false：
`{ "flag":true }`

## JSON null  
- JSON 可以设置 null 值：
`{ "jsontools":null }`
