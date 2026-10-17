---
title: "StopWordDictionary"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义停用词字典的接口。"
type: docs
weight: 22
url: /zh/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

定义停用词字典的接口。


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取 StopWordDictionary 中包含的停用词数量。 |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | 将指定的词集合添加到此 StopWordDictionary 实例中。 |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | 将指定的词集合添加到此 StopWordDictionary 实例中。 |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | 从此 StopWordDictionary 实例中移除指定的词集合。 |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | 从此 StopWordDictionary 实例中移除指定的词集合。 |
|
|  | [contains(String word)](#contains-java.lang.String-) | 确定 StopWordDictionary 对象是否包含指定的词。 |
|
|  | [clear()](#clear--) | 从 StopWordDictionary 对象中移除所有词。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取 StopWordDictionary 中包含的停用词数量。


**Returns:**
int - 字典中停用词的数量。

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


将指定的词集合添加到此 StopWordDictionary 实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词 | java.lang.Iterable<java.lang.String> | 要添加到字典中的词集合。 |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


将指定的词集合添加到此 StopWordDictionary 实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词 | java.lang.String[] | 要添加到字典中的词集合。 |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


从此 StopWordDictionary 实例中移除指定的词集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词 | java.lang.Iterable<java.lang.String> | 要移除的词集合。 |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


从此 StopWordDictionary 实例中移除指定的词集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词 | java.lang.String[] | 要移除的词集合。 |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


确定 StopWordDictionary 对象是否包含指定的词。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 单词 | java.lang.String | 在 StopWordDictionary 对象中定位的词。 |
|

**Returns:**
boolean - 如果 StopWordDictionary 对象包含指定的词则为 true；否则为 false。

### clear() {#clear--}
```
public abstract void clear()
```


从 StopWordDictionary 对象中移除所有词。


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.String> - 可用于遍历集合的迭代器。

