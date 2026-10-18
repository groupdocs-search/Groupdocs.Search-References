---
title: "SpellingCorrector"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een spellingcorrector voor termen in een query."
type: docs
weight: 21
url: /nl/java/com.groupdocs.search.dictionaries/spellingcorrector/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase)
```
public interface SpellingCorrector extends DictionaryBase
```

Definieert de interface van een spellingcorrector voor termen in een query.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Managing spelling corrector](../https://docs.groupdocs.com/display/searchjava/Spelling+corrector)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal woorden op dat in deze SpellingCorrector zit. |
|
|  | [getWords()](#getWords--) | Haalt de collectie woorden op die momenteel in deze SpellingCorrector zit. |
|
|  | [addRange(Iterable<String> words)](#addRange-java.lang.Iterable-java.lang.String--) | Voegt de opgegeven verzameling woorden toe aan deze instantie van de SpellingCorrector. |
|
|  | [addRange(String[] words)](#addRange-java.lang.String---) | Voegt de opgegeven verzameling woorden toe aan deze instantie van de SpellingCorrector. |
|
|  | [clear()](#clear--) | Verwijdert alle woorden uit een SpellingCorrector-object. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal woorden op dat in deze SpellingCorrector zit.


**Returns:**
int - Het aantal woorden dat in deze SpellingCorrector zit.

### getWords() {#getWords--}
```
public abstract String[] getWords()
```


Haalt de collectie woorden op die momenteel in deze SpellingCorrector zit.


**Returns:**
java.lang.String[] - De verzameling woorden.

### addRange(Iterable<String> words) {#addRange-java.lang.Iterable-java.lang.String--}
```
public abstract void addRange(Iterable<String> words)
```


Voegt de opgegeven verzameling woorden toe aan deze instantie van de SpellingCorrector.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woorden | java.lang.Iterable<java.lang.String> | De verzameling woorden om toe te voegen aan het woordenboek. |
|

### addRange(String[] words) {#addRange-java.lang.String---}
```
public abstract void addRange(String[] words)
```


Voegt de opgegeven verzameling woorden toe aan deze instantie van de SpellingCorrector.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woorden | java.lang.String[] | De verzameling woorden om toe te voegen aan het woordenboek. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle woorden uit een SpellingCorrector-object.


