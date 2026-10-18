---
title: "ExtractedItemInfo"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa información de un elemento de contenedor."
type: docs
weight: 18
url: /es/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Representa información de un elemento de contenedor.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Inicializa una nueva instancia de la  ExtractedItemInfo  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Obtiene un tipo de documento. |
|
|  | [getFields()](#getFields--) | Obtiene campos extraídos. |
|
|  | [getItemInfo()](#getItemInfo--) | Obtiene la información del elemento. |
|
|  | [getInnerPath()](#getInnerPath--) | Obtiene una ruta interna. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Inicializa una nueva instancia de la  ExtractedItemInfo  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | La familia de formatos de documento. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Los campos extraídos. |
|
|  | itemInfo | java.lang.String | La información del elemento. |
|
|  | innerPath | java.lang.String | La ruta al elemento en el contenedor. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Obtiene un tipo de documento.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Obtiene campos extraídos.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Los campos extraídos.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Obtiene la información del elemento.


**Returns:**
java.lang.String - La información del elemento.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Obtiene una ruta interna.


**Returns:**
java.lang.String - La ruta interna.

