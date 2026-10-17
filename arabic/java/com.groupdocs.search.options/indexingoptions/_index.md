---
title: "IndexingOptions"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يوفر خيارات لعملية الفهرسة."
type: docs
weight: 25
url: /ar/java/com.groupdocs.search.options/indexingoptions/
---
**Inheritance:**
java.lang.Object
```
public class IndexingOptions
```

يوفر خيارات لعملية الفهرسة.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [IndexingOptions()](#IndexingOptions--) | ينشئ مثيلاً جديداً من فئة  IndexingOptions  . |
|
|  | [IndexingOptions(Object data)](#IndexingOptions-java.lang.Object-) | ينشئ مثيلاً جديداً من فئة  IndexingOptions  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getThreads()](#getThreads--) | يحصل على عدد الخيوط المستخدمة في الفهرسة. |
|
|  | [setThreads(int value)](#setThreads-int-) | يضبط عدد الخيوط المستخدمة في الفهرسة. |
|
|  | [isAsync()](#isAsync--) | يحصل على علم تنفيذ العملية بشكل غير متزامن. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | يضبط علم تنفيذ العملية بشكل غير متزامن. |
|
|  | [getCancellation()](#getCancellation--) | يحصل على كائن إلغاء العملية. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | يضبط كائن إلغاء العملية. |
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
### IndexingOptions() {#IndexingOptions--}
```
public IndexingOptions()
```


ينشئ مثيلاً جديداً من فئة  IndexingOptions  .


### IndexingOptions(Object data) {#IndexingOptions-java.lang.Object-}
```
public IndexingOptions(Object data)
```


ينشئ مثيلاً جديداً من فئة  IndexingOptions  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | البيانات | java.lang.Object | البيانات المتسلسلة. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


يحصل على عدد الخيوط المستخدمة في الفهرسة. القيمة الافتراضية هي 1.


**Returns:**
int - عدد الخيوط المستخدمة للفهرسة.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


يضبط عدد الخيوط المستخدمة للفهرسة. القيمة الافتراضية هي 1.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | int | عدد الخيوط المستخدمة للفهرسة. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


يحصل على علامة التنفيذ غير المتزامن للعملية. القيمة الافتراضية هي false.


**Returns:**
boolean - علامة التنفيذ غير المتزامن للعملية.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


يضبط علامة التنفيذ غير المتزامن للعملية. القيمة الافتراضية هي false.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | قيمة | boolean | علامة التنفيذ غير المتزامن للعملية. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


يحصل على كائن إلغاء العملية. القيمة الافتراضية هي null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


يضبط كائن إلغاء العملية. القيمة الافتراضية هي null.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | كائن إلغاء العملية. |
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
