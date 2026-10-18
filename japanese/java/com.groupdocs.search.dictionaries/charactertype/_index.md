---
title: "CharacterType"
second_title: "GroupDocs.Search 用 Java API Reference"
description: "文字がどのようにインデックス付けされるかに応じた文字タイプを表します。"
type: docs
weight: 24
url: /ja/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

インデックス方法に応じた文字のタイプを表します。

## Fields

| Field | 説明 |
| --- | --- |
|  | [Separator](#Separator) | 区切り文字。 |
|
|  | [Letter](#Letter) | 有効な文字。 |
|
|  | [Blended](#Blended) | 区切り文字と有効な文字の両方。 |
|
|  | [SeparateWord](#SeparateWord) | 単語全体を表す文字。 |
|
## メソッド

| メソッド | 説明 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


区切り文字。


### Letter {#Letter}
```
public static final CharacterType Letter
```


有効な文字。


### Blended {#Blended}
```
public static final CharacterType Blended
```


区切り文字と有効な文字の両方。


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


単語全体を表す文字。


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
| パラメーター | タイプ | 説明 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
