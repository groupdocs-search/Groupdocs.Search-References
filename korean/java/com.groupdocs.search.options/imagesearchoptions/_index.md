---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "역 이미지 검색 작업에 대한 옵션을 제공합니다."
type: docs
weight: 24
url: /ko/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

역 이미지 검색 작업에 대한 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | ImageSearchOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | ImageSearchOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | 이미지 해시에서 일치하지 않는 비트의 최대 개수를 가져옵니다. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | 이미지 해시에서 일치하지 않는 비트의 최대 개수를 설정합니다. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | 이미지 역검색 요청에 대해 찾은 이미지의 최대 개수를 가져옵니다. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | 이미지 역검색 요청에 대해 찾은 이미지의 최대 개수를 설정합니다. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | 검색 문서 필터를 가져옵니다. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | 검색 문서 필터를 가져오거나 설정합니다. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


ImageSearchOptions 클래스의 새 인스턴스를 초기화합니다.


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


ImageSearchOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


이미지 해시에서 일치하지 않는 비트의 최대 개수를 가져옵니다. 기본값은 5입니다.


**Returns:**
int - 이미지 해시에서 일치하지 않는 비트의 최대 개수.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


이미지 해시에서 일치하지 않는 비트의 최대 개수를 설정합니다. 기본값은 5입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 이미지 해시에서 일치하지 않는 비트의 최대 개수. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


이미지 역검색 요청에 대해 찾은 이미지의 최대 개수를 가져옵니다. 기본값은 1000입니다.


**Returns:**
int - 이미지 역검색 요청에 대해 찾은 이미지의 최대 개수.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


이미지 역검색 요청에 대해 찾은 이미지의 최대 개수를 설정합니다. 기본값은 1000입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 이미지 역검색 요청에 대해 찾은 이미지의 최대 개수. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


검색 문서 필터를 가져옵니다. SearchDocumentFilter는 포함 논리로 작동합니다. 검색 문서 필터 인스턴스를 만들려면 GroupDocs.Search.Options.SearchDocumentFilter 클래스를 사용하십시오. 기본값은 null이며, 이는 모든 찾은 문서가 반환됨을 의미합니다.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


검색 문서 필터를 가져오거나 설정합니다. SearchDocumentFilter는 포함 논리로 작동합니다. 검색 문서 필터 인스턴스를 만들려면 GroupDocs.Search.Options.SearchDocumentFilter 클래스를 사용하십시오. 기본값은 null이며, 이는 모든 찾은 문서가 반환됨을 의미합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 검색 문서 필터. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
