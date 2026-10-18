---
title: "CharacterType"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Typ eines Zeichens dar, abhängig davon, wie er indiziert werden soll."
type: docs
weight: 24
url: /de/java/com.groupdocs.search.dictionaries/charactertype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum CharacterType extends Enum<CharacterType>
```

Stellt einen Zeichentyp dar, abhängig davon, wie er indiziert werden soll.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Separator](#Separator) | Das Trennzeichen. |
|
|  | [Letter](#Letter) | Das gültige Zeichen. |
|
|  | [Blended](#Blended) | Sowohl das Trennzeichen als auch das gültige Zeichen. |
|
|  | [SeparateWord](#SeparateWord) | Das Zeichen, das ein ganzes Wort darstellt. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separator {#Separator}
```
public static final CharacterType Separator
```


Das Trennzeichen.


### Letter {#Letter}
```
public static final CharacterType Letter
```


Das gültige Zeichen.


### Blended {#Blended}
```
public static final CharacterType Blended
```


Sowohl das Trennzeichen als auch das gültige Zeichen.


### SeparateWord {#SeparateWord}
```
public static final CharacterType SeparateWord
```


Das Zeichen, das ein ganzes Wort darstellt.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype)
