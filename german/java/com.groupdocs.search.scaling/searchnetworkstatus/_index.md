---
title: "SearchNetworkStatus"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Gibt einen Suchnetzwerk-Status an."
type: docs
weight: 13
url: /de/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

Gibt einen Suchnetzwerk-Status an.

## Felder

| Feld | Beschreibung |
| --- | --- |
|  | [Ready](#Ready) | Das Suchnetzwerk ist frei und bereit für Änderungen. |
|
|  | [Configuring](#Configuring) | Das Suchnetzwerk führt eine Konfigurationsoperation aus. |
|
|  | [Indexing](#Indexing) | Das Suchnetzwerk führt eine Indexierungsoperation aus. |
|
|  | [Optimizing](#Optimizing) | Das Suchnetzwerk führt eine Optimierungsoperation aus. |
|
|  | [Deleting](#Deleting) | Das Suchnetzwerk führt eine Löschoperation aus. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Das Suchnetzwerk ändert Attribute. |
|
|  | [Synchronizing](#Synchronizing) | Das Suchnetzwerk führt eine Synchronisationsoperation aus. |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


Das Suchnetzwerk ist frei und bereit für Änderungen.


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


Das Suchnetzwerk führt eine Konfigurationsoperation aus.


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


Das Suchnetzwerk führt eine Indexierungsoperation aus.


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


Das Suchnetzwerk führt eine Optimierungsoperation aus.


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


Das Suchnetzwerk führt eine Löschoperation aus.


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


Das Suchnetzwerk ändert Attribute.


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


Das Suchnetzwerk führt eine Synchronisationsoperation aus.


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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
