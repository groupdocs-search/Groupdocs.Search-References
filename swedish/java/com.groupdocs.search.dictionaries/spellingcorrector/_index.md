---
title: "SpellingCorrector"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en stavningskorrigerare för termer i en fråga."
type: docs
weight: 21
url: /sv/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Definierar gränssnittet för en stavningskorrigerare för termer i en fråga.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet ord som finns i detta  SpellingCorrector . |
|
|  | [getWords()](#getWords--) | Hämtar samlingen av ord som för närvarande finns i detta  SpellingCorrector . |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Lägger till den angivna samlingen av ord till den här instansen av SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Lägger till den angivna samlingen av ord till den här instansen av SpellingCorrector. |
|
|  | [clear()](#clear--) | Tar bort alla ord från ett SpellingCorrector-objekt. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet ord som finns i detta  SpellingCorrector .


**Returns:**
int - Antalet ord som finns i detta SpellingCorrector.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Hämtar samlingen av ord som för närvarande finns i detta  SpellingCorrector .


**Returns:**
java.lang.String[] - Samlingen av ord.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Lägger till den angivna samlingen av ord till den här instansen av SpellingCorrector.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.Iterable<java.lang.String> | Samlingen av ord att lägga till i ordboken. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Lägger till den angivna samlingen av ord till den här instansen av SpellingCorrector.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String[] | Samlingen av ord att lägga till i ordboken. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla ord från ett SpellingCorrector-objekt.


