---
title: "CharacterType"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Bir karakterin nasıl indekslenmesi gerektiğine bağlı olarak karakter tipini temsil eder."
type: docs
weight: 24
url: /tr/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Bir karakterin tipini, nasıl indekslenmesi gerektiğine bağlı olarak temsil eder.

## Alanlar

| Alan | Açıklama |
| --- | --- |
|  | [Separator](#Separator) | Ayırıcı karakter. |
|
|  | [Letter](#Letter) | Geçerli karakter. |
|
|  | [Blended](#Blended) | Hem ayırıcı hem de geçerli karakter. |
|
|  | [SeparateWord](#SeparateWord) | Tam bir kelimeyi temsil eden karakter. |
|
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Ayırıcı karakter.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Geçerli karakter.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Hem ayırıcı hem de geçerli karakter.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Tam bir kelimeyi temsil eden karakter.


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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
