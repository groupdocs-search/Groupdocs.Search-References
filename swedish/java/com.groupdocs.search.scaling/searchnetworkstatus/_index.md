---
title: "SearchNetworkStatus"
second_title: "GroupDocs.Search för Java API-referens"
description: "Anger en söknätverksstatus."
type: docs
weight: 13
url: /sv/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

Anger en söknätverksstatus.

## Fält

| Fält | Beskrivning |
| --- | --- |
|  | [Ready](#Ready) | Söknetverket är fritt och redo för ändringar. |
|
|  | [Configuring](#Configuring) | Söknetverket utför en konfigurationsoperation. |
|
|  | [Indexing](#Indexing) | Söknetverket utför en indexeringsoperation. |
|
|  | [Optimizing](#Optimizing) | Söknetverket utför en optimeringsoperation. |
|
|  | [Deleting](#Deleting) | Söknetverket utför en raderingsoperation. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Söknetverket ändrar attribut. |
|
|  | [Synchronizing](#Synchronizing) | Söknetverket utför en synkroniseringsoperation. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


Söknetverket är fritt och redo för ändringar.


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


Söknetverket utför en konfigurationsoperation.


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


Söknetverket utför en indexeringsoperation.


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


Söknetverket utför en optimeringsoperation.


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


Söknetverket utför en raderingsoperation.


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


Söknetverket ändrar attribut.


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


Söknetverket utför en synkroniseringsoperation.


### values() {#values--}
```
public static SearchNetworkStatus[] values()
```




**Returns:**
com.groupdocs.search.scaling.SearchNetworkStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchNetworkStatus valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
