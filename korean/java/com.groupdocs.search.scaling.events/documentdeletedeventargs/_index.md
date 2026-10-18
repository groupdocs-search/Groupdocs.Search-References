---
title: "DocumentDeletedEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 삭제가 완료되는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.scaling.events/documentdeletedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentDeletedEventArgs extends EventArgs
```

문서 삭제가 완료되는 이벤트에 대한 인수를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | 샤드 인덱스를 가져옵니다. |
|
|  | [getDocumentKey()](#getDocumentKey--) | 문서 키를 가져옵니다. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


샤드 인덱스를 가져옵니다.


**Returns:**
int - 샤드 인덱스.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


문서 키를 가져옵니다.


**Returns:**
java.lang.String - 문서 키.

