---
title: "OperationType"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta un tipo di operazione di indicizzazione."
type: docs
weight: 23
url: /it/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Rappresenta un tipo di operazione di indicizzazione.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Indexing](#Indexing) | Aggiunta di documenti a un indice. |
|
|  | [Updating](#Updating) | Aggiornamento di documenti in un indice. |
|
|  | [Merging](#Merging) | Unione di indici. |
|
|  | [Optimizing](#Optimizing) | Ottimizzazione di un indice. |
|
|  | [Deleting](#Deleting) | Eliminazione di percorsi da un indice. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Aggiunta di documenti a un indice.


### Updating {#Updating}
```
public static final OperationType Updating
```


Aggiornamento di documenti in un indice.


### Merging {#Merging}
```
public static final OperationType Merging
```


Unione di indici.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Ottimizzazione di un indice.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Eliminazione di percorsi da un indice.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
