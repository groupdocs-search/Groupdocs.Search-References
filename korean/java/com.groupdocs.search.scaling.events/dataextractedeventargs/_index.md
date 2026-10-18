---
title: "DataExtractedEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 데이터 추출이 완료되는 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.scaling.events/dataextractedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DataExtractedEventArgs extends EventArgs
```

문서 데이터 추출이 완료되는 이벤트에 대한 인수를 나타냅니다.

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getExtractorIndex()](#getExtractorIndex--) | 추출기 인덱스를 가져옵니다. |
|
|  | [getDocumentKey()](#getDocumentKey--) | 문서 키를 가져옵니다. |
|
### getExtractorIndex() {#getExtractorIndex--}
```
public final int getExtractorIndex()
```


추출기 인덱스를 가져옵니다.


**Returns:**
int - 추출기 인덱스.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


문서 키를 가져옵니다.


**Returns:**
java.lang.String - 문서 키.

