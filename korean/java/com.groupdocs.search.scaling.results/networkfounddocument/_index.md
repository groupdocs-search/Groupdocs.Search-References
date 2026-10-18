---
title: "NetworkFoundDocument"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크에서 발견된 문서를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.scaling.results/networkfounddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkFoundDocument
```

검색 네트워크에서 발견된 문서를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NetworkFoundDocument()](#NetworkFoundDocument--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFoundDocument()](#getFoundDocument--) | 찾은 문서를 가져옵니다. |
|
|  | [getShardIndex()](#getShardIndex--) | 샤드 인덱스를 가져옵니다. |
|
### NetworkFoundDocument() {#NetworkFoundDocument--}
```
public NetworkFoundDocument()
```


### getFoundDocument() {#getFoundDocument--}
```
public abstract FoundDocument getFoundDocument()
```


찾은 문서를 가져옵니다.


**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


샤드 인덱스를 가져옵니다.


**Returns:**
int - 샤드 인덱스.

