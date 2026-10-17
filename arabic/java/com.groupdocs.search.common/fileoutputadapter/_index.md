---
title: "FileOutputAdapter"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل محول إخراج يجمع المخرجات في ملف."
type: docs
weight: 21
url: /ar/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

يمثل محول إخراج يجمع المخرجات في ملف.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // إنشاء محول إخراج ملف
index.getDocumentText(documents[0], adapter); // توليد نص المستند إلى ملف الإخراج
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | ينشئ مثيلًا جديدًا من فئة  FileOutputAdapter . |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | يحصل على مسار ملف الإخراج. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


ينشئ مثيلًا جديدًا من فئة  FileOutputAdapter .


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | تنسيق الإخراج. |
|
|  | filePath | java.lang.String | مسار ملف الإخراج. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


يحصل على مسار ملف الإخراج.


**Returns:**
java.lang.String - مسار ملف الإخراج.

