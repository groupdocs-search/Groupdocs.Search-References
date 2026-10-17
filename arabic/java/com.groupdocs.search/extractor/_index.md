---
title: "Extractor"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل أداة لاستخراج البيانات الأولية من المستندات لفصل مرحلة الفهرسة السريعة اللاحقة."
type: docs
weight: 16
url: /ar/java/com.groupdocs.search/extractor/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventHubBase](../../com.groupdocs.search.events/eventhubbase)
```
public class Extractor extends EventHubBase
```

يمثل أداة لاستخراج البيانات الأولية من المستندات لفصل مرحلة الفهرسة السريعة اللاحقة.

## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [Extractor()](#Extractor--) | ينشئ مثيلاً جديداً من الفئة Extractor. |
|
## الحقول

| حقل | الوصف |
| --- | --- |
|  | [ErrorOccurred](#ErrorOccurred) | يحدث عندما يحدث خطأ أثناء عملية المستخرج. |
|
|  | [ImagePreparing](#ImagePreparing) | يحدث عندما يتم إعداد صورة للفهرسة. |
|
|  | [PasswordRequired](#PasswordRequired) | يحدث عندما يتطلب المستند كلمة مرور للفتح. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getSettings()](#getSettings--) | يحصل على إعدادات المستخرج. |
|
|  | [extract(Document document, ExtractionOptions extractionOptions)](#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-) | يستخرج البيانات من مستند. |
|
| [raiseErrorOccurredPublic(String message, boolean isCritical)](#raiseErrorOccurredPublic-java.lang.String-boolean-) |  |
| [raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)](#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-) |  |
| [raisePasswordRequiredPublic(String filePath)](#raisePasswordRequiredPublic-java.lang.String-) |  |
### Extractor() {#Extractor--}
```
public Extractor()
```


ينشئ مثيلاً جديداً من الفئة Extractor.


### ErrorOccurred {#ErrorOccurred}
```
public final Event<EventHandler<IndexErrorEventArgs>> ErrorOccurred
```


يحدث عندما يحدث خطأ أثناء عملية المستخرج.


### ImagePreparing {#ImagePreparing}
```
public final Event<EventHandler<ImagePreparingEventArgs>> ImagePreparing
```


يحدث عندما يتم إعداد صورة للفهرسة.


### PasswordRequired {#PasswordRequired}
```
public final Event<EventHandler<PasswordRequiredEventArgs>> PasswordRequired
```


يحدث عندما يتطلب المستند كلمة مرور للفتح.


### getSettings() {#getSettings--}
```
public final ExtractorSettings getSettings()
```


يحصل على إعدادات المستخرج.


**Returns:**
[ExtractorSettings](../../com.groupdocs.search.common/extractorsettings) - The extractor settings.

### extract(Document document, ExtractionOptions extractionOptions) {#extract-com.groupdocs.search.Document-com.groupdocs.search.options.ExtractionOptions-}
```
public final ExtractedData extract(Document document, ExtractionOptions extractionOptions)
```


يستخرج البيانات من مستند.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | document | [Document](../../com.groupdocs.search/document) | المستند من نظام الملفات أو التدفق أو الهيكل. |
|
|  | extractionOptions | [ExtractionOptions](../../com.groupdocs.search.options/extractionoptions) | خيارات الاستخراج. |
|

**Returns:**
[ExtractedData](../../com.groupdocs.search/extracteddata) - The extracted data of the document.

### raiseErrorOccurredPublic(String message, boolean isCritical) {#raiseErrorOccurredPublic-java.lang.String-boolean-}
```
public final void raiseErrorOccurredPublic(String message, boolean isCritical)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| رسالة | java.lang.String |  |
| isCritical | boolean |  |

### raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream) {#raiseImagePreparingPublic-java.lang.String-java.lang.String---int-com.groupdocs.search.common.ImageFrame---java.io.InputStream-}
```
public final void raiseImagePreparingPublic(String documentKey, String[] innerPath, int imageIndex, ImageFrame[] frames, InputStream stream)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| documentKey | java.lang.String |  |
| innerPath | java.lang.String[] |  |
| imageIndex | int |  |
| frames | [ImageFrame\[\]](../../com.groupdocs.search.common/imageframe) |  |
| stream | java.io.InputStream |  |

### raisePasswordRequiredPublic(String filePath) {#raisePasswordRequiredPublic-java.lang.String-}
```
public final String raisePasswordRequiredPublic(String filePath)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| filePath | java.lang.String |  |

**Returns:**
java.lang.String
