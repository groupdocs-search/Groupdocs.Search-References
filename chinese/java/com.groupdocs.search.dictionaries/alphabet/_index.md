---
title: "字母表"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义在索引期间用于检测字符类型的字符字典的接口。"
type: docs
weight: 15
url: /zh/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

定义字符字典的接口，该字典在索引期间用于检测字符类型。每个字符可以被视为分隔符、字母或两者兼有。


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | 获取字符的类型。 |
|
|  | [getCount()](#getCount--) | 获取 Alphabet 中包含的字符数量。 |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | 在此 Alphabet 实例中，为指定集合的每个字符设置类型。 |
|
|  | [clear()](#clear--) | 为此 Alphabet 中的所有字符设置 CharacterType.Separator 类型。 |
|
|  | [iterator()](#iterator--) | 返回一个遍历集合的迭代器。 |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


获取字符的类型。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字符 | char | 用于获取类型的字符。 |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


获取 Alphabet 中包含的字符数量。


**Returns:**
int - 字典中字符的数量。

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


在此 Alphabet 实例中，为指定集合的每个字符设置类型。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 字符 | char[] | 用于设置类型的字符集合。 |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | 字符类型。 |
|

### clear() {#clear--}
```
public abstract void clear()
```


为此 Alphabet 中的所有字符设置 CharacterType.Separator 类型。


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


返回一个遍历集合的迭代器。


**Returns:**
java.util.Iterator<java.lang.Character> - 可用于遍历集合的迭代器。

