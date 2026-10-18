---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이벤트 인수의 기본 클래스를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

이벤트 인수의 기본 클래스를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTime()](#getTime--) | 이벤트의 시간을 가져옵니다. |
|
|  | [getIndexId()](#getIndexId--) | 인덱스 ID를 가져옵니다. |
|
|  | [getIndexFolder()](#getIndexFolder--) | 인덱스 폴더를 가져옵니다. |
|
|  | [getStatus()](#getStatus--) | 인덱스 상태를 가져옵니다. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


이벤트의 시간을 가져옵니다.


**Returns:**
java.util.Date - 이벤트의 시간.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


인덱스 ID를 가져옵니다.


**Returns:**
java.util.UUID - 인덱스 ID.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


인덱스 폴더를 가져옵니다.


**Returns:**
java.lang.String - 인덱스 폴더.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


인덱스 상태를 가져옵니다.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

