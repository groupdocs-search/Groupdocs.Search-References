---
title: "StreamOutputAdapter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل محول إخراج يجمع الإخراج في java.io.OutputStream."
type: docs
weight: 31
url: /ar/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

يمثل محول إخراج يجمع الإخراج في java.io.OutputStream.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
DocumentInfo[] documents = index.getIndexedDocuments(); // الحصول على معلومات حول المستندات المفهرسة
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // إنشاء تدفق إخراج
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // إنشاء محول إخراج تدفق
index.getDocumentText(documents[0], adapter); // توليد نص المستند داخل التدفق
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | يُنشئ مثيلاً جديدًا من فئة StreamOutputAdapter. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getStream()](#getStream--) | يحصل على تدفق إخراج. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


يُنشئ مثيلاً جديدًا من فئة StreamOutputAdapter.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | تنسيق الإخراج. |
|
|  | stream | java.io.OutputStream | تدفق الإخراج. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


يحصل على تدفق إخراج.


**Returns:**
java.io.OutputStream - تدفق الإخراج.

