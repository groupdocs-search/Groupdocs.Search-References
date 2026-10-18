---
title: "OcrContext"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de OCR-verwerkingscontext voor."
type: docs
weight: 30
url: /nl/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Stelt de OCR-verwerkingscontext voor.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Initialiseert een nieuw exemplaar van de |
OcrContext
klasse.
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Haalt de stream op die de te verwerken afbeelding bevat. |
|
|  | [getImageLocation()](#getImageLocation--) | Haalt de locatie van de afbeelding op. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Haalt de bestandsextensie van de afbeelding op. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Initialiseert een nieuw exemplaar van de
OcrContext
klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | De stream die de te verwerken afbeelding bevat. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | De locatie van de afbeelding. |
|
|  | imageFileExtension | java.lang.String | De bestandsextensie van de afbeelding. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Haalt de stream op die de te verwerken afbeelding bevat.


**Returns:**
java.io.InputStream - De stream die de te verwerken afbeelding bevat.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Haalt de locatie van de afbeelding op.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Haalt de bestandsextensie van de afbeelding op.
Deze waarde kan worden gebruikt om het type van de afbeelding te bepalen.


**Returns:**
java.lang.String - De bestandsextensie van de afbeelding.

