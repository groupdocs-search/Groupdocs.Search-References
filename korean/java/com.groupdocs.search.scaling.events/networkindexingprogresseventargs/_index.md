---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 작업의 진행률 변경 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

인덱싱 작업의 진행률 변경 이벤트에 대한 인수를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 검색 네트워크 노드의 인덱스를 가져옵니다. |
|
|  | [getServiceIndex()](#getServiceIndex--) | 검색 네트워크 노드 서비스의 인덱스를 가져옵니다. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | 처리된 문서 수를 가져옵니다. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | 처리할 전체 문서 수를 가져옵니다. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 진행률의 백분율을 가져옵니다. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


검색 네트워크 노드의 인덱스를 가져옵니다.


**Returns:**
int - 검색 네트워크 노드의 인덱스.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


검색 네트워크 노드 서비스의 인덱스를 가져옵니다.


**Returns:**
int - 검색 네트워크 노드 서비스의 인덱스.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


처리된 문서 수를 가져옵니다.


**Returns:**
int - 처리된 문서 수.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


처리할 전체 문서 수를 가져옵니다.


**Returns:**
int - 처리할 전체 문서 수.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


진행률의 백분율을 가져옵니다.


**Returns:**
double - 진행률의 백분율.

