---
title: "IndexStatus"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Especifica el estado de un índice."
type: docs
weight: 41
url: /es/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Especifica el estado de un índice.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Ready](#Ready) | El índice está libre y listo para cambiar. |
|
|  | [Failed](#Failed) | El índice necesita recargarse debido a un error. |
|
|  | [Indexing](#Indexing) | El índice realiza una operación de indexación. |
|
|  | [Updating](#Updating) | El índice realiza una operación de actualización. |
|
|  | [Merging](#Merging) | El índice realiza una operación de fusión. |
|
|  | [Optimizing](#Optimizing) | El índice realiza una operación de optimización. |
|
|  | [Deleting](#Deleting) | Index realiza una operación de eliminación. |
|
|  | [Renaming](#Renaming) | Index realiza una operación de renombrado. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Index cambia atributos. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


El índice está libre y listo para cambiar.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


El índice necesita recargarse debido a un error.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


El índice realiza una operación de indexación.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


El índice realiza una operación de actualización.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


El índice realiza una operación de fusión.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


El índice realiza una operación de optimización.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Index realiza una operación de eliminación.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Index realiza una operación de renombrado.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Index cambia atributos.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
