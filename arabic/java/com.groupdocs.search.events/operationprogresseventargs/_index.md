---
title: "OperationProgressEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث تحديث تقدم عملية الفهرسة."
type: docs
weight: 18
url: /ar/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لحدث تحديث تقدم عملية الفهرسة.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | يحصل على إجمالي عدد المستندات للمعالجة. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | يحصل على عدد المستندات التي تمت معالجتها بنجاح. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | يحصل على عدد المستندات المتخطاة. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | يحصل على نسبة التقدم. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | يحصل على مفتاح آخر مستند تمت معالجته. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | يحصل على مسار آخر مستند تمت معالجته. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | يحصل على حالة آخر مستند تمت معالجته. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


يحصل على إجمالي عدد المستندات للمعالجة.


**Returns:**
int - إجمالي عدد المستندات للمعالجة.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


يحصل على عدد المستندات التي تمت معالجتها بنجاح.


**Returns:**
int - عدد المستندات التي تمت معالجتها بنجاح.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


يحصل على عدد المستندات المتخطاة.


**Returns:**
int - عدد المستندات المتخطاة.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


يحصل على نسبة التقدم.


**Returns:**
double - نسبة التقدم.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


يحصل على مفتاح آخر مستند تمت معالجته.


**Returns:**
java.lang.String - مفتاح آخر مستند تمت معالجته.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


يحصل على مسار آخر مستند تمت معالجته.


**Returns:**
java.lang.String - مسار آخر مستند تمت معالجته.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


يحصل على حالة آخر مستند تمت معالجته.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

