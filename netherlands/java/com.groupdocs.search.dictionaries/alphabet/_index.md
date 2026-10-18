---
title: "Alfabet"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een tekenwoordenboek dat tijdens het indexeren wordt gebruikt om het teken type te detecteren."
type: docs
weight: 15
url: /nl/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Definieert de interface van een tekenwoordenboek die wordt gebruikt tijdens het indexeren om het teken type te detecteren. Elk teken kan worden behandeld als scheidingsteken, als letter, of beide.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Haalt een type van een teken op. |
|
|  | [getCount()](#getCount--) | Haalt het aantal tekens op dat in het Alphabet zit. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Stelt het type in voor elk teken van de opgegeven collectie in deze instantie van het Alphabet. |
|
|  | [clear()](#clear--) | Stelt het CharacterType.Separator type in voor alle tekens in dit Alphabet. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Haalt een type van een teken op.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | teken | char | Het teken om een type op te halen. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal tekens op dat in het Alphabet zit.


**Returns:**
int - Het aantal tekens in het woordenboek.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Stelt het type in voor elk teken van de opgegeven collectie in deze instantie van het Alphabet.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekens | char[] | De collectie tekens om het type in te stellen. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Het teken type. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Stelt het CharacterType.Separator type in voor alle tekens in dit Alphabet.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.Character> - Een iterator die kan worden gebruikt om door de collectie te itereren.

