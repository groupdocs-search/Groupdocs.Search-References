---
title: "DocumentField"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示文档字段数据。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search.common/documentfield/
---
**Inheritance:**
java.lang.Object
```
public class DocumentField
```

表示文档字段数据。


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)
* [Indexing additional fields](../https://docs.groupdocs.com/display/searchjava/Indexing+additional+fields)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [DocumentField(String name, String value)](#DocumentField-java.lang.String-java.lang.String-) | 初始化 DocumentField 类的新实例。 |
|
|  | [DocumentField(Object data)](#DocumentField-java.lang.Object-) | 初始化 DocumentField 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getName()](#getName--) | 获取字段名称。 |
|
|  | [getValue()](#getValue--) | 获取字段值。 |
|
| [getCore()](#getCore--) |  |
### DocumentField(String name, String value) {#DocumentField-java.lang.String-java.lang.String-}
```
public DocumentField(String name, String value)
```


初始化 DocumentField 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 名称 | java.lang.String | 字段名称。 |
|
|  | 值 | java.lang.String | 字段值。 |
|

### DocumentField(Object data) {#DocumentField-java.lang.Object-}
```
public DocumentField(Object data)
```


初始化 DocumentField 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### getName() {#getName--}
```
public String getName()
```


获取字段名称。


**Returns:**
java.lang.String - 字段名称。

### getValue() {#getValue--}
```
public String getValue()
```


获取字段值。


**Returns:**
java.lang.String - 字段值。

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
