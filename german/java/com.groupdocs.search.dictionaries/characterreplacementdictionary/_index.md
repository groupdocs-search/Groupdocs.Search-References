---
title: "CharacterReplacementDictionary"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Zeichenersetzungswörterbuchs, das während des Indizierungsprozesses verwendet wird."
type: docs
weight: 16
url: /de/java/com.groupdocs.search.dictionaries/characterreplacementdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface CharacterReplacementDictionary extends DictionaryBase, Iterable<Character>
```

Definiert die Schnittstelle eines Zeichenersetzungswörterbuchs, das während des Indexierungsprozesses verwendet wird. Zeichenersetzung kann beispielsweise verwendet werden, um Akzente von akzentuierten Zeichen zu entfernen oder einen case‑insensitiven Index zu erstellen.


**Learn more**

* [Character replacement during Indexing](../https://docs.groupdocs.com/display/searchjava/Character+replacement+during+Indexing)
* [Managing character replacements](../https://docs.groupdocs.com/display/searchjava/Character+replacements)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Liest die Anzahl der in diesem  CharacterReplacementDictionary  enthaltenen Zeichen. |
|
|  | [addRange(Iterable<CharacterReplacementPair> characterReplacements)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--) | Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des  CharacterReplacementDictionary  hinzu. |
|
|  | [addRange(CharacterReplacementPair[] characterReplacements)](#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---) | Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des  CharacterReplacementDictionary  hinzu. |
|
|  | [removeRange(char[] characters)](#removeRange-char---) | Entfernt die angegebene Sammlung von Zeichenersetzungen aus dieser Instanz des  CharacterReplacementDictionary . |
|
|  | [contains(char character)](#contains-char-) | Bestimmt, ob ein  CharacterReplacementDictionary  Objekt eine Ersetzung für das angegebene Zeichen enthält. |
|
|  | [getReplacement(char character)](#getReplacement-char-) | Liefert eine Ersetzung für das angegebene Zeichen. |
|
|  | [clear()](#clear--) | Entfernt alle Zeichenersetzungen aus einem  CharacterReplacementDictionary  Objekt. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Liest die Anzahl der in diesem  CharacterReplacementDictionary  enthaltenen Zeichen.


**Returns:**
int - Die Anzahl der Zeichen im Wörterbuch.

### addRange(Iterable<CharacterReplacementPair> characterReplacements) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.CharacterReplacementPair--}
```
public abstract void addRange(Iterable<CharacterReplacementPair> characterReplacements)
```


Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des  CharacterReplacementDictionary  hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | characterReplacements | java.lang.Iterable<com.groupdocs.search.dictionaries.CharacterReplacementPair> | Die Sammlung von Zeichenersetzungen, die dem Wörterbuch hinzugefügt werden soll. |
|

### addRange(CharacterReplacementPair[] characterReplacements) {#addRange-com.groupdocs.search.dictionaries.CharacterReplacementPair---}
```
public abstract void addRange(CharacterReplacementPair[] characterReplacements)
```


Fügt die angegebene Sammlung von Zeichenersetzungen zu dieser Instanz des  CharacterReplacementDictionary  hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | characterReplacements | [CharacterReplacementPair\[\]](../../com.groupdocs.search.dictionaries/characterreplacementpair) | Die Sammlung von Zeichenersetzungen, die dem Wörterbuch hinzugefügt werden soll. |
|

### removeRange(char[] characters) {#removeRange-char---}
```
public abstract void removeRange(char[] characters)
```


Entfernt die angegebene Sammlung von Zeichenersetzungen aus dieser Instanz des  CharacterReplacementDictionary .


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeichen | char[] | Die Sammlung von Zeichen, die entfernt werden sollen. |
|

### contains(char character) {#contains-char-}
```
public abstract boolean contains(char character)
```


Bestimmt, ob ein  CharacterReplacementDictionary  Objekt eine Ersetzung für das angegebene Zeichen enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeichen | char | Das Zeichen, das im  CharacterReplacementDictionary  Objekt gefunden werden soll. |
|

**Returns:**
boolean -  true  wenn das  CharacterReplacementDictionary  Objekt das angegebene Zeichen enthält; andernfalls  false .

### getReplacement(char character) {#getReplacement-char-}
```
public abstract char getReplacement(char character)
```


Liefert eine Ersetzung für das angegebene Zeichen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Zeichen | char | Das Zeichen, für das eine Ersetzung ermittelt werden soll. |
|

**Returns:**
char - Die Ersetzung für das angegebene Zeichen.

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Zeichenersetzungen aus einem  CharacterReplacementDictionary  Objekt.


### iterator() {#iterator--}
```
public abstract Iterator<Character> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.Character> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

