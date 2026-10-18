---
title: "OperationType"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar en typ av indexeringsoperation."
type: docs
weight: 23
url: /sv/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Representerar en typ av indexeringsoperation.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Indexing](#Indexing) | Lägger till dokument i ett index. |
|
|  | [Updating](#Updating) | Uppdaterar dokument i ett index. |
|
|  | [Merging](#Merging) | Slår samman index. |
|
|  | [Optimizing](#Optimizing) | Optimerar ett index. |
|
|  | [Deleting](#Deleting) | Tar bort sökvägar från ett index. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Lägger till dokument i ett index.


### Updating {#Updating}
```
public static final OperationType Updating
```


Uppdaterar dokument i ett index.


### Merging {#Merging}
```
public static final OperationType Merging
```


Slår samman index.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Optimerar ett index.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Tar bort sökvägar från ett index.


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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
