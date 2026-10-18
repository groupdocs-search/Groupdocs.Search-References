---
title: "Alphabet"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Zeichenwörterbuchs, das während der Indizierung zur Erkennung des Zeichentyps verwendet wird."
type: docs
weight: 15
url: /de/java/com.groupdocs.search.dictionaries/alphabet/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface Alphabet extends DictionaryBase, Iterable<Character>
```

Definiert die Schnittstelle eines Wörterbuchs von Zeichen, das beim Indexieren verwendet wird, um den Zeichentyp zu erkennen. Jedes Zeichen kann als Trennzeichen, als Buchstabe oder beides behandelt werden.


**Learn more**

* [Character types](../https://docs.groupdocs.com/display/searchjava/Character+types)
* [Managing alphabet](../https://docs.groupdocs.com/display/searchjava/Alphabet)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCharacterType(char character)](#getCharacterType-char-) | Ermittelt einen Typ eines Zeichens. |
|
|  | [getCount()](#getCount--) | Ermittelt die Anzahl der Zeichen, die im  Alphabet  enthalten sind. |
|
|  | [setRange(char[] characters, CharacterType type)](#setRange-char---com.groupdocs.search.dictionaries.CharacterType-) | Setzt den Typ für jedes Zeichen der angegebenen Sammlung in dieser Instanz des  Alphabet . |
|
|  | [clear()](#clear--) | Setzt den  CharacterType.Separator  Typ für alle Zeichen in diesem  Alphabet . |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCharacterType(char character) {#getCharacterType-char-}
```
public abstract CharacterType getCharacterType(char character)
```


Ermittelt einen Typ eines Zeichens.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeichen | char | Das Zeichen, um einen Typ zu erhalten. |
|

**Returns:**
[CharacterType](../../com.groupdocs.search.dictionaries/charactertype) - A type of the character.

### getCount() {#getCount--}
```
public abstract int getCount()
```


Ermittelt die Anzahl der Zeichen, die im  Alphabet  enthalten sind.


**Returns:**
int - Die Anzahl der Zeichen im Wörterbuch.

### setRange(char[] characters, CharacterType type) {#setRange-char---com.groupdocs.search.dictionaries.CharacterType-}
```
public abstract void setRange(char[] characters, CharacterType type)
```


Setzt den Typ für jedes Zeichen der angegebenen Sammlung in dieser Instanz des  Alphabet .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeichen | char[] | Die Sammlung von Zeichen, um den Typ festzulegen. |
|
|  | type | [CharacterType](../../com.groupdocs.search.dictionaries/charactertype) | Der Zeichentyp. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Setzt den  CharacterType.Separator  Typ für alle Zeichen in diesem  Alphabet .


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.Character> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

