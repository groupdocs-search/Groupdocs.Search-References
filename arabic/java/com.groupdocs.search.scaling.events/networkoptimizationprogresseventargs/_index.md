---
title: "NetworkOptimizationProgressEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث تغيير تقدم عملية التحسين."
type: docs
weight: 15
url: /ar/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

يمثل المعلمات لحدث تغيير تقدم عملية التحسين.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | يحصل على فهرس عقدة شبكة البحث. |
|
|  | [getServiceIndex()](#getServiceIndex--) | يحصل على فهرس خدمة عقدة شبكة البحث. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | يحصل على عدد المقاطع المعالجة. |
|
|  | [getTotalSegments()](#getTotalSegments--) | يحصل على إجمالي عدد المقاطع للمعالجة. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


يحصل على عدد المقاطع المعالجة.


**Returns:**
int - عدد المقاطع المعالجة.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


يحصل على إجمالي عدد المقاطع للمعالجة.


**Returns:**
int - إجمالي عدد المقاطع للمعالجة.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


يحصل على نسبة التقدم.


**Returns:**
double - نسبة التقدم.

