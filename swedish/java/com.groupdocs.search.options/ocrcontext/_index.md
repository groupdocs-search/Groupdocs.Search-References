---
title: "OcrContext"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar OCR-behandlingskontexten."
type: docs
weight: 30
url: /sv/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Representerar OCR-behandlingskontexten.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Initierar en ny instans av |
OcrContext
klassen.
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Hämtar strömmen som innehåller bilden som ska bearbetas. |
|
|  | [getImageLocation()](#getImageLocation--) | Hämtar bildens plats. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Hämtar bildens filändelse. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Initierar en ny instans av
OcrContext
klassen.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Strömmen som innehåller bilden som ska bearbetas. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | Bildens plats. |
|
|  | imageFileExtension | java.lang.String | Bildens filändelse. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Hämtar strömmen som innehåller bilden som ska bearbetas.


**Returns:**
java.io.InputStream - Strömmen som innehåller bilden som ska bearbetas.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Hämtar bildens plats.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Hämtar bildens filändelse.
Detta värde kan användas för att bestämma bildens typ.


**Returns:**
java.lang.String - Bildens filändelse.

