---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示属性更改的容器。"
type: docs
weight: 10
url: /zh/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

表示属性更改的容器。


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | 初始化 AttributeChangeBatch 类的新实例。 |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | 初始化 AttributeChangeBatch 类的新实例。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | 将指定属性添加到指定的已索引文档中。 |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | 将指定属性添加到指定的已索引文档中。 |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | 将指定属性添加到索引中的所有文档。 |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | 从指定的已索引文档中移除指定属性。 |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | 从指定的已索引文档中移除指定属性。 |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | 从指定的已索引文档中移除所有属性。 |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | 从指定的已索引文档中移除所有属性。 |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | 从索引中的所有文档中移除指定属性。 |
|
|  | [clear()](#clear--) | 从索引中的所有文档中移除所有属性。 |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


初始化 AttributeChangeBatch 类的新实例。


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


初始化 AttributeChangeBatch 类的新实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 数据 | java.lang.Object | 序列化的数据。 |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


将指定属性添加到指定的已索引文档中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 文档路径。 |
|
|  | 属性 | java.lang.String[] | 要添加的属性。 |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


将指定属性添加到指定的已索引文档中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 路径 | java.lang.String[] | 文档路径。 |
|
|  | 属性 | java.lang.String[] | 要添加的属性。 |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


将指定属性添加到索引中的所有文档。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 属性 | java.lang.String[] | 要添加的属性。 |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


从指定的已索引文档中移除指定属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 文档路径。 |
|
|  | 属性 | java.lang.String[] | 要移除的属性。 |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


从指定的已索引文档中移除指定属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 路径 | java.lang.String[] | 文档路径。 |
|
|  | 属性 | java.lang.String[] | 要移除的属性。 |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


从指定的已索引文档中移除所有属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | path | java.lang.String | 文档路径。 |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


从指定的已索引文档中移除所有属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 路径 | java.lang.String[] | 文档路径。 |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


从索引中的所有文档中移除指定属性。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 属性 | java.lang.String[] | 要移除的属性。 |
|

### clear() {#clear--}
```
public void clear()
```


从索引中的所有文档中移除所有属性。


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
