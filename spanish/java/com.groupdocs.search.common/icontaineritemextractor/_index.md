---
title: "IContainerItemExtractor"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona métodos para extraer elementos de documentos contenedores."
type: docs
weight: 35
url: /es/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Proporciona métodos para extraer elementos de documentos contenedores.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | Obtiene la familia de formatos del documento. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Extrae elementos del documento contenedor. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Extrae elementos del documento contenedor. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Obtiene la familia de formatos del documento.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Extrae elementos del documento contenedor.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | filePath | java.lang.String | La ruta del archivo. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Una matriz de elementos extraídos.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Extrae elementos del documento contenedor.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | stream | java.io.InputStream | El flujo del documento. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - Una matriz de elementos extraídos.

