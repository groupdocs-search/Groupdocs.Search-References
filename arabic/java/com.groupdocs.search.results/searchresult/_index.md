---
title: "SearchResult"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل نتيجة بحث تتطابق مع استعلام البحث."
type: docs
weight: 19
url: /ar/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

يمثل نتيجة بحث تتطابق مع استعلام البحث.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


المثال يوضح استخدامًا نموذجيًا للفئة.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// إنشاء فهرس
Index index = new Index(indexFolder);
// فهرسة المستندات من المجلد المحدد
index.add(documentFolder);
// ضبط خيارات البحث
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // تمكين بحث Fuzzy
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // ضبط الحد الأقصى لعدد الاختلافات إلى 3
// البحث عن مستندات تحتوي على الكلمة 'Einstein' أو العبارة 'Theory of Relativity'
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// طباعة النتيجة
System.out.println(\"المستندات: \" + result.getDocumentCount());
System.out.println(\"إجمالي التكرارات: \" + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println(\"\tالمستند: \" + document.getDocumentInfo().getFilePath());
System.out.println(\"\tالتكرارات: \" + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println(\"\t\tالحقل: \" + field.getFieldName());
System.out.println(\"\t\tالتكرارات: \" + document.getOccurrenceCount());
// طباعة المصطلحات المكتشفة
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println(\"\t\t\t\" + field.getTerms()[k] + \" - \" + field.getTermsOccurrences()[k]);
}
}
// طباعة العبارات المكتشفة
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | يحصل على عدد المستندات التي تم العثور عليها. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | يحصل على إجمالي عدد التكرارات التي تم العثور عليها. |
|
|  | [getTruncated()](#getTruncated--) | يحصل على قيمة تشير إلى أن النتيجة مقطوعة. |
|
|  | [getWarnings()](#getWarnings--) | يحصل على تحذير يصف النتيجة. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | يحصل على رمز بحث القطعة للبحث عن القطعة التالية. |
|
|  | [getStartTime()](#getStartTime--) | يحصل على وقت بدء البحث. |
|
|  | [getEndTime()](#getEndTime--) | يحصل على وقت انتهاء البحث. |
|
|  | [getSearchDuration()](#getSearchDuration--) | يحصل على مدة البحث بالثواني. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | يحصل على المستند الموجود حسب الفهرس. |
|
|  | [iterator()](#iterator--) | يرجع مُكرِّرًا يتنقل عبر مجموعة المستندات التي تم العثور عليها. |
|
### SearchResult() {#SearchResult--}
```
public SearchResult()
```


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

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


يحصل على قيمة تشير إلى أن النتيجة مقطوعة.


**Returns:**
boolean - قيمة تشير إلى أن النتيجة مقطوعة.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


يحصل على تحذير يصف النتيجة.


**Returns:**
java.lang.String - تحذير يصف النتيجة.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


يحصل على رمز بحث القطعة للبحث عن القطعة التالية.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract FoundDocument getFoundDocument(int index)
```


يحصل على المستند الموجود حسب الفهرس.


**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
|  | الفهرس | int | فهرس المستند الذي تم العثور عليه. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


يرجع مُكرِّرًا يتنقل عبر مجموعة المستندات التي تم العثور عليها.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - مكرّر يمكن استخدامه للتنقل عبر مجموعة المستندات التي تم العثور عليها.

