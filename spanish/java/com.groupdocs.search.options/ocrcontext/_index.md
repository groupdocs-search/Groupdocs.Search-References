---
title: "OcrContext"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa el contexto de procesamiento OCR."
type: docs
weight: 30
url: /es/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Representa el contexto de procesamiento OCR.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Inicializa una nueva instancia de la |
OcrContext
clase.
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Obtiene el flujo que contiene la imagen a procesar. |
|
|  | [getImageLocation()](#getImageLocation--) | Obtiene la ubicación de la imagen. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Obtiene la extensión de archivo de la imagen. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Inicializa una nueva instancia de la
OcrContext
clase.


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | El flujo que contiene la imagen a procesar. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | La ubicación de la imagen. |
|
|  | imageFileExtension | java.lang.String | La extensión de archivo de la imagen. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Obtiene el flujo que contiene la imagen a procesar.


**Returns:**
java.io.InputStream - El flujo que contiene la imagen a procesar.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Obtiene la ubicación de la imagen.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Obtiene la extensión de archivo de la imagen.
Este valor puede usarse para determinar el tipo de la imagen.


**Returns:**
java.lang.String - La extensión de archivo de la imagen.

