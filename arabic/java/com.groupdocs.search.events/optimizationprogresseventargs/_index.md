---
title: "OptimizationProgressEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث تحديث تقدم عملية الفهرسة."
type: docs
weight: 19
url: /ar/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

يمثل المعلمات لحدث تحديث تقدم عملية الفهرسة.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | يحصل على إجمالي عدد المقاطع للمعالجة. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | يحصل على عدد المقاطع المعالجة. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | يحصل على نسبة التقدم. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


يحصل على إجمالي عدد المقاطع للمعالجة.


**Returns:**
int - إجمالي عدد المقاطع للمعالجة.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


يحصل على عدد المقاطع المعالجة.


**Returns:**
int - عدد المقاطع المعالجة.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


يحصل على نسبة التقدم.


**Returns:**
double - نسبة التقدم.

