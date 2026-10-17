---
title: "CharacterType"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente un type de caractère en fonction de la façon dont il doit être indexé."
type: docs
weight: 24
url: /fr/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Représente un type de caractère, en fonction de la façon dont il doit être indexé.

## Fields

| Field | Description |
| --- | --- |
|  | [Separator](#Separator) | Le caractère séparateur. |
|
|  | [Letter](#Letter) | Le caractère valide. |
|
|  | [Blended](#Blended) | À la fois le séparateur et le caractère valide. |
|
|  | [SeparateWord](#SeparateWord) | Le caractère qui représente un mot entier. |
|
## Méthodes

| Méthode | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Le caractère séparateur.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Le caractère valide.


### Blended {#Blended}
```
public static final CharacterType Blended
```


À la fois le séparateur et le caractère valide.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Le caractère qui représente un mot entier.


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
| Paramètre | Type | Description |
| --- | --- | --- |
| nom | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
