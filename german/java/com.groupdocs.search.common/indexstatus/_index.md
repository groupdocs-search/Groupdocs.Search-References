---
title: "IndexStatus"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Gibt einen Indexstatus an."
type: docs
weight: 41
url: /de/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Gibt einen Indexstatus an.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Ready](#Ready) | Index ist frei und bereit zur Änderung. |
|
|  | [Failed](#Failed) | Index muss aufgrund eines Fehlers neu geladen werden. |
|
|  | [Indexing](#Indexing) | Index führt einen Indexierungsvorgang aus. |
|
|  | [Updating](#Updating) | Index führt einen Aktualisierungsvorgang aus. |
|
|  | [Merging](#Merging) | Index führt einen Zusammenführungsvorgang aus. |
|
|  | [Optimizing](#Optimizing) | Index führt einen Optimierungsvorgang aus. |
|
|  | [Deleting](#Deleting) | Der Index führt eine Löschoperation aus. |
|
|  | [Renaming](#Renaming) | Der Index führt eine Umbenennungsoperation aus. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Der Index ändert Attribute. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Index ist frei und bereit zur Änderung.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Index muss aufgrund eines Fehlers neu geladen werden.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Index führt einen Indexierungsvorgang aus.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Index führt einen Aktualisierungsvorgang aus.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Index führt einen Zusammenführungsvorgang aus.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Index führt einen Optimierungsvorgang aus.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Der Index führt eine Löschoperation aus.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Der Index führt eine Umbenennungsoperation aus.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Der Index ändert Attribute.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
