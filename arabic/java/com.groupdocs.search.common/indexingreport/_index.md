---
title: "IndexingReport"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل معلومات تفصيلية عن عملية الفهرسة."
type: docs
weight: 25
url: /ar/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

يمثل معلومات تفصيلية عن عملية الفهرسة.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات
index.add(documentsFolder1);
index.add(documentsFolder2);
// الحصول على تقارير الفهرسة
IndexingReport[] reports = index.getIndexingReports();
// طباعة التقارير إلى وحدة التحكم
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | يحصل على إجمالي عدد المستندات في الفهرس. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | يحصل على إجمالي عدد المصطلحات في الفهرس. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | يحصل على الطول الإجمالي للمستندات المفهرسة بالميغابايت. |
|
|  | [getSegmentCount()](#getSegmentCount--) | يحصل على عدد مقاطع الفهرس. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | يحصل على الحجم الإجمالي للفهرس بالبايت. |
|
|  | [getStartTime()](#getStartTime--) | يحصل على وقت بدء الفهرسة. |
|
|  | [getEndTime()](#getEndTime--) | يحصل على وقت انتهاء الفهرسة. |
|
|  | [getIndexingTime()](#getIndexingTime--) | يحصل على مدة الفهرسة بالثواني. |
|
|  | [getErrors()](#getErrors--) | يحصل على قائمة الأخطاء. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | يحصل على قائمة المستندات المفهرسة. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | يحصل على قائمة المستندات المحدثة. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | يحصل على قائمة المستندات التي تم إزالتها من الفهرس. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


يحصل على إجمالي عدد المستندات في الفهرس.


**Returns:**
int - إجمالي عدد المستندات في الفهرس.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


يحصل على إجمالي عدد المصطلحات في الفهرس.


**Returns:**
int - إجمالي عدد المصطلحات في الفهرس.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


يحصل على الطول الإجمالي للمستندات المفهرسة بالميغابايت.


**Returns:**
double - الطول الإجمالي للمستندات المفهرسة بالميغابايت.

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


يحصل على عدد مقاطع الفهرس.


**Returns:**
int - عدد مقاطع الفهرس.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


يحصل على الحجم الإجمالي للفهرس بالبايت.


**Returns:**
long - الحجم الإجمالي للفهرس بالبايت.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


يحصل على وقت بدء الفهرسة.


**Returns:**
java.util.Date - وقت بدء الفهرسة.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


يحصل على وقت انتهاء الفهرسة.


**Returns:**
java.util.Date - وقت انتهاء الفهرسة.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


يحصل على مدة الفهرسة بالثواني.


**Returns:**
double - مدة الفهرسة بالثواني.

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


يحصل على قائمة الأخطاء.


**Returns:**
java.lang.String[] - قائمة الأخطاء.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


يحصل على قائمة المستندات المفهرسة.


**Returns:**
java.lang.String[] - قائمة المستندات المفهرسة.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


يحصل على قائمة المستندات المحدثة.


**Returns:**
java.lang.String[] - قائمة المستندات المحدثة.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


يحصل على قائمة المستندات التي تم إزالتها من الفهرس.


**Returns:**
java.lang.String[] - قائمة المستندات التي أزيلت من الفهرس.

