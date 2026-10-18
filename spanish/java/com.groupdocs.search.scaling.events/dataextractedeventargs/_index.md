---
title: "DataExtractedEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de finalización de la extracción de datos de un documento."
type: docs
weight: 10
url: /es/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

Representa los argumentos del evento de finalización de la extracción de datos de un documento.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | Obtiene el índice del extractor. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Obtiene la clave del documento. |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


Obtiene el índice del extractor.


**Returns:**
int - El índice del extractor.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtiene la clave del documento.


**Returns:**
java.lang.String - La clave del documento.

