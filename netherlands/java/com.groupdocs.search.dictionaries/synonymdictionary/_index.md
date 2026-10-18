---
title: "SynonymDictionary"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een woordenboek van synoniemen."
type: docs
weight: 23
url: /nl/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Definieert de interface van een woordenboek van synoniemen.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal woorden op dat in deze  SynonymDictionary  zit. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Voegt de opgegeven collectie van synoniemgroepen toe aan deze instantie van de  SynonymDictionary . |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Voegt de opgegeven collectie van synoniemgroepen toe aan deze instantie van de  SynonymDictionary . |
|
|  | [clear()](#clear--) | Verwijdert alle woorden uit dit  SynonymDictionary  object. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Haalt de synoniemen op voor het opgegeven woord. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Haalt alle groepen synoniemen op waartoe het opgegeven woord behoort. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Haalt alle groepen synoniemen op die in dit woordenboek staan. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal woorden op dat in deze  SynonymDictionary  zit.


**Returns:**
int - Het aantal woorden dat in deze  SynonymDictionary  zit.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Voegt de opgegeven collectie van synoniemgroepen toe aan deze instantie van de  SynonymDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | synoniemen | java.lang.Iterable<java.lang.String[]> | De collectie van synoniemgroepen om toe te voegen aan het woordenboek. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Voegt de opgegeven collectie van synoniemgroepen toe aan deze instantie van de  SynonymDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | synoniemen | java.lang.String[][] | De collectie van synoniemgroepen om toe te voegen aan het woordenboek. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle woorden uit dit  SynonymDictionary  object.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Haalt de synoniemen op voor het opgegeven woord. De resulterende array bevat het oorspronkelijke woord niet.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woord | java.lang.String | Het woord om de synoniemen voor te stellen. |
|

**Returns:**
java.lang.String[] - De synoniemen voor het opgegeven woord of een lege array als het  SynonymDictionary  object het opgegeven woord niet bevat.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Haalt alle groepen synoniemen op waartoe het opgegeven woord behoort.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woord | java.lang.String | Het woord voor het verkrijgen van groepen synoniemen. |
|

**Returns:**
java.lang.String[][] - Alle groepen synoniemen waartoe het opgegeven woord behoort.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Haalt alle groepen synoniemen op die in dit woordenboek staan.


**Returns:**
java.lang.String[][] - Alle groepen synoniemen.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.String> - Een iterator die kan worden gebruikt om door de collectie te itereren.

