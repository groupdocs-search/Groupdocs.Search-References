---
title: "IndexType"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Specifica un tipo di indice."
type: docs
weight: 49
url: /it/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Specifica un tipo di indice.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Fields

| Field | Descrizione |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Indice normale con i metadati dei documenti e il contenuto dei documenti che supporta tutte le funzionalità di ricerca. |
|
|  | [MetadataIndex](#MetadataIndex) | Indice che contiene solo i metadati dei documenti, senza contenuto. |
|
|  | [CompactIndex](#CompactIndex) | Tipo di indice che occupa molto meno spazio su disco ma non supporta la ricerca di frasi e le funzionalità di ricerca per intervallo di date. |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Indice normale con i metadati dei documenti e il contenuto dei documenti che supporta tutte le funzionalità di ricerca.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Indice che contiene solo i metadati dei documenti, senza contenuto.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Tipo di indice che occupa molto meno spazio su disco ma non supporta la ricerca di frasi e le funzionalità di ricerca per intervallo di date.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| nome | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
