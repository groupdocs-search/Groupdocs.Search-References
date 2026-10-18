---
title: "IndexStatus"
second_title: "GroupDocs.Search för Java API-referens"
description: "Specificerar ett indexstatus."
type: docs
weight: 41
url: /sv/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Specificerar ett indexstatus.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Ready](#Ready) | Indexet är fritt och redo att ändras. |
|
|  | [Failed](#Failed) | Indexet måste laddas om på grund av ett fel. |
|
|  | [Indexing](#Indexing) | Indexet utför en indexeringsoperation. |
|
|  | [Updating](#Updating) | Indexet utför en uppdateringsoperation. |
|
|  | [Merging](#Merging) | Indexet utför en sammanslagningsoperation. |
|
|  | [Optimizing](#Optimizing) | Indexet utför en optimeringsoperation. |
|
|  | [Deleting](#Deleting) | Index utför en raderingsoperation. |
|
|  | [Renaming](#Renaming) | Index utför en namnbytesoperation. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Index ändrar attribut. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Indexet är fritt och redo att ändras.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Indexet måste laddas om på grund av ett fel.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Indexet utför en indexeringsoperation.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Indexet utför en uppdateringsoperation.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Indexet utför en sammanslagningsoperation.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Indexet utför en optimeringsoperation.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Index utför en raderingsoperation.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Index utför en namnbytesoperation.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Index ändrar attribut.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
