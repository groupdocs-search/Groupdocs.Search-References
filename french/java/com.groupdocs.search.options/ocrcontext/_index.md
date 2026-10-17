---
title: "OcrContext"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente le contexte de traitement OCR."
type: docs
weight: 30
url: /fr/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Représente le contexte de traitement OCR.

## Constructeurs

| Constructeur | Description |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Initialise une nouvelle instance de la |
OcrContext
classe.
|
## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Obtient le flux contenant l’image à traiter. |
|
|  | [getImageLocation()](#getImageLocation--) | Obtient l’emplacement de l’image. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Obtient l’extension de fichier de l’image. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Initialise une nouvelle instance de la
OcrContext
classe.


**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Le flux contenant l’image à traiter. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | L’emplacement de l’image. |
|
|  | imageFileExtension | java.lang.String | L’extension de fichier de l’image. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Obtient le flux contenant l’image à traiter.


**Returns:**
java.io.InputStream - Le flux contenant l’image à traiter.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Obtient l’emplacement de l’image.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Obtient l’extension de fichier de l’image.
Cette valeur peut être utilisée pour déterminer le type de l’image.


**Returns:**
java.lang.String - L’extension de fichier de l’image.

