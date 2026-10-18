---
title: "SynonymDictionary"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Wörterbuchs für Synonyme."
type: docs
weight: 23
url: /de/java/com.groupdocs.search.dictionaries/synonymdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface SynonymDictionary extends DictionaryBase, Iterable<String>
```

Definiert die Schnittstelle eines Wörterbuchs für Synonyme.


**Learn more**

* [Synonym search](../https://docs.groupdocs.com/display/searchjava/Synonym+search)
* [Managing synonym dictionary](../https://docs.groupdocs.com/display/searchjava/Synonym+dictionary)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Ermittelt die Anzahl der Wörter, die in diesem SynonymDictionary enthalten sind. |
|
|  | [addRange(Iterable<String[]> synonyms)](#addRange-java.lang.Iterable-java.lang.String----) | Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des SynonymDictionary hinzu. |
|
|  | [addRange(String[][] synonyms)](#addRange-java.lang.String-----) | Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des SynonymDictionary hinzu. |
|
|  | [clear()](#clear--) | Entfernt alle Wörter aus diesem SynonymDictionary-Objekt. |
|
|  | [getSynonyms(String word)](#getSynonyms-java.lang.String-) | Ermittelt die Synonyme für das angegebene Wort. |
|
|  | [getSynonymGroups(String word)](#getSynonymGroups-java.lang.String-) | Ermittelt alle Synonymgruppen, zu denen das angegebene Wort gehört. |
|
|  | [getAllSynonymGroups()](#getAllSynonymGroups--) | Ermittelt alle in diesem Wörterbuch enthaltenen Synonymgruppen. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Ermittelt die Anzahl der Wörter, die in diesem SynonymDictionary enthalten sind.


**Returns:**
int – Die Anzahl der Wörter, die in diesem SynonymDictionary enthalten sind.

### addRange(Iterable<String[]> synonyms) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> synonyms)
```


Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des SynonymDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Synonyme | java.lang.Iterable<java.lang.String[]> | Die Sammlung von Synonymgruppen, die dem Wörterbuch hinzugefügt werden soll. |
|

### addRange(String[][] synonyms) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] synonyms)
```


Fügt die angegebene Sammlung von Synonymgruppen zu dieser Instanz des SynonymDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Synonyme | java.lang.String[][] | Die Sammlung von Synonymgruppen, die dem Wörterbuch hinzugefügt werden soll. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Wörter aus diesem SynonymDictionary-Objekt.


### getSynonyms(String word) {#getSynonyms-java.lang.String-}
```
public abstract String[] getSynonyms(String word)
```


Ermittelt die Synonyme für das angegebene Wort. Das resultierende Array enthält das Originalwort nicht.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wort | java.lang.String | Das Wort, für das Synonyme vorgeschlagen werden sollen. |
|

**Returns:**
java.lang.String[] – Die Synonyme für das angegebene Wort oder ein leeres Array, wenn das SynonymDictionary-Objekt das angegebene Wort nicht enthält.

### getSynonymGroups(String word) {#getSynonymGroups-java.lang.String-}
```
public abstract String[][] getSynonymGroups(String word)
```


Ermittelt alle Synonymgruppen, zu denen das angegebene Wort gehört.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wort | java.lang.String | Das Wort zum Abrufen von Synonymgruppen. |
|

**Returns:**
java.lang.String[][] - Alle Synonymgruppen, zu denen das angegebene Wort gehört.

### getAllSynonymGroups() {#getAllSynonymGroups--}
```
public abstract String[][] getAllSynonymGroups()
```


Ermittelt alle in diesem Wörterbuch enthaltenen Synonymgruppen.


**Returns:**
java.lang.String[][] - Alle Synonymgruppen.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.String> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

