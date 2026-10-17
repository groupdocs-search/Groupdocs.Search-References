---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义异形同音词字典的接口。"
type: docs
weight: 18
url: /zh/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

定义异形同音词字典的接口。


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取此  HomophoneDictionary  中包含的单词数量。 |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | 将指定的同音词组集合添加到此  HomophoneDictionary  实例中。 |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | 将指定的同音词组集合添加到此  HomophoneDictionary  实例中。 |
|
|  | [clear()](#clear--) | 从一个  HomophoneDictionary  对象中移除所有单词。 |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | 获取指定单词的同音词。 |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | 获取指定单词所属的所有同音词组。 |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | 获取此字典中包含的所有同音词组。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取此  HomophoneDictionary  中包含的单词数量。


**Returns:**
int - 单词数量。

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


将指定的同音词组集合添加到此  HomophoneDictionary  实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | 要添加到字典的同音词组集合。 |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


将指定的同音词组集合添加到此  HomophoneDictionary  实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | 要添加到字典的同音词组集合。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


从一个  HomophoneDictionary  对象中移除所有单词。


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


获取指定单词的同音词。生成的数组不包含原始单词。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 单词 | java.lang.String | 用于建议同音词的单词。 |
|

**Returns:**
java.lang.String[] - 指定单词的同音词；如果 HomophoneDictionary 对象不包含该单词，则返回空数组。

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


获取指定单词所属的所有同音词组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 单词 | java.lang.String | 用于获取同音词组的单词。 |
|

**Returns:**
java.lang.String[][] - 指定单词所属的所有同音词组。

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


获取此字典中包含的所有同音词组。


**Returns:**
java.lang.String[][] - 所有同音词组。

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.String> - 可用于遍历集合的迭代器。

