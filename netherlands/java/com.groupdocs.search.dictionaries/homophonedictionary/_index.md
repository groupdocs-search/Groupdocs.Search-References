---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Definieert de interface van een woordenboek van heterografische homofonen."
type: docs
weight: 18
url: /nl/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Definieert de interface van een woordenboek van heterografische homofonen.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getCount()](#getCount--) | Haalt het aantal woorden op dat in deze  HomophoneDictionary  zit. |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Voegt de opgegeven collectie van homofone groepen toe aan deze instantie van de  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Voegt de opgegeven collectie van homofone groepen toe aan deze instantie van de  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Verwijdert alle woorden uit een  HomophoneDictionary  object. |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Haalt de homofonen op voor het opgegeven woord. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Haalt alle groepen homofonen op waartoe het opgegeven woord behoort. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Haalt alle groepen homofonen op die in dit woordenboek zijn opgenomen. |
|
|  | [iterator()](#iterator--) | Retourneert een iterator die door de collectie iterereert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Haalt het aantal woorden op dat in deze  HomophoneDictionary  zit.


**Returns:**
int - Het aantal woorden.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Voegt de opgegeven collectie van homofone groepen toe aan deze instantie van de  HomophoneDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | De collectie van homofone groepen die aan het woordenboek moet worden toegevoegd. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Voegt de opgegeven collectie van homofone groepen toe aan deze instantie van de  HomophoneDictionary .


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | De collectie van homofone groepen die aan het woordenboek moet worden toegevoegd. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Verwijdert alle woorden uit een  HomophoneDictionary  object.


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Haalt de homofonen op voor het opgegeven woord. De resulterende array bevat het oorspronkelijke woord niet.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woord | java.lang.String | Het woord om de homofonen voor te stellen. |
|

**Returns:**
java.lang.String[] - De homofonen voor het opgegeven woord of een lege array als het HomophoneDictionary object het opgegeven woord niet bevat.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Haalt alle groepen homofonen op waartoe het opgegeven woord behoort.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | woord | java.lang.String | Het woord om groepen homofonen te verkrijgen. |
|

**Returns:**
java.lang.String[][] - Alle groepen homofonen waartoe het opgegeven woord behoort.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Haalt alle groepen homofonen op die in dit woordenboek zijn opgenomen.


**Returns:**
java.lang.String[][] - Alle groepen homofonen.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Retourneert een iterator die door de collectie iterereert.


**Returns:**
java.util.Iterator<java.lang.String> - Een iterator die kan worden gebruikt om door de collectie te itereren.

