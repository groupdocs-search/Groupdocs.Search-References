---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크의 노드 중 하나에서 오류가 발생하는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

검색 네트워크의 노드 중 하나에서 오류가 발생하는 이벤트에 대한 인수를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | 검색 네트워크 노드의 인덱스를 가져옵니다. |
|
|  | [getServiceIndex()](#getServiceIndex--) | 검색 네트워크 노드 서비스의 인덱스를 가져옵니다. |
|
|  | [getMessage()](#getMessage--) | 오류 메시지를 가져옵니다. |
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

### getMessage() {#getMessage--}
```
public final String getMessage()
```


오류 메시지를 가져옵니다.


**Returns:**
java.lang.String - 오류 메시지.

