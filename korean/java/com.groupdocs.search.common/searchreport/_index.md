---
title: "SearchReport"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 작업에 대한 자세한 정보를 나타냅니다."
type: docs
weight: 30
url: /ko/java/com.groupdocs.search.common/searchreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchReport
```

검색 작업에 대한 자세한 정보를 나타냅니다.


**Learn more**

* [Search reports](../https://docs.groupdocs.com/display/searchjava/Search+reports)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 인덱스에서 검색 중
SearchResult result1 = index.search("Einstein");
SearchResult result2 = index.search("\"Theory of Relativity\"");
// 검색 보고서 가져오기
SearchReport[] reports = index.getSearchReports();
// 콘솔에 보고서 출력
for (SearchReport report : reports) {
System.out.println("쿼리: " + report.getTextQuery());
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("소요 시간: " + report.getSearchDuration());
System.out.println("문서 수: " + report.getDocumentCount());
System.out.println("발생 횟수: " + report.getOccurrenceCount());
System.out.println();
}
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SearchReport()](#SearchReport--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getStartTime()](#getStartTime--) | 검색 시작 시간을 가져옵니다. |
|
|  | [getEndTime()](#getEndTime--) | 검색 종료 시간을 가져옵니다. |
|
|  | [getSearchDuration()](#getSearchDuration--) | 검색 소요 시간을 초 단위로 가져옵니다. |
|
|  | [getDocumentCount()](#getDocumentCount--) | 검색된 문서 수를 가져옵니다. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 검색된 전체 발생 횟수를 가져옵니다. |
|
|  | [getTextQuery()](#getTextQuery--) | 텍스트 형태의 검색 쿼리를 가져옵니다. |
|
|  | [getObjectQuery()](#getObjectQuery--) | 객체 형태의 검색 쿼리를 가져옵니다. |
|
|  | [getSearchOptions()](#getSearchOptions--) | 검색 옵션을 가져옵니다. |
|
|  | [toString()](#toString--) | 현재 SearchReport를 나타내는 문자열을 반환합니다. |
|
### SearchReport() {#SearchReport--}
```
public SearchReport()
```


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

### getTextQuery() {#getTextQuery--}
```
public abstract String getTextQuery()
```


텍스트 형태의 검색 쿼리를 가져옵니다.


**Returns:**
java.lang.String - 텍스트 형태의 검색 쿼리.

### getObjectQuery() {#getObjectQuery--}
```
public abstract SearchQuery getObjectQuery()
```


객체 형태의 검색 쿼리를 가져옵니다.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The search query in object form.

### getSearchOptions() {#getSearchOptions--}
```
public abstract SearchOptions getSearchOptions()
```


검색 옵션을 가져옵니다.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### toString() {#toString--}
```
public abstract String toString()
```


현재 SearchReport를 나타내는 문자열을 반환합니다.


**Returns:**
java.lang.String - 현재 SearchReport를 나타내는 문자열.

