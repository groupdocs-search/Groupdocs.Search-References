---
title: "UpdateOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para la operación de actualización."
type: docs
weight: 43
url: /es/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

Proporciona opciones para la operación de actualización.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | Inicializa una nueva instancia de la clase UpdateOptions. |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | Inicializa una nueva instancia de la clase UpdateOptions. |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getThreads()](#getThreads--) | Obtiene el número de hilos utilizados para la indexación. |
|
|  | [setThreads(int value)](#setThreads-int-) | Establece el número de hilos utilizados para la indexación. |
|
|  | [isAsync()](#isAsync--) | Obtiene la bandera de ejecución asíncrona de la operación. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Establece la bandera de ejecución asíncrona de la operación. |
|
|  | [getCancellation()](#getCancellation--) | Obtiene el objeto de cancelación de la operación. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Establece el objeto de cancelación de la operación. |
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
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


Inicializa una nueva instancia de la clase UpdateOptions.


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


Inicializa una nueva instancia de la clase UpdateOptions.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | datos | java.lang.Object | Los datos serializados. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


Obtiene el número de hilos usados para la indexación. El valor predeterminado es  1 .


**Returns:**
int - El número de hilos usados para la indexación.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


Establece el número de hilos usados para la indexación. El valor predeterminado es  1 .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | int | El número de hilos usados para la indexación. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


Obtiene la bandera de ejecución asíncrona de la operación. El valor predeterminado es  false .


**Returns:**
boolean - La bandera de ejecución asíncrona de la operación.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


Establece la bandera de ejecución asíncrona de la operación. El valor predeterminado es  false .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | La bandera de ejecución asíncrona de la operación. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


Obtiene el objeto de cancelación de la operación. El valor predeterminado es  null .


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


Establece el objeto de cancelación de la operación. El valor predeterminado es  null .


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | El objeto de cancelación de la operación. |
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
