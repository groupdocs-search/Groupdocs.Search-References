---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 작업 진행률이 업데이트되는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

인덱싱 작업 진행률이 업데이트되는 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | 처리할 전체 세그먼트 수를 가져옵니다. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | 처리된 세그먼트 수를 가져옵니다. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 진행률의 백분율을 가져옵니다. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


처리할 전체 세그먼트 수를 가져옵니다.


**Returns:**
int - 처리할 전체 세그먼트 수.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


처리된 세그먼트 수를 가져옵니다.


**Returns:**
int - 처리된 세그먼트 수.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


진행률의 백분율을 가져옵니다.


**Returns:**
double - 진행률의 백분율.

