---
title: "CharacterType"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет тип символа в зависимости от того, как его следует индексировать."
type: docs
weight: 24
url: /ru/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Представляет тип символа в зависимости от того, как он должен быть проиндексирован.

## Fields

| Field | Описание |
| --- | --- |
|  | [Separator](#Separator) | Разделительный символ. |
|
|  | [Letter](#Letter) | Допустимый символ. |
|
|  | [Blended](#Blended) | И разделительный, и допустимый символ. |
|
|  | [SeparateWord](#SeparateWord) | Символ, представляющий целое слово. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Разделительный символ.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Допустимый символ.


### Blended {#Blended}
```
public static final CharacterType Blended
```


И разделительный, и допустимый символ.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Символ, представляющий целое слово.


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
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
