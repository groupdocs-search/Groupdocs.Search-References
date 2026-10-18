---
title: "OcrContext"
second_title: "GroupDocs.Search for Java API Reference"
description: "OCR प्रोसेसिंग संदर्भ को दर्शाता है।"
type: docs
weight: 30
url: /hi/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

OCR प्रोसेसिंग संदर्भ को दर्शाता है।

## निर्माता

| निर्माता | विवरण |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | नया उदाहरण प्रारंभ करता है |
OcrContext
वर्ग।
|
## मेथड्स

| मेथड | विवरण |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | छवि को प्रोसेस करने वाले स्ट्रीम को प्राप्त करता है। |
|
|  | [getImageLocation()](#getImageLocation--) | छवि का स्थान प्राप्त करता है। |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | छवि का फ़ाइल एक्सटेंशन प्राप्त करता है। |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


नया उदाहरण प्रारंभ करता है
OcrContext
वर्ग।


**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | छवि को प्रोसेस करने वाला स्ट्रीम। |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | छवि का स्थान। |
|
|  | imageFileExtension | java.lang.String | छवि का फ़ाइल एक्सटेंशन। |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


छवि को प्रोसेस करने वाले स्ट्रीम को प्राप्त करता है।


**Returns:**
java.io.InputStream - छवि को प्रोसेस करने वाला स्ट्रीम।

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


छवि का स्थान प्राप्त करता है।


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


छवि का फ़ाइल एक्सटेंशन प्राप्त करता है।
इस मान का उपयोग छवि के प्रकार को निर्धारित करने के लिए किया जा सकता है।


**Returns:**
java.lang.String - छवि का फ़ाइल एक्सटेंशन।

