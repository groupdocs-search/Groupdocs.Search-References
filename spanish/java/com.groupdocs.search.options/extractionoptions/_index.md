---
title: "ExtractionOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para extraer datos de documentos."
type: docs
weight: 18
url: /es/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

Proporciona opciones para extraer datos de documentos.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | Inicializa una nueva instancia de la  ExtractionOptions  clase. |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | Inicializa una nueva instancia de la  ExtractionOptions  clase. |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | Inicializa una nueva instancia de la  ExtractionOptions  clase. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Obtiene el extractor de texto personalizado. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Establece o asigna el extractor de texto personalizado. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Obtiene un valor que indica si se debe detectar la codificación automáticamente o no. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Establece un valor que indica si se debe detectar la codificación automáticamente o no. |
|
|  | [getEncoding()](#getEncoding--) | Obtiene la codificación utilizada para extraer texto de documentos de texto. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | Establece la codificación utilizada para extraer texto de documentos de texto. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Obtiene un valor que indica si se usa el modo sin procesar para la extracción de texto cuando sea posible. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Establece un valor que indica si se usa el modo sin procesar para la extracción de texto cuando sea posible. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | Obtiene las opciones para indexar campos de metadatos. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | Obtiene las opciones para el procesamiento OCR y la indexación del texto reconocido. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | Obtiene las opciones de indexación de imágenes para la búsqueda inversa de imágenes. |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


Inicializa una nueva instancia de la  ExtractionOptions  clase.


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


Inicializa una nueva instancia de la  ExtractionOptions  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


Inicializa una nueva instancia de la  ExtractionOptions  clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Las opciones. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor personalizado. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | El conector ocr. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Obtiene el extractor de texto personalizado. El valor predeterminado es  null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Establece o asigna el extractor de texto personalizado. El valor predeterminado es  null .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor de texto personalizado. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


Obtiene un valor que indica si detectar la codificación automáticamente o no. El valor predeterminado es  false .


**Returns:**
boolean - Un valor que indica si detectar la codificación automáticamente o no.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


Establece un valor que indica si detectar la codificación automáticamente o no. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si detectar la codificación automáticamente o no. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


Obtiene la codificación utilizada para extraer texto de documentos de texto. El valor predeterminado es  null , lo que significa que se usa la codificación predeterminada UTF-8. Si AutoDetectEncoding es  true  entonces este valor se usa como la codificación predeterminada.


**Returns:**
java.lang.String - La codificación utilizada para extraer texto de documentos de texto.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


Establece la codificación utilizada para extraer texto de documentos de texto. El valor predeterminado es  null , lo que significa que se usa la codificación predeterminada UTF-8. Si AutoDetectEncoding es  true  entonces este valor se usa como la codificación predeterminada.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | java.lang.String | La codificación utilizada para extraer texto de documentos de texto. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


Obtiene un valor que indica si se utiliza el modo sin procesar para la extracción de texto cuando sea posible. El valor predeterminado es true. El modo sin procesar puede aumentar significativamente la velocidad de indexación, pero el modo normal mejora el formato del texto extraído.


**Returns:**
boolean - Un valor que indica si se utiliza el modo sin procesar para la extracción de texto cuando sea posible.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


Establece un valor que indica si se utiliza el modo sin procesar para la extracción de texto cuando sea posible. El valor predeterminado es true. El modo sin procesar puede aumentar significativamente la velocidad de indexación, pero el modo normal mejora el formato del texto extraído.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se utiliza el modo sin procesar para la extracción de texto cuando sea posible. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


Obtiene las opciones para indexar campos de metadatos.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


Obtiene las opciones para el procesamiento OCR y la indexación del texto reconocido.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


Obtiene las opciones de indexación de imágenes para la búsqueda inversa de imágenes.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
