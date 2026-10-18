---
title: "IndexingReport"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 작업에 대한 자세한 정보를 나타냅니다."
type: docs
weight: 25
url: /ko/java/com.groupdocs.search.common/indexingreport/
---
**Inheritance:**
java.lang.Object
```
public abstract class IndexingReport
```

인덱싱 작업에 대한 자세한 정보를 나타냅니다.


**Learn more**

* [Indexing reports](../https://docs.groupdocs.com/display/searchjava/Indexing+reports)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 문서 인덱싱
index.add(documentsFolder1);
index.add(documentsFolder2);
// 인덱싱 보고서 가져오기
IndexingReport[] reports = index.getIndexingReports();
// 콘솔에 보고서 출력
for (IndexingReport report : reports) {
DateFormat df = new SimpleDateFormat("MM/dd/yyyy HH:mm:ss");
System.out.println("Time: " + df.format(report.getStartTime()));
System.out.println("Duration: " + report.getIndexingTime());
System.out.println("Documents total: " + report.getTotalDocumentsInIndex());
System.out.println("Terms total: " + report.getTotalTermCount());
System.out.println("Indexed documents size (MB): " + report.getIndexedDocumentsSize());
System.out.println("Index size (MB): " + (report.getTotalIndexSize() / 1024.0 / 1024.0));
System.out.println();
}
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
| [IndexingReport()](#IndexingReport--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getTotalDocumentsInIndex()](#getTotalDocumentsInIndex--) | 인덱스에 있는 문서 총 수를 가져옵니다. |
|
|  | [getTotalTermCount()](#getTotalTermCount--) | 인덱스에 있는 용어 총 수를 가져옵니다. |
|
|  | [getIndexedDocumentsSize()](#getIndexedDocumentsSize--) | 인덱싱된 문서의 총 길이를 MB 단위로 가져옵니다. |
|
|  | [getSegmentCount()](#getSegmentCount--) | 인덱스 세그먼트 수를 가져옵니다. |
|
|  | [getTotalIndexSize()](#getTotalIndexSize--) | 인덱스의 전체 크기를 바이트 단위로 가져옵니다. |
|
|  | [getStartTime()](#getStartTime--) | 인덱싱 시작 시간을 가져옵니다. |
|
|  | [getEndTime()](#getEndTime--) | 인덱싱 종료 시간을 가져옵니다. |
|
|  | [getIndexingTime()](#getIndexingTime--) | 인덱싱 지속 시간을 초 단위로 가져옵니다. |
|
|  | [getErrors()](#getErrors--) | 오류 목록을 가져옵니다. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | 인덱싱된 문서 목록을 가져옵니다. |
|
|  | [getUpdatedDocuments()](#getUpdatedDocuments--) | 업데이트된 문서 목록을 가져옵니다. |
|
|  | [getRemovedDocuments()](#getRemovedDocuments--) | 인덱스에서 제거된 문서 목록을 가져옵니다. |
|
### IndexingReport() {#IndexingReport--}
```
public IndexingReport()
```


### getTotalDocumentsInIndex() {#getTotalDocumentsInIndex--}
```
public abstract int getTotalDocumentsInIndex()
```


인덱스에 있는 문서 총 수를 가져옵니다.


**Returns:**
int - 인덱스에 있는 문서의 총 수.

### getTotalTermCount() {#getTotalTermCount--}
```
public abstract int getTotalTermCount()
```


인덱스에 있는 용어 총 수를 가져옵니다.


**Returns:**
int - 인덱스의 전체 용어 수.

### getIndexedDocumentsSize() {#getIndexedDocumentsSize--}
```
public abstract double getIndexedDocumentsSize()
```


인덱싱된 문서의 총 길이를 MB 단위로 가져옵니다.


**Returns:**
double - 인덱싱된 문서의 총 길이(MB).

### getSegmentCount() {#getSegmentCount--}
```
public abstract int getSegmentCount()
```


인덱스 세그먼트 수를 가져옵니다.


**Returns:**
int - 인덱스 세그먼트 수.

### getTotalIndexSize() {#getTotalIndexSize--}
```
public abstract long getTotalIndexSize()
```


인덱스의 전체 크기를 바이트 단위로 가져옵니다.


**Returns:**
long - 전체 인덱스 크기(바이트).

### getStartTime() {#getStartTime--}
```
public abstract Date getStartTime()
```


인덱싱 시작 시간을 가져옵니다.


**Returns:**
java.util.Date - 인덱싱 시작 시간.

### getEndTime() {#getEndTime--}
```
public abstract Date getEndTime()
```


인덱싱 종료 시간을 가져옵니다.


**Returns:**
java.util.Date - 인덱싱 종료 시간.

### getIndexingTime() {#getIndexingTime--}
```
public abstract double getIndexingTime()
```


인덱싱 지속 시간을 초 단위로 가져옵니다.


**Returns:**
double - 인덱싱 지속 시간(초).

### getErrors() {#getErrors--}
```
public abstract String[] getErrors()
```


오류 목록을 가져옵니다.


**Returns:**
java.lang.String[] - 오류 목록.

### getIndexedDocuments() {#getIndexedDocuments--}
```
public abstract String[] getIndexedDocuments()
```


인덱싱된 문서 목록을 가져옵니다.


**Returns:**
java.lang.String[] - 인덱싱된 문서 목록.

### getUpdatedDocuments() {#getUpdatedDocuments--}
```
public abstract String[] getUpdatedDocuments()
```


업데이트된 문서 목록을 가져옵니다.


**Returns:**
java.lang.String[] - 업데이트된 문서 목록.

### getRemovedDocuments() {#getRemovedDocuments--}
```
public abstract String[] getRemovedDocuments()
```


인덱스에서 제거된 문서 목록을 가져옵니다.


**Returns:**
java.lang.String[] - 인덱스에서 제거된 문서 목록.

