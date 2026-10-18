---
title: "CharacterType"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili tipe karakter tergantung bagaimana karakter tersebut harus diindeks."
type: docs
weight: 24
url: /id/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Mewakili tipe karakter, tergantung pada cara pengindeksannya.

## Fields

| Field | Deskripsi |
| --- | --- |
|  | [Separator](#Separator) | Karakter pemisah. |
|
|  | [Letter](#Letter) | Karakter yang valid. |
|
|  | [Blended](#Blended) | Baik pemisah maupun karakter yang valid. |
|
|  | [SeparateWord](#SeparateWord) | Karakter yang mewakili sebuah kata lengkap. |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Karakter pemisah.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Karakter yang valid.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Baik pemisah maupun karakter yang valid.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Karakter yang mewakili sebuah kata lengkap.


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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
