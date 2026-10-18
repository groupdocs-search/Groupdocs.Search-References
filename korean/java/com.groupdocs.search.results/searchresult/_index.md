---
title: "SearchResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 쿼리와 일치하는 검색 결과를 나타냅니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.search.results/searchresult/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class SearchResult implements Iterable<FoundDocument>
```

검색 쿼리와 일치하는 검색 결과를 나타냅니다.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentFolder);
// 검색 옵션 설정
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 퍼지 검색 활성화
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // 최대 차이 수를 3으로 설정
// 'Einstein' 단어 또는 'Theory of Relativity' 구문이 포함된 문서를 검색
SearchResult result = index.search("Einstein OR \"Theory of Relativity\"", options);
// 결과 출력
System.out.println("Documents: " + result.getDocumentCount());
System.out.println("Total occurrences: " + result.getOccurrenceCount());
for (int i = 0; i < result.getDocumentCount(); i++) {
FoundDocument document = result.getFoundDocument(i);
System.out.println("\tDocument: " + document.getDocumentInfo().getFilePath());
System.out.println("\tOccurrences: " + document.getOccurrenceCount());
for (int j = 0; j < document.getFoundFields().length; j++) {
FoundDocumentField field = document.getFoundFields()[j];
System.out.println("\t\tField: " + field.getFieldName());
System.out.println("\t\t발생 횟수: " + document.getOccurrenceCount());
// 찾은 용어 출력
if (field.getTerms() != null) {
for (int k = 0; k < field.getTerms().length; k++) {
System.out.println("\t\t\t" + field.getTerms()[k] + " - " + field.getTermsOccurrences()[k]);
}
}
// 찾은 구문 출력
if (field.getTermSequences() != null) {
for (int k = 0; k < field.getTermSequences().length; k++) {
String[] terms = field.getTermSequences()[k];
String sequence = "";
for (int m = 0; m < terms.length; m++) {
sequence += terms[m] + " ";
}
System.out.println("\t\t\t" + sequence + " - " + field.getTermSequencesOccurrences()[k]);
}
}
}
}
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SearchResult()](#SearchResult--) |  |
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
|  | [getNextChunkSearchToken()](#getNextChunkSearchToken--) | 다음 청크를 검색하기 위한 청크 검색 토큰을 가져옵니다. |
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
### SearchResult() {#SearchResult--}
```
public SearchResult()
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

### getNextChunkSearchToken() {#getNextChunkSearchToken--}
```
public abstract ChunkSearchToken getNextChunkSearchToken()
```


다음 청크를 검색하기 위한 청크 검색 토큰을 가져옵니다.


**Returns:**
[ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) - A chunk search token for searching the next chunk.

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
public abstract FoundDocument getFoundDocument(int index)
```


인덱스로 검색된 문서를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 검색된 문서의 인덱스. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - The found document.

### iterator() {#iterator--}
```
public abstract Iterator<FoundDocument> iterator()
```


검색된 문서 컬렉션을 순회하는 반복자를 반환합니다.


**Returns:**
java.util.Iterator<com.groupdocs.search.results.FoundDocument> - 찾은 문서 컬렉션을 반복하는 데 사용할 수 있는 반복자.

