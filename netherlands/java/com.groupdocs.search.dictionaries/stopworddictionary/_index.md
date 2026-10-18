---
title: "StopWordDictionary"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een woordenboek van stopwoorden."
type: docs
weight: 22
url: /nl/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Definieert de interface van een woordenboek van stopwoorden.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal stopwoorden op dat in de StopWordDictionary zit. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Voegt de opgegeven verzameling woorden toe aan deze instantie van de StopWordDictionary. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Voegt de opgegeven verzameling woorden toe aan deze instantie van de StopWordDictionary. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Verwijdert de opgegeven verzameling woorden uit deze instantie van de StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Verwijdert de opgegeven verzameling woorden uit deze instantie van de StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Bepaalt of een StopWordDictionary-object het opgegeven woord bevat. |
|
|  | [clear()](#clear--) | Verwijdert alle woorden uit een StopWordDictionary-object. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal stopwoorden op dat in de StopWordDictionary zit.


**Returns:**
int - Het aantal stopwoorden in het woordenboek.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Voegt de opgegeven verzameling woorden toe aan deze instantie van de StopWordDictionary.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woorden | java.lang.Iterable<java.lang.String> | De verzameling woorden om toe te voegen aan het woordenboek. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Voegt de opgegeven verzameling woorden toe aan deze instantie van de StopWordDictionary.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woorden | java.lang.String[] | De verzameling woorden om toe te voegen aan het woordenboek. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Verwijdert de opgegeven verzameling woorden uit deze instantie van de StopWordDictionary.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woorden | java.lang.Iterable<java.lang.String> | De verzameling woorden om te verwijderen. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Verwijdert de opgegeven verzameling woorden uit deze instantie van de StopWordDictionary.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woorden | java.lang.String[] | De verzameling woorden om te verwijderen. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Bepaalt of een StopWordDictionary-object het opgegeven woord bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woord | java.lang.String | Het woord om te zoeken in het StopWordDictionary-object. |
|

**Returns:**
boolean - true als het StopWordDictionary-object het opgegeven woord bevat; anders false.

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle woorden uit een StopWordDictionary-object.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.String> - Een iterator die kan worden gebruikt om door de collectie te itereren.

