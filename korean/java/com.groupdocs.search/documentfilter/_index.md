---
title: "DocumentFilter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 필터의 기본 클래스를 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

문서 필터의 기본 클래스를 나타냅니다. 문서 필터 인스턴스를 생성하는 메서드를 포함합니다.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [toString()](#toString--) | 문서 필터의 문자열 표현을 반환합니다. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | 생성 날짜가 하한보다 이전인 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | 생성 날짜가 상한보다 이후인 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | 지정된 범위를 벗어난 생성 날짜를 가진 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | 수정 날짜가 하한보다 이전인 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | 수정 날짜가 상한보다 이후인 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | 지정된 범위를 벗어난 수정 날짜를 가진 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | 정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | 정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | 길이가 하한보다 짧은 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | 길이가 상한보다 긴 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | 지정된 문서 길이 범위를 벗어난 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | 허용된 확장자를 갖지 않은 문서를 건너뛰는 필터를 생성합니다. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | 지정된 내부 필터와 반대 논리를 갖는 필터를 생성합니다. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | 지정된 필터들의 논리적 AND를 생성합니다. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | 지정된 필터들의 논리적 OR를 생성합니다. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


문서 필터의 문자열 표현을 반환합니다.


**Returns:**
java.lang.String - 문서 필터의 문자열 표현.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


생성 날짜가 하한보다 이전인 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 문서 생성 시간의 하한. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


생성 날짜가 상한보다 이후인 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | upperBound | java.util.Date | 문서 생성 시간의 상한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


지정된 범위를 벗어난 생성 날짜를 가진 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 문서 생성 시간의 하한. |
|
|  | upperBound | java.util.Date | 문서 생성 시간의 상한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


수정 날짜가 하한보다 이전인 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 문서 수정 시간의 하한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


수정 날짜가 상한보다 이후인 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | upperBound | java.util.Date | 문서 수정 시간의 상한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


지정된 범위를 벗어난 수정 날짜를 가진 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | lowerBound | java.util.Date | 문서 수정 시간의 하한값. |
|
|  | upperBound | java.util.Date | 문서 수정 시간의 상한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. 정규 표현식은 문서의 전체 경로에 적용됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pattern | java.lang.String | 정규 표현식 패턴. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. 정규 표현식은 문서의 전체 경로에 적용됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pattern | java.lang.String | 정규 표현식 패턴. |
|
|  | options | int | 정규 표현식 옵션. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


길이가 하한보다 짧은 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | lowerBound | long | 문서 길이의 하한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


길이가 상한보다 긴 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | upperBound | long | 문서 길이의 상한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


지정된 문서 길이 범위를 벗어난 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | lowerBound | long | 문서 길이의 하한값. |
|
|  | upperBound | long | 문서 길이의 상한값. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


허용된 확장자를 갖지 않은 문서를 건너뛰는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | extensions | java.lang.String[] | 허용 가능한 확장자의 목록입니다. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


지정된 내부 필터와 반대 논리를 갖는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | 내부 문서 필터입니다. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


지정된 필터들의 논리적 AND를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | 문서 필터들입니다. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


지정된 필터들의 논리적 OR를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | 문서 필터들입니다. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

