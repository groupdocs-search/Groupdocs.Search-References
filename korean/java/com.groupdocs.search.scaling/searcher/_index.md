---
title: "Searcher"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크의 샤드에 대한 검색 쿼리를 관리하는 서비스를 나타냅니다."
type: docs
weight: 12
url: /ko/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

검색 네트워크의 샤드에 대한 검색 쿼리를 관리하는 서비스를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 분산 검색 인덱스에서 텍스트 형태의 쿼리로 검색을 시작합니다. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 분산 검색 인덱스에서 검색을 시작합니다. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | 분산 검색 인덱스에서 역 이미지 검색을 수행합니다. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | 분산 검색 인덱스에서 검색을 계속합니다. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | 분산 검색 인덱스에서 역 이미지 검색을 계속합니다. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | 검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | 전체 인덱싱된 문서 배열을 가져옵니다. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | 지정된 문서의 중첩 항목 배열을 가져옵니다 (ZIP, OST, PST와 같은 컨테이너 문서용). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | 인덱싱된 문서의 텍스트를 생성하고 출력 어댑터를 통해 전달합니다. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


분산 검색 인덱스에서 텍스트 형태의 쿼리로 검색을 시작합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | java.lang.String | 검색 쿼리. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


분산 검색 인덱스에서 검색을 시작합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 검색 쿼리. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


분산 검색 인덱스에서 역 이미지 검색을 수행합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | 검색할 이미지. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | 이미지 검색 옵션. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


분산 검색 인덱스에서 검색을 계속합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | 네트워크 검색 토큰. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


분산 검색 인덱스에서 역 이미지 검색을 계속합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | 네트워크 이미지 검색 토큰. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | 찾은 문서. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 검색 결과 하이라이터. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | 하이라이트 옵션입니다. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


전체 인덱싱된 문서 배열을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | shardIndex | int | 샤드 인덱스입니다. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - 모든 인덱싱된 문서의 배열.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


지정된 문서의 중첩 항목 배열을 가져옵니다 (ZIP, OST, PST와 같은 컨테이너 문서용).


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | 문서 정보. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - 문서 항목의 배열.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


인덱싱된 문서의 텍스트를 생성하고 출력 어댑터를 통해 전달합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | 인덱싱된 문서 정보입니다. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 출력 어댑터입니다. |
|

