---
title: "ImagePreparingEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos del evento de inicio de la preparación de una imagen."
type: docs
weight: 15
url: /es/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

Representa los argumentos del evento de inicio de la preparación de una imagen.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | Obtiene la clave del documento. |
|
|  | [getInnerPath()](#getInnerPath--) | Obtiene la ruta interna de un documento anidado. |
|
|  | [getImageIndex()](#getImageIndex--) | Obtiene el número ordinal de la imagen en el documento. |
|
|  | [getImageFrames()](#getImageFrames--) | Obtiene los fotogramas de la imagen. |
|
|  | [getImageStream()](#getImageStream--) | Obtiene el flujo de la imagen. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Obtiene la clave del documento.


**Returns:**
java.lang.String - La clave del documento.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


Obtiene la ruta interna de un documento anidado.


**Returns:**
java.lang.String[] - La ruta interna de un documento anidado.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Obtiene el número ordinal de la imagen en el documento.


**Returns:**
int - El número ordinal de la imagen en el documento.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


Obtiene los fotogramas de la imagen.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - Los fotogramas de la imagen.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Obtiene el flujo de la imagen.


**Returns:**
java.io.InputStream - El flujo de la imagen.

