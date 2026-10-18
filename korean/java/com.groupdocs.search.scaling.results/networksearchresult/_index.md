---
title: "NetworkSearchResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 쿼리와 일치하는 검색 결과를 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.scaling.results/networksearchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class NetworkSearchResult implements Iterable<NetworkFoundDocument>
```

검색 쿼리와 일치하는 검색 결과를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NetworkSearchResult()](#NetworkSearchResult--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentCount()](#getDocumentCount--) | 검색된 문서 수를 가져옵니다. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 검색된 전체 발생 횟수를 가져옵니다. |
|
|  | [getTruncated()](#getTruncated--) | 결과가 잘렸음을 나타내는 값을 가져옵니다. |
|
|  | [getWarnings()](#getWarnings--) | 결과를 설명하는 경고를 가져옵니다. |
|
|  | [getStartTime()](#getStartTime--) | 검색 시작 시간을 가져옵니다. |
|
|  | [getEndTime()](#getEndTime--) | 검색 종료 시간을 가져옵니다. |
|
|  | [getSearchDuration()](#getSearchDuration--) | 검색 소요 시간을 초 단위로 가져옵니다. |
|
|  | [getFoundDocument(int index)](#getFoundDocument-int-) | 인덱스로 검색된 문서를 가져옵니다. |
|
|  | [iterator()](#iterator--) | 검색된 문서 컬렉션을 순회하는 반복자를 반환합니다. |
|
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | 다음 청크를 검색하기 위한 청크 검색 토큰을 가져옵니다. |
|
|  | [getNodeIndex()](#getNodeIndex--) | 결과를 받은 노드의 인덱스를 가져옵니다. |
|
### NetworkSearchResult() {#NetworkSearchResult--}
```
public NetworkSearchResult()
```


### getDocumentCount() {#getDocumentCount--}
```
public abstract int getDocumentCount()
```


검색된 문서 수를 가져옵니다.


**Returns:**
int - 검색된 문서 수.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


검색된 전체 발생 횟수를 가져옵니다.


**Returns:**
int - 검색된 전체 발생 횟수.

### getTruncated() {#getTruncated--}
```
public abstract boolean getTruncated()
```


결과가 잘렸음을 나타내는 값을 가져옵니다.


**Returns:**
boolean - 결과가 잘렸음을 나타내는 값.

### getWarnings() {#getWarnings--}
```
public abstract String getWarnings()
```


결과를 설명하는 경고를 가져옵니다.


**Returns:**
java.lang.String - 결과를 설명하는 경고.

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


검색 시작 시간을 가져옵니다.


**Returns:**
java.util.Date - 검색 시작 시간.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


검색 종료 시간을 가져옵니다.


**Returns:**
java.util.Date - 검색 종료 시간.

### getSearchDuration() {#getSearchDuration--}
```
public abstract double getSearchDuration()
```


검색 소요 시간을 초 단위로 가져옵니다.


**Returns:**
double - 검색 소요 시간(초).

### getFoundDocument(int index) {#getFoundDocument-int-}
```
public abstract NetworkFoundDocument getFoundDocument(int index)
```


인덱스로 검색된 문서를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 검색된 문서의 인덱스. |
|

**Returns:**
[NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<NetworkFoundDocument> iterator()
```


검색된 문서 컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<com.groupdocs.search.scaling.results.NetworkFoundDocument> - 검색된 문서 컬렉션을 순회하는 데 사용할 수 있는 반복자.

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract NetworkSearchToken getNextChunkSearchToken()
```


다음 청크를 검색하기 위한 청크 검색 토큰을 가져옵니다.


**Returns:**
[NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) - A chunk search token for searching the next chunk.

### getNodeIndex() {#getNodeIndex--}
```
public abstract int getNodeIndex()
```


결과를 받은 노드의 인덱스를 가져옵니다.


**Returns:**
int - 결과를 받은 노드의 인덱스.

