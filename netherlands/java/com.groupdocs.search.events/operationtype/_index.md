---
title: "OperationType"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt een type indexeringsbewerking voor."
type: docs
weight: 23
url: /nl/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Stelt een type indexeringsbewerking voor.

## Velden

| Veld | Beschrijving |
| --- | --- |
|  | [Indexing](#Indexing) | Documenten toevoegen aan een index. |
|
|  | [Updating](#Updating) | Documenten bijwerken in een index. |
|
|  | [Merging](#Merging) | Indexes samenvoegen. |
|
|  | [Optimizing](#Optimizing) | Een index optimaliseren. |
|
|  | [Deleting](#Deleting) | Paden verwijderen uit een index. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Documenten toevoegen aan een index.


### Updating {#Updating}
```
public static final OperationType Updating
```


Documenten bijwerken in een index.


### Merging {#Merging}
```
public static final OperationType Merging
```


Indexes samenvoegen.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Een index optimaliseren.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Paden verwijderen uit een index.


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
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
