---
title: "TextOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لاسترجاع نص المستند من الفهرس."
type: docs
weight: 41
url: /ar/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

يوفر خيارات لاسترجاع نص المستند من الفهرس.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | يُنشئ مثيلاً جديدًا لفئة  TextOptions . |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | يُنشئ مثيلاً جديدًا لفئة  TextOptions . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | يحصل على مستخرج النص المخصص الذي تم استخدامه للفهرسة. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | يضبط مستخرج النص المخصص الذي تم استخدامه للفهرسة. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | يحصل على حقول المستند الإضافية التي تم استخدامها للفهرسة. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | يضبط حقول المستند الإضافية التي تم استخدامها للفهرسة. |
|
|  | [getCancellation()](#getCancellation--) | يحصل على كائن الإلغاء. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | يضبط كائن الإلغاء. |
|
|  | [getGenerateHead()](#getGenerateHead--) | يحصل على قيمة تشير إلى ما إذا كان وسم Head يتم إنشاؤه في HTML الناتج. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | يضبط قيمة تشير إلى ما إذا كان وسم Head يتم إنشاؤه في HTML الناتج. |
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
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


يُنشئ مثيلاً جديدًا لفئة  TextOptions .


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


يُنشئ مثيلاً جديدًا لفئة  TextOptions .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


يحصل على مستخرج النص المخصص الذي تم استخدامه للفهرسة. القيمة الافتراضية هي null. لاحظ أن هذه القيمة تُستخدم فقط إذا لم يتم حفظ نص المستند في الفهرس.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


يضبط مستخرج النص المخصص الذي تم استخدامه للفهرسة. القيمة الافتراضية هي null. لاحظ أن هذه القيمة تُستخدم فقط إذا لم يتم حفظ نص المستند في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | مستخرج النص المخصص الذي تم استخدامه للفهرسة. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


يحصل على حقول المستند الإضافية التي تم استخدامها للفهرسة. القيمة الافتراضية هي null. لاحظ أن هذه القيمة تُستخدم فقط إذا لم يتم حفظ نص المستند في الفهرس.


**Returns:**
com.groupdocs.search.common.DocumentField[] - حقول المستند الإضافية التي تم استخدامها للفهرسة.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


يضبط حقول المستند الإضافية التي تم استخدامها للفهرسة. القيمة الافتراضية هي null. لاحظ أن هذه القيمة تُستخدم فقط إذا لم يتم حفظ نص المستند في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | حقول المستند الإضافية التي تم استخدامها للفهرسة. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


يحصل على كائن الإلغاء. القيمة الافتراضية هي null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


يضبط كائن الإلغاء. القيمة الافتراضية هي null.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | كائن الإلغاء. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


يحصل على قيمة تشير إلى ما إذا كان وسم Head يتم إنشاؤه في HTML الناتج. القيمة الافتراضية هي true.


**Returns:**
boolean - قيمة تشير إلى ما إذا كان وسم Head يتم إنشاؤه في HTML الناتج.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان وسم Head يتم إنشاؤه في HTML الناتج. القيمة الافتراضية هي true.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | قيمة تشير إلى ما إذا كان وسم Head يتم إنشاؤه في HTML الناتج. |
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
