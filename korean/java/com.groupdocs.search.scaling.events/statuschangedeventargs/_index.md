---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크 상태 변경 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

검색 네트워크 상태 변경 이벤트에 대한 인수를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | 이전 검색 네트워크 상태를 가져옵니다. |
|
|  | [getNewStatus()](#getNewStatus--) | 새 검색 네트워크 상태를 가져옵니다. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


이전 검색 네트워크 상태를 가져옵니다.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


새 검색 네트워크 상태를 가져옵니다.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

