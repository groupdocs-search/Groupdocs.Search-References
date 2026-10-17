---
title: "StringOutputAdapter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل محول إخراج يجمع الإخراج كـ System.String."
type: docs
weight: 32
url: /ar/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

يمثل محول إخراج يجمع الإخراج كـ System.String.


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
StringOutputAdapter adapter = new StringOutputAdapter(); // إنشاء محول إخراج نصي
index.getDocumentText(documents[0], adapter); // توليد نص المستند داخل المحول
String result = adapter.getResult(); // الحصول على نتيجة
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | ينشئ مثيلاً جديداً من الفئة  StringOutputAdapter  . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getResult()](#getResult--) | يحصل على السلسلة الناتجة. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


ينشئ مثيلاً جديداً من الفئة  StringOutputAdapter  .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | تنسيق الإخراج. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


يحصل على السلسلة الناتجة.


**Returns:**
java.lang.String - السلسلة الناتجة.

