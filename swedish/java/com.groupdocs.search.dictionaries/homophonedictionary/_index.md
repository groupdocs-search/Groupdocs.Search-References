---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en ordbok med heterografiska homofoner."
type: docs
weight: 18
url: /sv/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Definierar gränssnittet för en ordbok med heterografiska homofoner.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet ord som finns i denna  HomophoneDictionary . |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Lägger till den angivna samlingen av homofongrupp till denna instans av  HomophoneDictionary . |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Lägger till den angivna samlingen av homofongrupp till denna instans av  HomophoneDictionary . |
|
|  | [clear()](#clear--) | Tar bort alla ord från ett  HomophoneDictionary  -objekt. |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Hämtar homofonerna för det angivna ordet. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Hämtar alla grupper av homofoner som det angivna ordet tillhör. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Hämtar alla grupper av homofoner som finns i denna ordbok. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet ord som finns i denna  HomophoneDictionary .


**Returns:**
int - Antalet ord.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Lägger till den angivna samlingen av homofongrupp till denna instans av  HomophoneDictionary .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | Samlingen av homofongrupper att lägga till i ordboken. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Lägger till den angivna samlingen av homofongrupp till denna instans av  HomophoneDictionary .


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | Samlingen av homofongrupper att lägga till i ordboken. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla ord från ett  HomophoneDictionary  -objekt.


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Hämtar homofonerna för det angivna ordet. Den resulterande arrayen innehåller inte det ursprungliga ordet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String | Ordet för att föreslå homofonerna. |
|

**Returns:**
java.lang.String[] - Homofonerna för det angivna ordet eller tom array om  HomophoneDictionary  objektet inte innehåller det angivna ordet.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Hämtar alla grupper av homofoner som det angivna ordet tillhör.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String | Ordet för att hämta grupper av homofoner. |
|

**Returns:**
java.lang.String[][] - Alla grupper av homofoner som det angivna ordet tillhör.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Hämtar alla grupper av homofoner som finns i denna ordbok.


**Returns:**
java.lang.String[][] - Alla grupper av homofoner.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.String> - En iterator som kan användas för att iterera genom samlingen.

