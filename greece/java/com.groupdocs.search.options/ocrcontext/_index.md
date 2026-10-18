---
title: "OcrContext"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αναπαριστά το πλαίσιο επεξεργασίας OCR."
type: docs
weight: 30
url: /el/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

Αναπαριστά το πλαίσιο επεξεργασίας OCR.

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της |
OcrContext
κλάσης.
|
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | Λαμβάνει τη ροή που περιέχει την εικόνα προς επεξεργασία. |
|
|  | [getImageLocation()](#getImageLocation--) | Λαμβάνει τη θέση της εικόνας. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | Λαμβάνει την επέκταση αρχείου της εικόνας. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


Αρχικοποιεί μια νέα παρουσία της
OcrContext
κλάσης.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | Η ροή που περιέχει την εικόνα προς επεξεργασία. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | Η θέση της εικόνας. |
|
|  | imageFileExtension | java.lang.String | Η επέκταση αρχείου της εικόνας. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


Λαμβάνει τη ροή που περιέχει την εικόνα προς επεξεργασία.


**Returns:**
java.io.InputStream - Η ροή που περιέχει την εικόνα προς επεξεργασία.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


Λαμβάνει τη θέση της εικόνας.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


Λαμβάνει την επέκταση αρχείου της εικόνας.
Αυτή η τιμή μπορεί να χρησιμοποιηθεί για τον προσδιορισμό του τύπου της εικόνας.


**Returns:**
java.lang.String - Η επέκταση αρχείου της εικόνας.

