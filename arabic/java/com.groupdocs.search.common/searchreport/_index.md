---
title: "SearchReport"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل معلومات مفصلة عن عملية البحث."
type: docs
weight: 30
url: /ar/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

يمثل معلومات مفصلة عن عملية البحث.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// إنشاء فهرس في المجلد المحدد
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentsFolder);
// البحث في الفهرس
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// الحصول على تقارير البحث
SearchReport[] reports = index.getSearchReports();
// طباعة التقارير إلى وحدة التحكم
for (SearchReport report : reports) {
System.out.println("Query: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getSearchDuration());
System.out.println("Documents: " + report.getDocumentCount());
System.out.println("Occurrences: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | يحصل على وقت بدء البحث. |
|
|  | [getEndTime()](#getEndTime--) | يحصل على وقت انتهاء البحث. |
|
|  | [getSearchDuration()](#getSearchDuration--) | يحصل على مدة البحث بالثواني. |
|
|  | [getDocumentCount()](#getDocumentCount--) | يحصل على عدد المستندات التي تم العثور عليها. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | يحصل على إجمالي عدد التكرارات التي تم العثور عليها. |
|
|  | [getTextQuery()](#getTextQuery--) | يحصل على استعلام البحث في شكل نصي. |
|
|  | [getObjectQuery()](#getObjectQuery--) | يحصل على استعلام البحث في شكل كائن. |
|
|  | [getSearchOptions()](#getSearchOptions--) | يحصل على خيارات البحث. |
|
|  | [toString()](#toString--) | يرجع سلسلة تمثل تقرير البحث الحالي. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


يحصل على وقت بدء البحث.


**Returns:**
java.util.Date - وقت بدء البحث.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


يحصل على وقت انتهاء البحث.


**Returns:**
java.util.Date - وقت انتهاء البحث.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


يحصل على مدة البحث بالثواني.


**Returns:**
double - مدة البحث بالثواني.

### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


يحصل على عدد المستندات التي تم العثور عليها.


**Returns:**
int - عدد المستندات التي تم العثور عليها.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


يحصل على إجمالي عدد التكرارات التي تم العثور عليها.


**Returns:**
int - إجمالي عدد التكرارات التي تم العثور عليها.

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


يحصل على استعلام البحث في شكل نصي.


**Returns:**
java.lang.String - استعلام البحث في شكل نصي.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


يحصل على استعلام البحث في شكل كائن.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


يحصل على خيارات البحث.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


يرجع سلسلة تمثل تقرير البحث الحالي.


**Returns:**
java.lang.String - سلسلة تمثل تقرير البحث الحالي.

