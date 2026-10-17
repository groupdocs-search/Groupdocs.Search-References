---
title: "PasswordDictionary"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义文档密码字典的接口。"
type: docs
weight: 20
url: /zh/java/com.groupdocs.search.dictionaries/passworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface PasswordDictionary extends DictionaryBase, Iterable<String>
```

定义文档密码字典的接口。


**Learn more**

* [Indexing password protected documents](../https://docs.groupdocs.com/display/searchjava/Indexing+password+protected+documents)
* [Managing document passwords](../https://docs.groupdocs.com/display/searchjava/Document+passwords)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取字典中包含的元素数量。 |
|
|  | [getPassword(String filePath)](#getPassword-java.lang.String-) | 获取文件的密码。 |
|
|  | [clear()](#clear--) | 从此  PasswordDictionary  对象中移除所有密码。 |
|
|  | [contains(String filePath)](#contains-java.lang.String-) | 确定字典是否包含指定文档的密码。 |
|
|  | [add(String filePath, String password)](#add-java.lang.String-java.lang.String-) | 向字典中添加文档的密码。 |
|
|  | [remove(String filePath)](#remove-java.lang.String-) | 从字典中移除指定文档的密码。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取字典中包含的元素数量。


**Returns:**
int - 字典中包含的元素数量。

### getPassword(String filePath) {#getPassword-java.lang.String-}
```
public abstract String getPassword(String filePath)
```


获取文件的密码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 文件路径。 |
|

**Returns:**
java.lang.String - 文件的密码。

### clear() {#clear--}
```
public abstract void clear()
```


从此  PasswordDictionary  对象中移除所有密码。


### contains(String filePath) {#contains-java.lang.String-}
```
public abstract boolean contains(String filePath)
```


确定字典是否包含指定文档的密码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 文档文件路径。 |
|

**Returns:**
boolean -  true  如果字典包含该文档的密码；否则为  false 。

### add(String filePath, String password) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String filePath, String password)
```


向字典中添加文档的密码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 文档文件路径。 |
|
|  | 密码 | java.lang.String | 文档密码。 |
|

### remove(String filePath) {#remove-java.lang.String-}
```
public abstract boolean remove(String filePath)
```


从字典中移除指定文档的密码。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 文件路径 | java.lang.String | 文档文件路径。 |
|

**Returns:**
boolean -  true  如果密码成功移除；否则为  false 。如果在字典中未找到  filePath ，此方法也返回  false 。

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.String> - 可用于遍历集合的迭代器。

