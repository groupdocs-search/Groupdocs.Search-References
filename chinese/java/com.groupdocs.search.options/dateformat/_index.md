---
title: "DateFormat"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示日期格式。"
type: docs
weight: 13
url: /zh/java/com.groupdocs.search.options/dateformat/
---
**Inheritance:**
java.lang.Object
```
public class DateFormat
```

表示日期格式。


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)


此示例演示了该类的典型用法。

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "daterange(2017-01-01 ~~ 2019-12-31)";
Index index = new Index(indexFolder); // 在指定文件夹中创建索引
index.add(documentsFolder); // 从指定文件夹索引文档
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // 删除默认日期格式
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getDateSeparator(),
DateFormatElement.getYearFourDigits(),
};
// 创建日期格式模式 'MM/dd/yyyy'
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // 在索引中搜索
 
```
 
````


## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [DateFormat(String cultureName, DateFormatElement[] formatElements)](#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---) | 初始化 DateFormat 类的新实例。 |
|
|  | [DateFormat(DateFormatElement[] formatElements, String dateSeparator)](#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-) | 初始化 DateFormat 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getDateSeparator()](#getDateSeparator--) | 获取日期分隔符。 |
|
|  | [toString()](#toString--) | 返回表示当前 DateFormat 的字符串。 |
|
| [getCore()](#getCore--) |  |
### DateFormat(String cultureName, DateFormatElement[] formatElements) {#DateFormat-java.lang.String-com.groupdocs.search.options.DateFormatElement---}
```
public DateFormat(String cultureName, DateFormatElement[] formatElements)
```


初始化 DateFormat 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | cultureName | java.lang.String | 文化名称。 |
|
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | 格式元素。 |
|

### DateFormat(DateFormatElement[] formatElements, String dateSeparator) {#DateFormat-com.groupdocs.search.options.DateFormatElement---java.lang.String-}
```
public DateFormat(DateFormatElement[] formatElements, String dateSeparator)
```


初始化 DateFormat 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | formatElements | [DateFormatElement\[\]](../../com.groupdocs.search.options/dateformatelement) | 格式元素。 |
|
|  | dateSeparator | java.lang.String | 日期分隔符。 |
|

### getDateSeparator() {#getDateSeparator--}
```
public String getDateSeparator()
```


获取日期分隔符。


**Returns:**
java.lang.String - 日期分隔符。

### toString() {#toString--}
```
public String toString()
```


返回表示当前 DateFormat 的字符串。


**Returns:**
java.lang.String - 表示当前 DateFormat 的字符串。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
