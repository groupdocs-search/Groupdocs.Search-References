---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义在索引过程中使用的字符替换字典的接口。"
type: docs
weight: 16
url: /zh/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

定义在索引过程中使用的字符替换字典的接口。例如，字符替换可用于去除带音调的字符的重音或实现不区分大小写的索引。


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCount()](#getCount--) | 获取此  CharacterReplacementDictionary  中包含的字符数量。 |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | 向此  CharacterReplacementDictionary  实例添加指定的字符替换集合。 |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | 向此  CharacterReplacementDictionary  实例添加指定的字符替换集合。 |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | 从此 CharacterReplacementDictionary 实例中移除指定的字符替换集合。 |
|
|  | [contains(char character)](#contains-char-) | 确定 CharacterReplacementDictionary 对象是否包含指定字符的替换。 |
|
|  | [getReplacement(char character)](#getReplacement-char-) | 获取指定字符的替换。 |
|
|  | [clear()](#clear--) | 从 CharacterReplacementDictionary 对象中移除所有字符替换。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


获取此  CharacterReplacementDictionary  中包含的字符数量。


**Returns:**
int - 字典中字符的数量。

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


向此  CharacterReplacementDictionary  实例添加指定的字符替换集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | 要添加到字典的字符替换集合。 |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


向此  CharacterReplacementDictionary  实例添加指定的字符替换集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | 要添加到字典的字符替换集合。 |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


从此 CharacterReplacementDictionary 实例中移除指定的字符替换集合。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字符 | char[] | 要移除的字符集合。 |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


确定 CharacterReplacementDictionary 对象是否包含指定字符的替换。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字符 | char | 在 CharacterReplacementDictionary 对象中要定位的字符。 |
|

**Returns:**
boolean - 如果 CharacterReplacementDictionary 对象包含指定字符则为 true；否则为 false。

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


获取指定字符的替换。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字符 | char | 要获取替换的字符。 |
|

**Returns:**
char - 指定字符的替换。

### clear() {#clear--}
```
public abstract void clear()
```


从 CharacterReplacementDictionary 对象中移除所有字符替换。


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.Character> - 可用于遍历集合的迭代器。

