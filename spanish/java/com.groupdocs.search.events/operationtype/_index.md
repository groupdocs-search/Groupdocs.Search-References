---
title: "OperationType"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa un tipo de operación de índice."
type: docs
weight: 23
url: /es/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Representa un tipo de operación de índice.

## Campos

| Campo | Descripción |
| --- | --- |
|  | [Indexing](#Indexing) | Añadiendo documentos a un índice. |
|
|  | [Updating](#Updating) | Actualizando documentos en un índice. |
|
|  | [Merging](#Merging) | Fusionando índices. |
|
|  | [Optimizing](#Optimizing) | Optimizando un índice. |
|
|  | [Deleting](#Deleting) | Eliminando rutas de un índice. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Añadiendo documentos a un índice.


### Updating {#Updating}
```
public static final OperationType Updating
```


Actualizando documentos en un índice.


### Merging {#Merging}
```
public static final OperationType Merging
```


Fusionando índices.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Optimizando un índice.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Eliminando rutas de un índice.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
