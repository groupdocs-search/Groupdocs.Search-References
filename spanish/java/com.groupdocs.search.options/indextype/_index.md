---
title: "IndexType"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Especifica un tipo de índice."
type: docs
weight: 49
url: /es/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

Especifica un tipo de índice.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## Campos

| Campo | Descripción |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | Índice normal con metadatos de documentos y contenido de documentos que admite todas las funciones de búsqueda. |
|
|  | [MetadataIndex](#MetadataIndex) | Índice que contiene solo los metadatos de los documentos, sin contenido. |
|
|  | [CompactIndex](#CompactIndex) | Tipo de índice que ocupa mucho menos espacio en disco pero no admite la búsqueda de frases ni las funciones de búsqueda por rango de fechas. |
|
## Métodos

| Método | Descripción |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


Índice normal con metadatos de documentos y contenido de documentos que admite todas las funciones de búsqueda.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


Índice que contiene solo los metadatos de los documentos, sin contenido.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


Tipo de índice que ocupa mucho menos espacio en disco pero no admite la búsqueda de frases ni las funciones de búsqueda por rango de fechas.


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
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
