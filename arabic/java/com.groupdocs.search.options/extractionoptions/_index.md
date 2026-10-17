---
title: "ExtractionOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لاستخراج البيانات من المستندات."
type: docs
weight: 18
url: /ar/java/com.groupdocs.search.options/extractionoptions/
---
**Inheritance:**
java.lang.Object
```
public class ExtractionOptions
```

يوفر خيارات لاستخراج البيانات من المستندات.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [ExtractionOptions()](#ExtractionOptions--) | ينشئ مثيلاً جديداً من الفئة  ExtractionOptions  . |
|
|  | [ExtractionOptions(Object data)](#ExtractionOptions-java.lang.Object-) | ينشئ مثيلاً جديداً من الفئة  ExtractionOptions  . |
|
|  | [ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)](#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-) | ينشئ مثيلاً جديداً من الفئة  ExtractionOptions  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | يحصل على مستخرج النص المخصص. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | يضبط أو يضبط مستخرج النص المخصص. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | يحصل على قيمة تشير إلى ما إذا كان سيتم اكتشاف الترميز تلقائيًا أم لا. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم اكتشاف الترميز تلقائيًا أم لا. |
|
|  | [getEncoding()](#getEncoding--) | يحصل على الترميز المستخدم لاستخراج النص من المستندات النصية. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | يضبط الترميز المستخدم لاستخراج النص من المستندات النصية. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | يحصل على قيمة تشير إلى ما إذا كان سيتم استخدام الوضع الخام لاستخراج النص إذا كان ذلك ممكنًا. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | يضبط قيمة تشير إلى ما إذا كان سيتم استخدام الوضع الخام لاستخراج النص إذا كان ذلك ممكنًا. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | يحصل على الخيارات الخاصة بفهرسة حقول بيانات التعريف. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | يحصل على الخيارات الخاصة بمعالجة OCR وفهرسة النص المعترف به. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | يحصل على خيارات فهرسة الصور للبحث العكسي عن الصور. |
|
| [getCore()](#getCore--) |  |
### ExtractionOptions() {#ExtractionOptions--}
```
public ExtractionOptions()
```


ينشئ مثيلاً جديداً من الفئة  ExtractionOptions  .


### ExtractionOptions(Object data) {#ExtractionOptions-java.lang.Object-}
```
public ExtractionOptions(Object data)
```


ينشئ مثيلاً جديداً من الفئة  ExtractionOptions  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector) {#ExtractionOptions-com.groupdocs.search.options.IndexingOptions-com.groupdocs.search.common.IFieldExtractor-com.groupdocs.search.options.IOcrConnector-}
```
public ExtractionOptions(IndexingOptions options, IFieldExtractor customExtractor, IOcrConnector ocrConnector)
```


ينشئ مثيلاً جديداً من الفئة  ExtractionOptions  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | الخيارات. |
|
|  | customExtractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | المستخرج المخصص. |
|
|  | ocrConnector | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | موصل الـ ocr. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


يحصل على المستخرج النصي المخصص. القيمة الافتراضية هي null .


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


يضبط أو يضبط المستخرج النصي المخصص. القيمة الافتراضية هي null .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | المستخرج النصي المخصص. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


يحصل على قيمة تشير إلى ما إذا كان سيتم اكتشاف الترميز تلقائيًا أم لا. القيمة الافتراضية هي false.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان سيتم اكتشاف الترميز تلقائيًا أم لا.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان سيتم اكتشاف الترميز تلقائيًا أم لا. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان سيتم اكتشاف الترميز تلقائيًا أم لا. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


يحصل على الترميز المستخدم لاستخراج النص من المستندات النصية. القيمة الافتراضية هي null، مما يعني أن الترميز الافتراضي UTF-8 يُستخدم. إذا كان AutoDetectEncoding هو true فإن هذه القيمة تُستخدم كترميز افتراضي.


**Returns:**
java.lang.String - الترميز المستخدم لاستخراج النص من المستندات النصية.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


يضبط الترميز المستخدم لاستخراج النص من المستندات النصية. القيمة الافتراضية هي null، مما يعني أن الترميز الافتراضي UTF-8 يُستخدم. إذا كان AutoDetectEncoding هو true فإن هذه القيمة تُستخدم كترميز افتراضي.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | java.lang.String | الترميز المستخدم لاستخراج النص من المستندات النصية. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


يحصل على قيمة تشير إلى ما إذا كان وضع الخام يُستخدم لاستخراج النص إذا كان ذلك ممكنًا. القيمة الافتراضية هي true. يمكن لوضع الخام أن يزيد بشكل كبير من سرعة الفهرسة، لكن الوضع العادي يحسن تنسيق النص المستخرج.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان وضع الخام يُستخدم لاستخراج النص إذا كان ذلك ممكنًا.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان وضع الخام يُستخدم لاستخراج النص إذا كان ذلك ممكنًا. القيمة الافتراضية هي true. يمكن لوضع الخام أن يزيد بشكل كبير من سرعة الفهرسة، لكن الوضع العادي يحسن تنسيق النص المستخرج.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان وضع الخام يُستخدم لاستخراج النص إذا كان ذلك ممكنًا. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


يحصل على الخيارات الخاصة بفهرسة حقول بيانات التعريف.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


يحصل على الخيارات الخاصة بمعالجة OCR وفهرسة النص المعترف به.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


يحصل على خيارات فهرسة الصور للبحث العكسي عن الصور.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
