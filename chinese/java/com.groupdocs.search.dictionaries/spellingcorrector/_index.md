---
title: "拼写校正器"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义查询中术语的拼写纠正器的接口。"
type: docs
weight: 21
url: /zh/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

定义查询中术语的拼写纠正器的接口。


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取此 SpellingCorrector 中包含的单词数量。 |
|
|  | [getWords()](#getWords--) | 获取当前包含在此 SpellingCorrector 中的单词集合。 |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | 将指定的词集合添加到此 SpellingCorrector 实例中。 |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | 将指定的词集合添加到此 SpellingCorrector 实例中。 |
|
|  | [clear()](#clear--) | 从 SpellingCorrector 对象中移除所有词。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取此 SpellingCorrector 中包含的单词数量。


**Returns:**
int - 此 SpellingCorrector 包含的词数。

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


获取当前包含在此 SpellingCorrector 中的单词集合。


**Returns:**
java.lang.String[] - 词的集合。

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


将指定的词集合添加到此 SpellingCorrector 实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词 | java.lang.Iterable<java.lang.String> | 要添加到字典中的词集合。 |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


将指定的词集合添加到此 SpellingCorrector 实例中。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 词 | java.lang.String[] | 要添加到字典中的词集合。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


从 SpellingCorrector 对象中移除所有词。


