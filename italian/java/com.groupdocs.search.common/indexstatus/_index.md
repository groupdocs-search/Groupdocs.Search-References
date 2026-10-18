---
title: "IndexStatus"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Specifica lo stato di un indice."
type: docs
weight: 41
url: /it/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Specifica lo stato di un indice.

## Fields

| Field | Descrizione |
| --- | --- |
|  | [Ready](#Ready) | L'indice è libero e pronto per le modifiche. |
|
|  | [Failed](#Failed) | L'indice deve essere ricaricato a causa di un errore. |
|
|  | [Indexing](#Indexing) | L'indice esegue un'operazione di indicizzazione. |
|
|  | [Updating](#Updating) | L'indice esegue un'operazione di aggiornamento. |
|
|  | [Merging](#Merging) | L'indice esegue un'operazione di fusione. |
|
|  | [Optimizing](#Optimizing) | L'indice esegue un'operazione di ottimizzazione. |
|
|  | [Deleting](#Deleting) | L'indice esegue un'operazione di eliminazione. |
|
|  | [Renaming](#Renaming) | L'indice esegue un'operazione di rinomina. |
|
|  | [ChangingAttributes](#ChangingAttributes) | L'indice modifica gli attributi. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


L'indice è libero e pronto per le modifiche.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


L'indice deve essere ricaricato a causa di un errore.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


L'indice esegue un'operazione di indicizzazione.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


L'indice esegue un'operazione di aggiornamento.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


L'indice esegue un'operazione di fusione.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


L'indice esegue un'operazione di ottimizzazione.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


L'indice esegue un'operazione di eliminazione.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


L'indice esegue un'operazione di rinomina.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


L'indice modifica gli attributi.


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
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
