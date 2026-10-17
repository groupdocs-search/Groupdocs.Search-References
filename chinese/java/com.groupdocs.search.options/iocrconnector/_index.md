---
title: "IOcrConnector"
second_title: "GroupDocs.Search 用于 Java 的 API 参考"
description: "定义识别图像文档和嵌入图像中文本所需的方法。"
type: docs
weight: 45
url: /zh/java/com.groupdocs.search.options/iocrconnector/
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

