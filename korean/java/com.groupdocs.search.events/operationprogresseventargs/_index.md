---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 작업 진행률이 업데이트되는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

인덱싱 작업 진행률이 업데이트되는 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | 처리할 전체 문서 수를 가져옵니다. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | 성공적으로 처리된 문서 수를 가져옵니다. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | 건너뛴 문서 수를 가져옵니다. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | 진행률의 백분율을 가져옵니다. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | 마지막으로 처리된 문서의 키를 가져옵니다. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | 마지막으로 처리된 문서의 경로를 가져옵니다. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | 마지막으로 처리된 문서의 상태를 가져옵니다. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


처리할 전체 문서 수를 가져옵니다.


**Returns:**
int - 처리할 전체 문서 수.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


성공적으로 처리된 문서 수를 가져옵니다.


**Returns:**
int - 성공적으로 처리된 문서 수.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


건너뛴 문서 수를 가져옵니다.


**Returns:**
int - 건너뛴 문서 수.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


진행률의 백분율을 가져옵니다.


**Returns:**
double - 진행률의 백분율.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


마지막으로 처리된 문서의 키를 가져옵니다.


**Returns:**
java.lang.String - 마지막으로 처리된 문서 키.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


마지막으로 처리된 문서의 경로를 가져옵니다.


**Returns:**
java.lang.String - 마지막으로 처리된 문서 경로.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


마지막으로 처리된 문서의 상태를 가져옵니다.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

