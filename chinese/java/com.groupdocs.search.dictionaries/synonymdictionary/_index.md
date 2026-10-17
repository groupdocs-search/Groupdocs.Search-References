---
title: "SynonymDictionary"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义同义词字典的接口。"
type: docs
weight: 23
url: /zh/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

定义同义词字典的接口。


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取此 SynonymDictionary 中包含的单词数量。 |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | 将指定的同义词组集合添加到此 SynonymDictionary 实例中。 |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | 将指定的同义词组集合添加到此 SynonymDictionary 实例中。 |
|
|  | [clear()](#clear--) | 从此 SynonymDictionary 对象中移除所有单词。 |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | 获取指定单词的同义词。 |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | 获取指定单词所属的所有同义词组。 |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | 获取此词典中包含的所有同义词组。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取此 SynonymDictionary 中包含的单词数量。


**Returns:**
int - 此 SynonymDictionary 中包含的单词数量。

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


将指定的同义词组集合添加到此 SynonymDictionary 实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 同义词 | java.lang.Iterable<java.lang.String[]> | 要添加到词典的同义词组集合。 |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


将指定的同义词组集合添加到此 SynonymDictionary 实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 同义词 | java.lang.String[][] | 要添加到词典的同义词组集合。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


从此 SynonymDictionary 对象中移除所有单词。


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


获取指定单词的同义词。生成的数组不包含原始单词。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 单词 | java.lang.String | 用于建议同义词的单词。 |
|

**Returns:**
java.lang.String[] - 指定单词的同义词，若此 SynonymDictionary 对象不包含该单词，则返回空数组。

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


获取指定单词所属的所有同义词组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 单词 | java.lang.String | 用于获取同义词组的词。 |
|

**Returns:**
java.lang.String[][] - 指定词所属的所有同义词组。

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


获取此词典中包含的所有同义词组。


**Returns:**
java.lang.String[][] - 所有同义词组。

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.String> - 可用于遍历集合的迭代器。

