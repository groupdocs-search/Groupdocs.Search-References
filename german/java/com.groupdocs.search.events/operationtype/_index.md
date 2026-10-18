---
title: "OperationType"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt einen Indexoperationstyp dar."
type: docs
weight: 23
url: /de/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Stellt einen Indexoperationstyp dar.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Indexing](#Indexing) | Hinzufügen von Dokumenten zu einem Index. |
|
|  | [Updating](#Updating) | Aktualisieren von Dokumenten in einem Index. |
|
|  | [Merging](#Merging) | Zusammenführen von Indizes. |
|
|  | [Optimizing](#Optimizing) | Optimieren eines Index. |
|
|  | [Deleting](#Deleting) | Löschen von Pfaden aus einem Index. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Hinzufügen von Dokumenten zu einem Index.


### Updating {#Updating}
```
public static final OperationType Updating
```


Aktualisieren von Dokumenten in einem Index.


### Merging {#Merging}
```
public static final OperationType Merging
```


Zusammenführen von Indizes.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Optimieren eines Index.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Löschen von Pfaden aus einem Index.


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
