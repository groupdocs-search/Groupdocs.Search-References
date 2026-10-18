---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 문서 필터를 생성하는 메서드를 포함합니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

검색 문서 필터를 생성하는 메서드를 포함합니다.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | 정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | 정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | 지정된 가능한 확장자 목록에 포함되지 않은 문서를 건너뛰기 위한 필터를 생성합니다. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | 지정된 내부 필터와 반대 논리를 갖는 필터를 생성합니다. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | 지정된 필터들의 논리적 AND를 생성합니다. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | 지정된 필터들의 논리적 OR를 생성합니다. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | 지정된 허용 속성 목록 중 값을 갖지 않는 문서를 건너뛰기 위한 필터를 생성합니다. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


정규 표현식과 일치하지 않는 문서를 건너뛰기 위한 필터를 생성합니다. 정규 표현식은 문서의 전체 경로에 적용됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pattern | java.lang.String | 정규 표현식 패턴. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
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
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


지정된 가능한 확장자 목록에 포함되지 않은 문서를 건너뛰기 위한 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | extensions | java.lang.String[] | 가능한 확장자의 목록. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


지정된 내부 필터와 반대 논리를 갖는 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 내부 검색 문서 필터. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


지정된 필터들의 논리적 AND를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | 검색 문서 필터들. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


지정된 필터들의 논리적 OR를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | 검색 문서 필터들. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


지정된 허용 속성 목록 중 값을 갖지 않는 문서를 건너뛰기 위한 필터를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 속성 | java.lang.String[] | 허용 가능한 속성의 목록. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

