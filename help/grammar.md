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

## JSON 布尔值  
- JSON 布尔值可以是 true 或者 false：
`{ "flag":true }`

## JSON null  
- JSON 可以设置 null 值：
`{ "jsontools":null }`

