---
title: "AliasDictionary"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Definiert die Schnittstelle eines Aliaswörterbuchs."
type: docs
weight: 14
url: /de/java/com.groupdocs.search.dictionaries/aliasdictionary/
---
**All Implemented Interfaces:**
[com.groupdocs.search.dictionaries.DictionaryBase](../../com.groupdocs.search.dictionaries/dictionarybase), java.lang.Iterable
```
public interface AliasDictionary extends DictionaryBase, Iterable<String>
```

Definiert die Schnittstelle eines Aliaswörterbuchs.


**Learn more**

* [Using aliases](../https://docs.groupdocs.com/display/searchjava/Using+aliases)
* [Managing alias dictionary](../https://docs.groupdocs.com/display/searchjava/Alias+dictionary)

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getCount()](#getCount--) | Liefert die Anzahl der Aliasse, die im AliasDictionary enthalten sind. |
|
|  | [addRange(Iterable<AliasReplacementPair> pairs)](#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--) | Fügt die angegebene Sammlung von Alias/Ersatz-Paaren zu dieser Instanz des AliasDictionary hinzu. |
|
|  | [addRange(AliasReplacementPair[] pairs)](#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---) | Fügt die angegebene Sammlung von Alias/Ersatz-Paaren zu dieser Instanz des AliasDictionary hinzu. |
|
|  | [add(String alias, String text)](#add-java.lang.String-java.lang.String-) | Fügt das angegebene Paar aus Alias und zugehörigem Text zu dieser Instanz des AliasDictionary hinzu. |
|
|  | [remove(String alias)](#remove-java.lang.String-) | Entfernt den angegebenen Alias aus einem AliasDictionary-Objekt. |
|
|  | [contains(String alias)](#contains-java.lang.String-) | Bestimmt, ob ein AliasDictionary-Objekt den angegebenen Alias enthält. |
|
|  | [getText(String alias)](#getText-java.lang.String-) | Liefert einen Text, der dem angegebenen Alias zugeordnet ist. |
|
|  | [clear()](#clear--) | Entfernt alle Aliasse aus einem AliasDictionary-Objekt. |
|
|  | [iterator()](#iterator--) | Gibt einen Iterator zurück, der durch die Sammlung iteriert. |
|
### getCount() {#getCount--}
```
public abstract int getCount()
```


Liefert die Anzahl der Aliasse, die im AliasDictionary enthalten sind.


**Returns:**
int - Die Anzahl der Aliasse, die im AliasDictionary enthalten sind.

### addRange(Iterable<AliasReplacementPair> pairs) {#addRange-java.lang.Iterable-com.groupdocs.search.dictionaries.AliasReplacementPair--}
```
public abstract void addRange(Iterable<AliasReplacementPair> pairs)
```


Fügt die angegebene Sammlung von Alias/Ersatz-Paaren zu dieser Instanz des AliasDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Paare | java.lang.Iterable<com.groupdocs.search.dictionaries.AliasReplacementPair> | Die Sammlung von Alias/Ersatz-Paaren, die dem Wörterbuch hinzugefügt werden sollen. |
|

### addRange(AliasReplacementPair[] pairs) {#addRange-com.groupdocs.search.dictionaries.AliasReplacementPair---}
```
public abstract void addRange(AliasReplacementPair[] pairs)
```


Fügt die angegebene Sammlung von Alias/Ersatz-Paaren zu dieser Instanz des AliasDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pairs | [AliasReplacementPair\[\]](../../com.groupdocs.search.dictionaries/aliasreplacementpair) | Die Sammlung von Alias/Ersatz-Paaren, die dem Wörterbuch hinzugefügt werden sollen. |
|

### add(String alias, String text) {#add-java.lang.String-java.lang.String-}
```
public abstract void add(String alias, String text)
```


Fügt das angegebene Paar aus Alias und zugehörigem Text zu dieser Instanz des AliasDictionary hinzu.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Alias | java.lang.String | Der Alias, der dem Wörterbuch hinzugefügt werden soll. |
|
|  | Text | java.lang.String | Der Text, der dem Alias zugeordnet werden soll. |
|

### remove(String alias) {#remove-java.lang.String-}
```
public abstract boolean remove(String alias)
```


Entfernt den angegebenen Alias aus einem AliasDictionary-Objekt.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Alias | java.lang.String | Der zu entfernende Alias. |
|

**Returns:**
boolean - Diese Methode gibt  true  zurück, wenn das Alias erfolgreich gefunden und entfernt wurde. Diese Methode gibt  false  zurück, wenn das Alias im  AliasDictionary  Objekt nicht gefunden wird.

### contains(String alias) {#contains-java.lang.String-}
```
public abstract boolean contains(String alias)
```


Bestimmt, ob ein AliasDictionary-Objekt den angegebenen Alias enthält.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Alias | java.lang.String | Das Alias, das im  AliasDictionary  Objekt zu finden ist. |
|

**Returns:**
boolean -  true  wenn das  AliasDictionary  Objekt das angegebene Alias enthält; andernfalls  false .

### getText(String alias) {#getText-java.lang.String-}
```
public abstract String getText(String alias)
```


Liefert einen Text, der dem angegebenen Alias zugeordnet ist.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Alias | java.lang.String | Das Alias, das im  AliasDictionary  Objekt zu finden ist. |
|

**Returns:**
java.lang.String - Ein Text, der dem angegebenen Alias zugeordnet ist, oder  null .

### clear() {#clear--}
```
public abstract void clear()
```


Entfernt alle Aliasse aus einem AliasDictionary-Objekt.


### iterator() {#iterator--}
```
public abstract Iterator<String> iterator()
```


Gibt einen Iterator zurück, der durch die Sammlung iteriert.


**Returns:**
java.util.Iterator<java.lang.String> - Ein Iterator, der verwendet werden kann, um durch die Sammlung zu iterieren.

