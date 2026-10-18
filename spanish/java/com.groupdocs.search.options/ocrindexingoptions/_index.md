---
title: "OcrIndexingOptions"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Proporciona opciones para el procesamiento OCR e indexación del texto reconocido."
type: docs
weight: 31
url: /es/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

Proporciona opciones para el procesamiento OCR e indexación del texto reconocido.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | Obtiene un valor que indica si se debe reconocer texto en archivos de imagen separados. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | Establece un valor que indica si se debe reconocer texto en archivos de imagen separados. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | Obtiene un valor que indica si se debe reconocer texto en imágenes que son elementos de un contenedor (por ejemplo, imágenes en un archivo ZIP). |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | Establece un valor que indica si se debe reconocer texto en imágenes que son elementos de un contenedor (por ejemplo, imágenes en un archivo ZIP). |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | Obtiene un valor que indica si se debe reconocer texto en imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | Establece un valor que indica si se debe reconocer texto en imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). |
|
|  | [getOcrConnector()](#getOcrConnector--) | Obtiene un conector OCR que se utiliza para el procesamiento OCR. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | Establece un conector OCR que se utiliza para el procesamiento OCR. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


Obtiene un valor que indica si se debe reconocer texto en archivos de imagen separados. El valor predeterminado es false.


**Returns:**
boolean - Un valor que indica si se debe reconocer texto en archivos de imagen separados.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


Establece un valor que indica si se debe reconocer texto en archivos de imagen separados. El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se debe reconocer texto en archivos de imagen separados. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


Obtiene un valor que indica si se debe reconocer texto en imágenes que son elementos de un contenedor (por ejemplo, imágenes en un archivo ZIP). El valor predeterminado es false.


**Returns:**
boolean - Un valor que indica si se debe reconocer texto en imágenes que son elementos de un contenedor.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


Establece un valor que indica si se debe reconocer texto en imágenes que son elementos de un contenedor (por ejemplo, imágenes en un archivo ZIP). El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se debe reconocer texto en imágenes que son elementos de un contenedor. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


Obtiene un valor que indica si se debe reconocer texto en imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). El valor predeterminado es false.


**Returns:**
boolean - Un valor que indica si se debe reconocer texto en imágenes incrustadas.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


Establece un valor que indica si se debe reconocer texto en imágenes incrustadas (por ejemplo, imágenes en un documento DOCX). El valor predeterminado es false.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | valor | boolean | Un valor que indica si se debe reconocer texto en imágenes incrustadas. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


Obtiene un conector OCR que se utiliza para el procesamiento OCR. El valor predeterminado es null, lo que significa que no se usa OCR.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


Establece un conector OCR que se utiliza para el procesamiento OCR. El valor predeterminado es null, lo que significa que no se usa OCR.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | Un conector OCR que se utiliza para el procesamiento OCR. |
|

