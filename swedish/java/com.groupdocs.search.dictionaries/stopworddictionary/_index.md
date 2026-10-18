---
title: "StopWordDictionary"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en ordbok med stoppord."
type: docs
weight: 22
url: /sv/java/com.groupdocs.search.dictionaries/stopworddictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface StopWordDictionary extends DictionaryBase, Iterable<String>
```

Definierar gränssnittet för en ordbok med stoppord.


**Learn more**

* [Indexing with stop words](../https://docs.groupdocs.com/display/searchjava/Indexing+with+stop+words)
* [Managing stop word dictionary](../https://docs.groupdocs.com/display/searchjava/Stop+word+dictionary)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet stoppord som finns i StopWordDictionary. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Lägger till den angivna samlingen av ord till den här instansen av StopWordDictionary. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Lägger till den angivna samlingen av ord till den här instansen av StopWordDictionary. |
|
|  | [removeRange(Iterable<String> words)](#removeRange-java.lang.Iterable-java.lang.String--) | Tar bort den angivna samlingen av ord från den här instansen av StopWordDictionary. |
|
|  | [removeRange(String[] words)](#removeRange-java.lang.String---) | Tar bort den angivna samlingen av ord från den här instansen av StopWordDictionary. |
|
|  | [contains(String word)](#contains-java.lang.String-) | Bestämmer om ett StopWordDictionary-objekt innehåller det angivna ordet. |
|
|  | [clear()](#clear--) | Tar bort alla ord från ett StopWordDictionary-objekt. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet stoppord som finns i StopWordDictionary.


**Returns:**
int - Antalet stoppord i ordboken.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Lägger till den angivna samlingen av ord till den här instansen av StopWordDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.Iterable<java.lang.String> | Samlingen av ord att lägga till i ordboken. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Lägger till den angivna samlingen av ord till den här instansen av StopWordDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String[] | Samlingen av ord att lägga till i ordboken. |
|

### removeRange(Iterable<String> words) {#removeRange-java.lang.Iterable-java.lang.String--}
```
public abstract void removeRange(Iterable<String> words)
```


Tar bort den angivna samlingen av ord från den här instansen av StopWordDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.Iterable<java.lang.String> | Samlingen av ord att ta bort. |
|

### removeRange(String[] words) {#removeRange-java.lang.String---}
```
public abstract void removeRange(String[] words)
```


Tar bort den angivna samlingen av ord från den här instansen av StopWordDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String[] | Samlingen av ord att ta bort. |
|

### contains(String word) {#contains-java.lang.String-}
```
public abstract boolean contains(String word)
```


Bestämmer om ett StopWordDictionary-objekt innehåller det angivna ordet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String | Ordet att leta efter i StopWordDictionary-objektet. |
|

**Returns:**
boolean - true om StopWordDictionary-objektet innehåller det angivna ordet; annars false.

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla ord från ett StopWordDictionary-objekt.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.String> - En iterator som kan användas för att iterera genom samlingen.

