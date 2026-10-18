---
title: "TextOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para recuperar el texto del documento desde un índice."
type: docs
weight: 41
url: /es/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

Proporciona opciones para recuperar el texto del documento desde un índice.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | Inicializa una nueva instancia de la clase  TextOptions . |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | Inicializa una nueva instancia de la clase  TextOptions . |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | Obtiene el extractor de texto personalizado que se utilizó para indexar. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Establece el extractor de texto personalizado que se utilizó para indexar. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | Obtiene los campos de documento adicionales que se usaron para la indexación. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Establece los campos de documento adicionales que se usaron para la indexación. |
|
|  | [getCancellation()](#getCancellation--) | Obtiene el objeto de cancelación. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Establece el objeto de cancelación. |
|
|  | [getGenerateHead()](#getGenerateHead--) | Obtiene un valor que indica si la etiqueta Head se genera en el HTML de salida. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | Establece un valor que indica si la etiqueta Head se genera en el HTML de salida. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


Inicializa una nueva instancia de la clase  TextOptions .


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


Inicializa una nueva instancia de la clase  TextOptions .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


Obtiene el extractor de texto personalizado que se usó para la indexación. El valor predeterminado es null. Tenga en cuenta que este valor se usa solo si el texto del documento no se guardó en el índice.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


Establece el extractor de texto personalizado que se usó para la indexación. El valor predeterminado es null. Tenga en cuenta que este valor se usa solo si el texto del documento no se guardó en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | El extractor de texto personalizado que se usó para la indexación. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Obtiene los campos de documento adicionales que se usaron para la indexación. El valor predeterminado es null. Tenga en cuenta que este valor se usa solo si el texto del documento no se guardó en el índice.


**Returns:**
com.groupdocs.search.common.DocumentField[] - Los campos de documento adicionales que se usaron para la indexación.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Establece los campos de documento adicionales que se usaron para la indexación. El valor predeterminado es null. Tenga en cuenta que este valor se usa solo si el texto del documento no se guardó en el índice.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | Los campos de documento adicionales que se usaron para la indexación. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Obtiene el objeto de cancelación. El valor predeterminado es null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Establece el objeto de cancelación. El valor predeterminado es null.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | El objeto de cancelación. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


Obtiene un valor que indica si la etiqueta Head se genera en el HTML de salida. El valor predeterminado es true.


**Returns:**
boolean - Un valor que indica si la etiqueta Head se genera en el HTML de salida.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


Establece un valor que indica si la etiqueta Head se genera en el HTML de salida. El valor predeterminado es true.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si la etiqueta Head se genera en el HTML de salida. |
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
