---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스 오류가 발생한 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.search.events/indexerroreventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class IndexErrorEventArgs extends BaseIndexEventArgs
```

인덱스 오류가 발생한 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getMessage()](#getMessage--) | 오류 메시지를 가져옵니다. |
|
|  | [isCritical()](#isCritical--) | 오류가 발생했으며 인덱스를 재시작해야 함을 나타내는 플래그를 가져옵니다. |
|
### getMessage() {#getMessage--}
```
public final String getMessage()
```


오류 메시지를 가져옵니다.


**Returns:**
java.lang.String - 오류 메시지.

### isCritical() {#isCritical--}
```
public final boolean isCritical()
```


오류가 발생했으며 인덱스를 재시작해야 함을 나타내는 플래그를 가져옵니다.


**Returns:**
boolean - 오류가 발생했으며 인덱스를 재시작해야 함을 나타내는 플래그.

