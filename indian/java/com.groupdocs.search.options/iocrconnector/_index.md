---
title: "IOcrConnector"
second_title: "GroupDocs.Search for Java API Reference"
description: "इमेज दस्तावेज़ों और एम्बेडेड इमेजेज़ पर टेक्स्ट पहचानने के लिए आवश्यक मेथड्स को परिभाषित करता है।"
type: docs
weight: 45
url: /hi/java/com.groupdocs.search.options/iocrconnector/
---```
public interface IOcrConnector
```

Defines methods that are required to recognize text on image documents and embedded images.

## Methods

| Method | Description |
| --- | --- |
| [recognize(OcrContext context)](#recognize-com.groupdocs.search.options.OcrContext-) | Performs OCR processing on an image.
 |
### recognize(OcrContext context) {#recognize-com.groupdocs.search.options.OcrContext-}
```
public abstract String recognize(OcrContext context)
```


Performs OCR processing on an image.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| context | [OcrContext](../../com.groupdocs.search.options/ocrcontext) | The OCR processing context.
 |

**Returns:**
java.lang.String - The recognized text.

