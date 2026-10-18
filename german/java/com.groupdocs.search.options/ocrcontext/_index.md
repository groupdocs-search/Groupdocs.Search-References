---
title: "OcrContext"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt den OCR-Verarbeitungskontext dar."
type: docs
weight: 30
url: /de/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Stellt den OCR-Verarbeitungskontext dar.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Initialisiert eine neue Instanz von |
OcrContext
Klasse.
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Liefert den Stream, der das zu verarbeitende Bild enthält. |
|
|  | [getImageLocation()](#getImageLocation--) | Liefert den Speicherort des Bildes. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Liefert die Dateierweiterung des Bildes. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Initialisiert eine neue Instanz von
OcrContext
Klasse.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Der Stream, der das zu verarbeitende Bild enthält. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | Der Speicherort des Bildes. |
|
|  | imageFileExtension | java.lang.String | Die Dateierweiterung des Bildes. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Liefert den Stream, der das zu verarbeitende Bild enthält.


**Returns:**
java.io.InputStream - Der Stream, der das zu verarbeitende Bild enthält.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Liefert den Speicherort des Bildes.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Liefert die Dateierweiterung des Bildes.
Dieser Wert kann verwendet werden, um den Typ des Bildes zu bestimmen.


**Returns:**
java.lang.String - Die Dateierweiterung des Bildes.

