---
title: "IOcrConnector"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이미지 문서 및 포함된 이미지에서 텍스트를 인식하는 데 필요한 메서드를 정의합니다."
type: docs
weight: 45
url: /ko/java/com.groupdocs.search.options/iocrconnector/
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

