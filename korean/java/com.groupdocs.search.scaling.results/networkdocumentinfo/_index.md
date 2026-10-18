---
title: "NetworkDocumentInfo"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크에서 인덱싱된 문서에 대한 설명자를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.scaling.results/networkdocumentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkDocumentInfo
```

검색 네트워크에서 인덱싱된 문서에 대한 설명자를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NetworkDocumentInfo()](#NetworkDocumentInfo--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | 인덱싱된 문서에 대한 설명자를 가져옵니다. |
|
|  | [getShardIndex()](#getShardIndex--) | 샤드 인덱스를 가져옵니다. |
|
### NetworkDocumentInfo() {#NetworkDocumentInfo--}
```
public NetworkDocumentInfo()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


인덱싱된 문서에 대한 설명자를 가져옵니다.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The descriptor for an indexed document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


샤드 인덱스를 가져옵니다.


**Returns:**
int - 샤드 인덱스.

