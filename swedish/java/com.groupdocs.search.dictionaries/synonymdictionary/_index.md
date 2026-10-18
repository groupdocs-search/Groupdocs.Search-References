---
title: "SynonymDictionary"
second_title: "GroupDocs.Search för Java API-referens"
description: "Definierar gränssnittet för en ordbok med synonymer."
type: docs
weight: 23
url: /sv/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Definierar gränssnittet för en ordbok med synonymer.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getCount()](#getCount--) | Hämtar antalet ord som finns i detta SynonymDictionary. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Lägger till den angivna samlingen av synonymgrupper till denna instans av SynonymDictionary. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Lägger till den angivna samlingen av synonymgrupper till denna instans av SynonymDictionary. |
|
|  | [clear()](#clear--) | Tar bort alla ord från detta SynonymDictionary-objekt. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Hämtar synonymerna för det angivna ordet. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Hämtar alla synonymgrupper som det angivna ordet tillhör. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Hämtar alla synonymgrupper som finns i detta dictionary. |
|
|  | [iterator()](#iterator--) | Returnerar en iterator som itererar genom samlingen. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Hämtar antalet ord som finns i detta SynonymDictionary.


**Returns:**
int - Antalet ord som finns i detta SynonymDictionary.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Lägger till den angivna samlingen av synonymgrupper till denna instans av SynonymDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | synonymer | java.lang.Iterable<java.lang.String[]> | Samlingen av synonymgrupper att lägga till i dictionaryn. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Lägger till den angivna samlingen av synonymgrupper till denna instans av SynonymDictionary.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | synonymer | java.lang.String[][] | Samlingen av synonymgrupper att lägga till i dictionaryn. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Tar bort alla ord från detta SynonymDictionary-objekt.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Hämtar synonymerna för det angivna ordet. Den resulterande arrayen innehåller inte det ursprungliga ordet.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String | Ordet för att föreslå synonymerna. |
|

**Returns:**
java.lang.String[] - Synonymerna för det angivna ordet eller tom array om SynonymDictionary-objektet inte innehåller det angivna ordet.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Hämtar alla synonymgrupper som det angivna ordet tillhör.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | ord | java.lang.String | Ordet för att hämta grupper av synonymer. |
|

**Returns:**
java.lang.String[][] - Alla grupper av synonymer som det angivna ordet tillhör.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Hämtar alla synonymgrupper som finns i detta dictionary.


**Returns:**
java.lang.String[][] - Alla grupper av synonymer.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Returnerar en iterator som itererar genom samlingen.


**Returns:**
java.util.Iterator<java.lang.String> - En iterator som kan användas för att iterera genom samlingen.

