---
title: "NetworkImageSearchResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 이미지와 일치하는 이미지 검색 결과를 나타냅니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.search.scaling.results/networkimagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class NetworkImageSearchResult
```

검색 이미지와 일치하는 이미지 검색 결과를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NetworkImageSearchResult()](#NetworkImageSearchResult--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | 검색된 이미지 수를 가져옵니다. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | 인덱스로 검색된 이미지를 가져옵니다. |
|
|  | [getNetworkImageSearchToken()](#getNetworkImageSearchToken--) | 다음 청크를 검색하기 위한 청크 이미지 검색 토큰을 가져옵니다. |
|
|  | [getNodeIndex()](#getNodeIndex--) | 결과를 받은 노드의 인덱스를 가져옵니다. |
|
|  | [getShardIndex()](#getShardIndex--) | 결과를 받은 샤드의 인덱스를 가져옵니다. |
|
### NetworkImageSearchResult() {#NetworkImageSearchResult--}
```
public NetworkImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


검색된 이미지 수를 가져옵니다.


**Returns:**
int - 검색된 이미지 수.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


인덱스로 검색된 이미지를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 검색된 이미지의 인덱스. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

### getNetworkImageSearchToken() {#getNetworkImageSearchToken--}
```
public abstract NetworkImageSearchToken getNetworkImageSearchToken()
```


다음 청크를 검색하기 위한 청크 이미지 검색 토큰을 가져옵니다.


**Returns:**
[NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) - A chunk image search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


결과를 받은 노드의 인덱스를 가져옵니다.


**Returns:**
int - 결과를 받은 노드의 인덱스.

### getShardIndex() {#getShardIndex--}
```
public abstract int getShardIndex()
```


결과를 받은 샤드의 인덱스를 가져옵니다.


**Returns:**
int - 결과를 받은 샤드의 인덱스.

