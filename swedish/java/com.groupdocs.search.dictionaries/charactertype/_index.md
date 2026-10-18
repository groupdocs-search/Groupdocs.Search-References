---
title: "CharacterType"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en typ av tecken beroende på hur det ska indexeras."
type: docs
weight: 24
url: /sv/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Representerar en typ av tecken, beroende på hur det ska indexeras.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Separator](#Separator) | Separatortecknet. |
|
|  | [Letter](#Letter) | Det giltiga tecknet. |
|
|  | [Blended](#Blended) | Både separatorn och det giltiga tecknet. |
|
|  | [SeparateWord](#SeparateWord) | Tecknet som representerar ett helt ord. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Separatortecknet.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Det giltiga tecknet.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Både separatorn och det giltiga tecknet.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Tecknet som representerar ett helt ord.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
