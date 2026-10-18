---
title: "OcrContext"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta il contesto di elaborazione OCR."
type: docs
weight: 30
url: /it/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Rappresenta il contesto di elaborazione OCR.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Inizializza una nuova istanza di |
OcrContext
classe.
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Ottiene lo stream contenente l'immagine da elaborare. |
|
|  | [getImageLocation()](#getImageLocation--) | Ottiene la posizione dell'immagine. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Ottiene l'estensione del file dell'immagine. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Inizializza una nuova istanza di
OcrContext
classe.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Lo stream contenente l'immagine da elaborare. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | La posizione dell'immagine. |
|
|  | imageFileExtension | java.lang.String | L'estensione del file dell'immagine. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Ottiene lo stream contenente l'immagine da elaborare.


**Returns:**
java.io.InputStream - Lo stream contenente l'immagine da elaborare.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Ottiene la posizione dell'immagine.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Ottiene l'estensione del file dell'immagine.
Questo valore può essere usato per determinare il tipo dell'immagine.


**Returns:**
java.lang.String - L'estensione del file dell'immagine.

