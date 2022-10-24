---
title: CharacterType
second_title: GroupDocs.Search for Java API Reference
description: Represents a type of a character depending on how it should be indexed.
type: docs
weight: 24
url: /java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Represents a type of a character, depending on how it should be indexed.
## Fields

| Field | Description |
| --- | --- |
| [Separator](#Separator) | The separator character. |
| [Letter](#Letter) | The valid character. |
| [Blended](#Blended) | Both the separator and the valid character. |
| [SeparateWord](#SeparateWord) | The character that represents a whole word. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


The separator character.

### Letter {#Letter}
```
public static final CharacterType Letter
```


The valid character.

### Blended {#Blended}
```
public static final CharacterType Blended
```


Both the separator and the valid character.

### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


The character that represents a whole word.

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
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
