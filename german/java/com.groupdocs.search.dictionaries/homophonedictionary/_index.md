---
title: "HomophoneDictionary"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Wörterbuchs für heterographische Homophone."
type: docs
weight: 18
url: /de/java/com.groupdocs.search.dictionaries/homophonedictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface HomophoneDictionary extends DictionaryBase, Iterable<String>
```

Definiert die Schnittstelle eines Wörterbuchs für heterographische Homophone.


**Learn more**

* [Homophone search](../https://docs.groupdocs.com/display/searchjava/Homophone+search)
* [Managing homophone dictionary](../https://docs.groupdocs.com/display/searchjava/Homophone+dictionary)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Gibt die Anzahl der Wörter zurück, die in diesem  HomophoneDictionary  enthalten sind. |
|
|  | [addRange(Iterable<String[]> homophones)](#addRange-java.lang.Iterable-java.lang.String----) | Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des  HomophoneDictionary  hinzu. |
|
|  | [addRange(String[][] homophones)](#addRange-java.lang.String-----) | Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des  HomophoneDictionary  hinzu. |
|
|  | [clear()](#clear--) | Entfernt alle Wörter aus einem  HomophoneDictionary  Objekt. |
|
|  | [getHomophones(String word)](#getHomophones-java.lang.String-) | Gibt die Homophone für das angegebene Wort zurück. |
|
|  | [getHomophoneGroups(String word)](#getHomophoneGroups-java.lang.String-) | Gibt alle Homophon‑Gruppen zurück, zu denen das angegebene Wort gehört. |
|
|  | [getAllHomophoneGroups()](#getAllHomophoneGroups--) | Gibt alle in diesem Wörterbuch enthaltenen Homophon‑Gruppen zurück. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Gibt die Anzahl der Wörter zurück, die in diesem  HomophoneDictionary  enthalten sind.


**Returns:**
int - Die Anzahl der Wörter.

### addRange(Iterable<String[]> homophones) {#addRange-java.lang.Iterable-java.lang.String----}
```
public abstract void addRange(Iterable<String[]> homophones)
```


Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des  HomophoneDictionary  hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | homophones | java.lang.Iterable<java.lang.String[]> | Die Sammlung von Homophon‑Gruppen, die dem Wörterbuch hinzugefügt werden soll. |
|

### addRange(String[][] homophones) {#addRange-java.lang.String-----}
```
public abstract void addRange(String[][] homophones)
```


Fügt die angegebene Sammlung von Homophon‑Gruppen zu dieser Instanz des  HomophoneDictionary  hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | homophones | java.lang.String[][] | Die Sammlung von Homophon‑Gruppen, die dem Wörterbuch hinzugefügt werden soll. |
|

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Wörter aus einem  HomophoneDictionary  Objekt.


### getHomophones(String word) {#getHomophones-java.lang.String-}
```
public abstract String[] getHomophones(String word)
```


Gibt die Homophone für das angegebene Wort zurück. Das resultierende Array enthält das ursprüngliche Wort nicht.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wort | java.lang.String | Das Wort, um die Homophone vorzuschlagen. |
|

**Returns:**
java.lang.String[] - Die Homophone für das angegebene Wort oder ein leeres Array, wenn das  HomophoneDictionary  Objekt das angegebene Wort nicht enthält.

### getHomophoneGroups(String word) {#getHomophoneGroups-java.lang.String-}
```
public abstract String[][] getHomophoneGroups(String word)
```


Gibt alle Homophon‑Gruppen zurück, zu denen das angegebene Wort gehört.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Wort | java.lang.String | Das Wort, um Gruppen von Homophonen zu erhalten. |
|

**Returns:**
java.lang.String[][] - Alle Gruppen von Homophonen, zu denen das angegebene Wort gehört.

### getAllHomophoneGroups() {#getAllHomophoneGroups--}
```
public abstract String[][] getAllHomophoneGroups()
```


Gibt alle in diesem Wörterbuch enthaltenen Homophon‑Gruppen zurück.


**Returns:**
java.lang.String[][] - Alle Gruppen von Homophonen.

### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.String> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

