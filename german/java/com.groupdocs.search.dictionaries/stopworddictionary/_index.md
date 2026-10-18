---
title: "StopWordDictionary"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Wörterbuchs für Stoppwörter."
type: docs
weight: 22
url: /de/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Definiert die Schnittstelle eines Wörterbuchs für Stoppwörter.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Gibt die Anzahl der Stoppwörter zurück, die im StopWordDictionary enthalten sind. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des StopWordDictionary hinzu. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des StopWordDictionary hinzu. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Entfernt die angegebene Sammlung von Wörtern aus dieser Instanz des StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Entfernt die angegebene Sammlung von Wörtern aus dieser Instanz des StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Bestimmt, ob ein StopWordDictionary-Objekt das angegebene Wort enthält. |
|
|  | [clear()](#clear--) | Entfernt alle Wörter aus einem StopWordDictionary-Objekt. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gibt die Anzahl der Stoppwörter zurück, die im StopWordDictionary enthalten sind.


**Returns:**
int - Die Anzahl der Stoppwörter im Wörterbuch.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des StopWordDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wörter | java.lang.Iterable<java.lang.String> | Die Sammlung von Wörtern, die dem Wörterbuch hinzugefügt werden sollen. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Fügt die angegebene Sammlung von Wörtern zu dieser Instanz des StopWordDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wörter | java.lang.String[] | Die Sammlung von Wörtern, die dem Wörterbuch hinzugefügt werden sollen. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Entfernt die angegebene Sammlung von Wörtern aus dieser Instanz des StopWordDictionary.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wörter | java.lang.Iterable<java.lang.String> | Die Sammlung von Wörtern, die entfernt werden sollen. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Entfernt die angegebene Sammlung von Wörtern aus dieser Instanz des StopWordDictionary.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wörter | java.lang.String[] | Die Sammlung von Wörtern, die entfernt werden sollen. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Bestimmt, ob ein StopWordDictionary-Objekt das angegebene Wort enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wort | java.lang.String | Das Wort, das im StopWordDictionary-Objekt gefunden werden soll. |
|

**Returns:**
boolean - true, wenn das StopWordDictionary-Objekt das angegebene Wort enthält; andernfalls false.

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Wörter aus einem StopWordDictionary-Objekt.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.String> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

