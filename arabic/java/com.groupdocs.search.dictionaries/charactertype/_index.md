---
title: "CharacterType"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نوعًا من الأحرف بناءً على كيفية فهرستها."
type: docs
weight: 24
url: /ar/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

يمثل نوعًا من الأحرف، بناءً على كيفية فهرستها.

## الحقول

| حقل | الوصف |
| --- | --- |
|  | [Separator](#Separator) | حرف الفاصل. |
|
|  | [Letter](#Letter) | الحرف الصالح. |
|
|  | [Blended](#Blended) | كلا الفاصل والحرف الصالح. |
|
|  | [SeparateWord](#SeparateWord) | الحرف الذي يمثل كلمة كاملة. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


حرف الفاصل.


### Letter {#Letter}
```
public static final CharacterType Letter
```


الحرف الصالح.


### Blended {#Blended}
```
public static final CharacterType Blended
```


كلا الفاصل والحرف الصالح.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


الحرف الذي يمثل كلمة كاملة.


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
| معامل | نوع | الوصف |
| --- | --- | --- |
| الاسم | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
