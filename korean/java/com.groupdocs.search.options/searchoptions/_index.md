---
title: "SearchOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 작업에 대한 옵션을 제공합니다."
type: docs
weight: 34
url: /ko/java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

검색 작업에 대한 옵션을 제공합니다.


**Learn more**

* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [SearchOptions()](#SearchOptions--) | SearchOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SearchOptions(Object data)](#SearchOptions-java.lang.Object-) | SearchOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getUseSynonymSearch()](#getUseSynonymSearch--) | 검색에서 동의어 사용 플래그를 가져옵니다. |
|
|  | [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | 검색에서 동의어 사용 플래그를 설정합니다. |
|
|  | [getUseHomophoneSearch()](#getUseHomophoneSearch--) | 검색에서 동음이의어 사용 플래그를 가져옵니다. |
|
|  | [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | 검색에서 동음이의어 사용 플래그를 설정합니다. |
|
|  | [getUseWordFormsSearch()](#getUseWordFormsSearch--) | 검색에서 다른 형태의 단어 사용 플래그를 가져옵니다. |
|
|  | [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | 검색에서 다른 형태의 단어 사용 플래그를 설정합니다. |
|
|  | [getRetrieveAttributes()](#getRetrieveAttributes--) | 찾은 문서와 연관된 속성 검색 플래그를 가져옵니다. |
|
|  | [setRetrieveAttributes(boolean value)](#setRetrieveAttributes-boolean-) | 검색된 문서와 연관된 속성을 검색하는 플래그를 설정합니다. |
|
|  | [getFuzzySearch()](#getFuzzySearch--) | 퍼지 검색 옵션을 가져옵니다. |
|
|  | [getSpellingCorrector()](#getSpellingCorrector--) | 맞춤법 교정 옵션을 가져옵니다. |
|
|  | [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | 키보드 레이아웃 교정 옵션을 가져옵니다. |
|
|  | [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | 대소문자 구분 검색 플래그를 가져옵니다. |
|
|  | [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | 대소문자 구분 검색 플래그를 설정합니다. |
|
|  | [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | 검색 쿼리에서 모든 용어의 전체 최대 발생 횟수를 가져옵니다. |
|
|  | [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | 검색 쿼리에서 모든 용어의 전체 최대 발생 횟수를 설정합니다. |
|
|  | [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | 검색 쿼리에서 각 용어의 최대 발생 횟수를 가져옵니다. |
|
|  | [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | 검색 쿼리에서 각 용어의 최대 발생 횟수를 설정합니다. |
|
|  | [getDateFormats()](#getDateFormats--) | 날짜 범위 검색을 위한 날짜 형식 컬렉션을 가져옵니다. |
|
|  | [isChunkSearch()](#isChunkSearch--) | 청크별 검색 플래그를 가져옵니다. |
|
|  | [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | 청크별 검색 플래그를 설정합니다. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | 검색 문서 필터를 가져옵니다. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | 검색 문서 필터를 설정합니다. |
|
|  | [getCancellation()](#getCancellation--) | 작업 취소 객체를 가져옵니다. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 작업 취소 객체를 설정합니다. |
|
| [getCore()](#getCore--) |  |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


SearchOptions 클래스의 새 인스턴스를 초기화합니다.


### SearchOptions(Object data) {#SearchOptions-java.lang.Object-}
```
public SearchOptions(Object data)
```


SearchOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public boolean getUseSynonymSearch()
```


검색에서 동의어 사용 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 검색에서 동의어 사용 플래그.

### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public void setUseSynonymSearch(boolean value)
```


검색에서 동의어 사용 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 검색에서 동의어 사용 플래그. |
|

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public boolean getUseHomophoneSearch()
```


검색에서 동음이의어 사용 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 검색에서 동음이의어 사용 플래그.

### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public void setUseHomophoneSearch(boolean value)
```


검색에서 동음이의어 사용 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 검색에서 동음이의어 사용 플래그. |
|

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public boolean getUseWordFormsSearch()
```


검색에서 다른 형태의 단어 사용 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 검색에서 다른 형태의 단어 사용 플래그.

### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public void setUseWordFormsSearch(boolean value)
```


검색에서 다른 형태의 단어 사용 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 검색에서 다른 형태의 단어를 사용하도록 하는 플래그. |
|

### getRetrieveAttributes() {#getRetrieveAttributes--}
```
public boolean getRetrieveAttributes()
```


검색된 문서와 연관된 속성을 검색하는 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 검색된 문서와 연관된 속성을 검색하는 플래그.

### setRetrieveAttributes(boolean value) {#setRetrieveAttributes-boolean-}
```
public void setRetrieveAttributes(boolean value)
```


검색된 문서와 연관된 속성을 검색하는 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 검색된 문서와 연관된 속성을 검색하는 플래그. |
|

### getFuzzySearch() {#getFuzzySearch--}
```
public FuzzySearchOptions getFuzzySearch()
```


퍼지 검색 옵션을 가져옵니다.


**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.

### getSpellingCorrector() {#getSpellingCorrector--}
```
public SpellingCorrectorOptions getSpellingCorrector()
```


맞춤법 교정 옵션을 가져옵니다.


**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.

### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


키보드 레이아웃 교정 옵션을 가져옵니다.


**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.

### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public boolean getUseCaseSensitiveSearch()
```


대소문자 구분 검색 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 대소문자 구분 검색 플래그.

### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public void setUseCaseSensitiveSearch(boolean value)
```


대소문자 구분 검색 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 대소문자 구분 검색 플래그. |
|

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public int getMaxTotalOccurrenceCount()
```


검색 쿼리에서 모든 용어의 총 최대 발생 횟수를 가져옵니다. 기본값은 500000입니다.


**Returns:**
int - 총 최대 발생 횟수.

### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public void setMaxTotalOccurrenceCount(int value)
```


검색 쿼리에서 모든 용어의 총 최대 발생 횟수를 설정합니다. 기본값은 500000입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 총 최대 발생 횟수. |
|

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public int getMaxOccurrenceCountPerTerm()
```


검색 쿼리에서 각 용어의 최대 발생 횟수를 가져옵니다. 기본값은 100000입니다.


**Returns:**
int - 검색 쿼리에서 각 용어의 최대 발생 횟수.

### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public void setMaxOccurrenceCountPerTerm(int value)
```


검색 쿼리에서 각 용어의 최대 발생 횟수를 설정합니다. 기본값은 100000입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 검색 쿼리에서 각 용어의 최대 발생 횟수. |
|

### getDateFormats() {#getDateFormats--}
```
public DateFormatCollection getDateFormats()
```


날짜 범위 검색을 위한 날짜 형식 컬렉션을 가져옵니다. 기본 날짜 형식은 'dd.MM.yyyy', 'MM/dd/yyyy', 'yyyy-MM-dd'입니다.


**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.


예제에서는 검색을 위한 날짜 형식을 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스를 생성합니다.
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.getDateFormats().clear(); // 기본 날짜 형식 제거
DateFormatElement[] elements = new DateFormatElement[] {
DateFormatElement.getMonthTwoDigits(),
DateFormatElement.getDayOfMonthTwoDigits(),
DateFormatElement.getYearFourDigits(),
};
// 날짜 형식 패턴 'MM/dd/yyyy' 생성
com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
options.getDateFormats().addItem(dateFormat);
SearchResult result = index.search(query, options); // 인덱스에서 검색
 
```
 
````


### isChunkSearch() {#isChunkSearch--}
```
public boolean isChunkSearch()
```


청크 단위 검색 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 청크 단위 검색 플래그.

### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public void setChunkSearch(boolean value)
```


청크 단위 검색 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 청크 단위 검색 플래그. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


검색 문서 필터를 가져옵니다. SearchDocumentFilter는 포함 로직으로 작동합니다. 검색 문서 필터 인스턴스를 만들려면 SearchDocumentFilter 클래스를 사용하십시오. 기본값은 null이며, 이는 모든 검색된 문서가 반환됨을 의미합니다.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.


예제는 문서 필터를 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 문서 인덱싱
index.add(documentsFolder);
// 확장자 '.doc', '.docx', '.rtf'를 가진 문서를 건너뛰는 검색 문서 필터 생성
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // 파일 확장자 필터 생성
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // 파일 확장자 필터 반전
options.setSearchDocumentFilter(invertedFilter);
// 인덱스에서 검색
SearchResult result = index.search("Einstein", options);
 
```
 
````


### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


검색 문서 필터를 설정합니다.  SearchDocumentFilter  는 포함 논리에서 작동합니다. 검색 문서 필터 인스턴스를 생성하려면  SearchDocumentFilter  클래스를 사용하십시오. 기본값은  null  로, 이는 모든 검색된 문서가 반환됨을 의미합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | 검색 문서 필터. |


예제는 문서 필터를 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments1\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 문서 인덱싱
index.add(documentsFolder);
// 확장자 '.doc', '.docx', '.rtf'를 가진 문서를 건너뛰는 검색 문서 필터 생성
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // 파일 확장자 필터 생성
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // 파일 확장자 필터 반전
options.setSearchDocumentFilter(invertedFilter);
// 인덱스에서 검색
SearchResult result = index.search("Einstein", options);
 
```
 
````

|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


작업 취소 객체를 가져옵니다. 기본값은 null입니다.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


작업 취소 객체를 설정합니다. 기본값은 null입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 작업 취소 객체. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
