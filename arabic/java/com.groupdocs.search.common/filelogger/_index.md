---
title: "FileLogger"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل مسجلًا يسجل الأحداث والأخطاء في ملف محلي."
type: docs
weight: 20
url: /ar/java/com.groupdocs.search.common/filelogger/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.common.ILogger](../../com.groupdocs.search.common/ilogger)
```
public class FileLogger implements ILogger
```

يمثل مسجلًا يسجل الأحداث والأخطاء في ملف محلي.


**Learn more**

* [Logging](../https://docs.groupdocs.com/display/searchjava/Logging)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
String logPath = "c:\\Log.txt";
IndexSettings settings = new IndexSettings();
settings.setLogger(new FileLogger(logPath, 4.0)); // تحديد مسار ملف السجل والحد الأقصى للطول 4 ميغابايت
Index index = new Index(indexFolder, settings); // إنشاء فهرس في المجلد المحدد
index.add(documentsFolder); // فهرسة المستندات من المجلد المحدد
SearchResult result = index.search(query); // البحث في الفهرس
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
|  | [FileLogger(String filePath, double maxSize)](#FileLogger-java.lang.String-double-) | يُنشئ مثيلاً جديدًا من فئة FileLogger. |
|
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [error(String message)](#error-java.lang.String-) | يسجل خطأً حدث في الفهرس. |
|
|  | [trace(String message)](#trace-java.lang.String-) | يسجل حدثًا حدث في الفهرس. |
|
|  | [getFilePath()](#getFilePath--) | يحصل على مسار ملف السجل. |
|
|  | [getMaxSize()](#getMaxSize--) | يحصل على الحد الأقصى لحجم ملف السجل بالميغابايت. |
|
### FileLogger(String filePath, double maxSize) {#FileLogger-java.lang.String-double-}
```
public FileLogger(String filePath, double maxSize)
```


يُنشئ مثيلاً جديدًا من فئة FileLogger.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | filePath | java.lang.String | مسار ملف السجل. |
|
|  | maxSize | double | الحد الأقصى لحجم ملف السجل بالميغابايت. يجب أن تكون القيمة في النطاق من 0.1 إلى 1000. |
|

### error(String message) {#error-java.lang.String-}
```
public final void error(String message)
```


يسجل خطأً حدث في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | رسالة | java.lang.String | رسالة الخطأ. |
|

### trace(String message) {#trace-java.lang.String-}
```
public final void trace(String message)
```


يسجل حدثًا حدث في الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | رسالة | java.lang.String | رسالة الحدث. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


يحصل على مسار ملف السجل.


**Returns:**
java.lang.String - مسار ملف السجل.

### getMaxSize() {#getMaxSize--}
```
public final double getMaxSize()
```


يحصل على الحد الأقصى لحجم ملف السجل بالميغابايت.


**Returns:**
double - الحد الأقصى لحجم ملف السجل بالميغابايت.

