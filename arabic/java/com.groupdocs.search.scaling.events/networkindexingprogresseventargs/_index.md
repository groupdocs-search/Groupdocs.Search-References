---
title: "NetworkIndexingProgressEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث تغيير تقدم عملية الفهرسة."
type: docs
weight: 14
url: /ar/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

يمثل المعلمات لحدث تغيير تقدم عملية الفهرسة.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | يحصل على فهرس عقدة شبكة البحث. |
|
|  | [getServiceIndex()](#getServiceIndex--) | يحصل على فهرس خدمة عقدة شبكة البحث. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | يحصل على عدد المستندات التي تم معالجتها. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | يحصل على إجمالي عدد المستندات للمعالجة. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | يحصل على نسبة التقدم. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


يحصل على فهرس عقدة شبكة البحث.


**Returns:**
int - فهرس عقدة شبكة البحث.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


يحصل على فهرس خدمة عقدة شبكة البحث.


**Returns:**
int - فهرس خدمة عقدة شبكة البحث.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


يحصل على عدد المستندات التي تم معالجتها.


**Returns:**
int - عدد المستندات التي تم معالجتها.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


يحصل على إجمالي عدد المستندات للمعالجة.


**Returns:**
int - إجمالي عدد المستندات للمعالجة.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


يحصل على نسبة التقدم.


**Returns:**
double - نسبة التقدم.

