---
title: "SearchNetworkStatus"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Especifica un estado de la red de búsqueda."
type: docs
weight: 13
url: /es/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

Especifica un estado de la red de búsqueda.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Ready](#Ready) | La red de búsqueda está libre y lista para cambios. |
|
|  | [Configuring](#Configuring) | La red de búsqueda realiza una operación de configuración. |
|
|  | [Indexing](#Indexing) | La red de búsqueda realiza una operación de indexación. |
|
|  | [Optimizing](#Optimizing) | La red de búsqueda realiza una operación de optimización. |
|
|  | [Deleting](#Deleting) | La red de búsqueda realiza una operación de eliminación. |
|
|  | [ChangingAttributes](#ChangingAttributes) | La red de búsqueda cambia atributos. |
|
|  | [Synchronizing](#Synchronizing) | La red de búsqueda realiza una operación de sincronización. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


La red de búsqueda está libre y lista para cambios.


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


La red de búsqueda realiza una operación de configuración.


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


La red de búsqueda realiza una operación de indexación.


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


La red de búsqueda realiza una operación de optimización.


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


La red de búsqueda realiza una operación de eliminación.


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


La red de búsqueda cambia atributos.


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


La red de búsqueda realiza una operación de sincronización.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
