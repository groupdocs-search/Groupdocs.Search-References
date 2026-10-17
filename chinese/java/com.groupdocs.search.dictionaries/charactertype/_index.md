---
title: "CharacterType"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "表示字符的类型，取决于其应如何被索引。"
type: docs
weight: 24
url: /zh/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

表示字符的类型，取决于其索引方式。

## Fields

| Field | 描述 |
| --- | --- |
|  | [Separator](#Separator) | 分隔符字符。 |
|
|  | [Letter](#Letter) | 有效字符。 |
|
|  | [Blended](#Blended) | 分隔符和有效字符两者。 |
|
|  | [SeparateWord](#SeparateWord) | 表示完整单词的字符。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


分隔符字符。


### Letter {#Letter}
```
public static final CharacterType Letter
```


有效字符。


### Blended {#Blended}
```
public static final CharacterType Blended
```


分隔符和有效字符两者。


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


表示完整单词的字符。


### values() {#values--}
```
public static CharacterType[] values()
```




**Returns:**
com.groupdocs.search.dictionaries.CharacterType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static CharacterType valueOf(String name)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
