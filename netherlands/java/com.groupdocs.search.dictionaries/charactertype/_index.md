---
title: "CharacterType"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een type teken voor, afhankelijk van hoe het moet worden geïndexeerd."
type: docs
weight: 24
url: /nl/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Stelt een type teken voor, afhankelijk van hoe het moet worden geïndexeerd.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Separator](#Separator) | Het scheidingsteken. |
|
|  | [Letter](#Letter) | Het geldige teken. |
|
|  | [Blended](#Blended) | Zowel het scheidingsteken als het geldige teken. |
|
|  | [SeparateWord](#SeparateWord) | Het teken dat een heel woord vertegenwoordigt. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Het scheidingsteken.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Het geldige teken.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Zowel het scheidingsteken als het geldige teken.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Het teken dat een heel woord vertegenwoordigt.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
