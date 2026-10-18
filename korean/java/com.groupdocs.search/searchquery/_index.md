---
title: "SearchQuery"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "객체 형태의 검색 쿼리를 나타냅니다."
type: docs
weight: 25
url: /ko/java/com.groupdocs.search/searchquery/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchQuery
```

객체 형태의 검색 쿼리를 나타냅니다.


**Learn more**

* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)
* [Queries in text and object form](../https://docs.groupdocs.com/display/searchjava/Queries+in+text+and+object+form)
* [Nesting search queries in object form](../https://docs.groupdocs.com/display/searchjava/Nesting+search+queries+in+object+form)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
 
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
 
// 날짜 범위 검색의 하위 쿼리 생성
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 
// 누락된 단어 수가 0에서 2까지인 와일드카드 하위 쿼리 생성
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 
// 간단한 단어의 하위 쿼리 생성
SearchQuery subquery3 = SearchQuery.createWordQuery(\"birth\");
subquery3.setSearchOptions(new SearchOptions()); // 하위 쿼리 3에만 검색 옵션 설정
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 
// 여러 하위 쿼리를 하나의 쿼리로 결합
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 
// 발견된 발생 횟수 용량이 증가된 검색 옵션 객체 생성
SearchOptions options = new SearchOptions(); // 전체 검색 옵션
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
 
SearchResult result = index.search(query, options); // 검색 중
 
```
 
````


## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | 필드 이름을 가져옵니다. |
|
|  | [getChildCount()](#getChildCount--) | 하위 쿼리 수를 가져옵니다. |
|
|  | [getFirstChild()](#getFirstChild--) | 첫 번째 하위 쿼리를 가져옵니다. |
|
|  | [getSecondChild()](#getSecondChild--) | 두 번째 하위 쿼리를 가져옵니다. |
|
|  | [getChild(int index)](#getChild-int-) | 인덱스로 하위 쿼리를 가져옵니다. |
|
|  | [getSearchOptions()](#getSearchOptions--) | 이 seach 쿼리의 검색 옵션을 가져오거나 설정합니다. |
|
|  | [setSearchOptions(SearchOptions value)](#setSearchOptions-com.groupdocs.search.options.SearchOptions-) | 이 seach 쿼리의 검색 옵션을 가져오거나 설정합니다. |
|
|  | [toString()](#toString--) | 현재  SearchQuery  인스턴스를 나타내는  System.String  을 반환합니다. |
|
|  | [createWordQuery(String term)](#createWordQuery-java.lang.String-) | 간단한 단어 쿼리를 생성합니다. |
|
|  | [createWordPatternQuery(WordPattern pattern)](#createWordPatternQuery-com.groupdocs.search.common.WordPattern-) | 단어 패턴 쿼리를 생성합니다. |
|
|  | [createRegexQuery(String pattern)](#createRegexQuery-java.lang.String-) | 정규 표현식 쿼리를 생성합니다. |
|
|  | [createRegexQuery(String pattern, int options)](#createRegexQuery-java.lang.String-int-) | 정규 표현식 쿼리를 생성합니다. |
|
|  | [createNumericRangeQuery(long start, long end)](#createNumericRangeQuery-long-long-) | 숫자 범위 쿼리를 생성합니다. |
|
|  | [createDateRangeQuery(Date start, Date end)](#createDateRangeQuery-java.util.Date-java.util.Date-) | 날짜 범위 쿼리를 생성합니다. |
|
|  | [createPhraseSearchQuery(SearchQuery[] queries)](#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-) | 구문 검색 쿼리를 생성합니다. |
|
|  | [createAndQuery(SearchQuery[] queries)](#createAndQuery-com.groupdocs.search.SearchQuery---) | 각 원본 쿼리에 대해 찾을 수 있는 문서만 찾는 결합된 쿼리를 생성합니다. |
|
|  | [createFieldQuery(String fieldName, SearchQuery query)](#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-) | 지정된 쿼리에 필드를 추가합니다. |
|
|  | [createNotQuery(SearchQuery query)](#createNotQuery-com.groupdocs.search.SearchQuery-) | 원본 쿼리로 찾을 수 있는 문서를 제외하고 인덱스의 나머지 문서를 찾는 반전 쿼리를 생성합니다. |
|
|  | [createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | 각 원본 쿼리에 대해 찾을 수 있는 문서만 찾는 결합된 쿼리를 생성합니다. |
|
|  | [createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)](#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-) | 원본 쿼리 중 하나라도 찾을 수 있는 모든 문서를 찾는 결합된 쿼리를 생성합니다. |
|
|  | [createOrQuery(SearchQuery[] queries)](#createOrQuery-com.groupdocs.search.SearchQuery---) | 원본 쿼리 중 하나라도 찾을 수 있는 모든 문서를 찾는 결합된 쿼리를 생성합니다. |
|
|  | [createWildcardQuery(int count)](#createWildcardQuery-int-) | 구문 검색을 위한 와일드카드를 생성합니다. |
|
|  | [createWildcardQuery(int minCount, int maxCount)](#createWildcardQuery-int-int-) | 구문 검색을 위한 와일드카드를 생성합니다. |
|
### getFieldName() {#getFieldName--}
```
public String getFieldName()
```


필드 이름을 가져옵니다.


**Returns:**
java.lang.String - 필드 이름입니다.

### getChildCount() {#getChildCount--}
```
public int getChildCount()
```


하위 쿼리 수를 가져옵니다.


**Returns:**
int - 하위 쿼리 수입니다.

### getFirstChild() {#getFirstChild--}
```
public SearchQuery getFirstChild()
```


첫 번째 하위 쿼리를 가져옵니다.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The first child query.

### getSecondChild() {#getSecondChild--}
```
public SearchQuery getSecondChild()
```


두 번째 하위 쿼리를 가져옵니다.


**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - The second child query.

### getChild(int index) {#getChild-int-}
```
public abstract SearchQuery getChild(int index)
```


인덱스로 하위 쿼리를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 인덱스입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A child query corresponding the specified index.

### getSearchOptions() {#getSearchOptions--}
```
public final SearchOptions getSearchOptions()
```


이 seach 쿼리의 검색 옵션을 가져오거나 설정합니다.


**Returns:**
[SearchOptions](../../com.groupdocs.search.options/searchoptions) - The search options.

### setSearchOptions(SearchOptions value) {#setSearchOptions-com.groupdocs.search.options.SearchOptions-}
```
public final void setSearchOptions(SearchOptions value)
```


이 seach 쿼리의 검색 옵션을 가져오거나 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |
|

### toString() {#toString--}
```
public abstract String toString()
```


현재  SearchQuery  인스턴스를 나타내는  System.String  을 반환합니다.


**Returns:**
java.lang.String - 현재 SearchQuery 인스턴스를 나타내는 System.String입니다.

### createWordQuery(String term) {#createWordQuery-java.lang.String-}
```
public static SearchQuery createWordQuery(String term)
```


간단한 단어 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 용어 | java.lang.String | 검색할 용어입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A simple word query.

### createWordPatternQuery(WordPattern pattern) {#createWordPatternQuery-com.groupdocs.search.common.WordPattern-}
```
public static SearchQuery createWordPatternQuery(WordPattern pattern)
```


단어 패턴 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pattern | [WordPattern](../../com.groupdocs.search.common/wordpattern) | 단어 패턴입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A word pattern query.

### createRegexQuery(String pattern) {#createRegexQuery-java.lang.String-}
```
public static SearchQuery createRegexQuery(String pattern)
```


정규 표현식 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pattern | java.lang.String | 일치시킬 정규 표현식 패턴입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createRegexQuery(String pattern, int options) {#createRegexQuery-java.lang.String-int-}
```
public static SearchQuery createRegexQuery(String pattern, int options)
```


정규 표현식 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | pattern | java.lang.String | 일치시킬 정규 표현식 패턴입니다. |
|
|  | options | int | 정규 표현식을 수정하는 열거형 값들의 비트 연산 조합입니다. 이 값에는 RegexOptions.IgnoreCase 플래그가 포함되어야 합니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A regular expression query.

### createNumericRangeQuery(long start, long end) {#createNumericRangeQuery-long-long-}
```
public static SearchQuery createNumericRangeQuery(long start, long end)
```


숫자 범위 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 시작 | long | 범위의 시작 값입니다. |
|
|  | 끝 | long | 범위의 끝 값입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A numeric range query.

### createDateRangeQuery(Date start, Date end) {#createDateRangeQuery-java.util.Date-java.util.Date-}
```
public static SearchQuery createDateRangeQuery(Date start, Date end)
```


날짜 범위 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 시작 | java.util.Date | 범위의 시작 값입니다. |
|
|  | 끝 | java.util.Date | 범위의 끝 값입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A date range query.

### createPhraseSearchQuery(SearchQuery[] queries) {#createPhraseSearchQuery-com.groupdocs.search.SearchQuery...-}
```
public static SearchQuery createPhraseSearchQuery(SearchQuery[] queries)
```


구문 검색 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 하위 쿼리들입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A phrase search query.

### createAndQuery(SearchQuery[] queries) {#createAndQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createAndQuery(SearchQuery[] queries)
```


각 원본 쿼리에 대해 찾을 수 있는 문서만 찾는 결합된 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 검색할 필드 이름. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createFieldQuery(String fieldName, SearchQuery query) {#createFieldQuery-java.lang.String-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createFieldQuery(String fieldName, SearchQuery query)
```


지정된 쿼리에 필드를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | fieldName | java.lang.String | 검색할 필드 이름. |
|
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 필드를 추가하는 쿼리. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A query with the field to search in.

### createNotQuery(SearchQuery query) {#createNotQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createNotQuery(SearchQuery query)
```


원본 쿼리로 찾을 수 있는 문서를 제외하고 인덱스의 나머지 문서를 찾는 반전 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 반전하는 쿼리. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined NOT query.

### createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createAndQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


각 원본 쿼리에 대해 찾을 수 있는 문서만 찾는 결합된 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 왼쪽 자식 쿼리. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 오른쪽 자식 쿼리. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined AND query.

### createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery) {#createOrQuery-com.groupdocs.search.SearchQuery-com.groupdocs.search.SearchQuery-}
```
public static SearchQuery createOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```


원본 쿼리 중 하나라도 찾을 수 있는 모든 문서를 찾는 결합된 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | leftQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 왼쪽 자식 쿼리. |
|
|  | rightQuery | [SearchQuery](../../com.groupdocs.search/searchquery) | 오른쪽 자식 쿼리. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createOrQuery(SearchQuery[] queries) {#createOrQuery-com.groupdocs.search.SearchQuery---}
```
public static SearchQuery createOrQuery(SearchQuery[] queries)
```


원본 쿼리 중 하나라도 찾을 수 있는 모든 문서를 찾는 결합된 쿼리를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | queries | [SearchQuery\[\]](../../com.groupdocs.search/searchquery) | 하위 쿼리들입니다. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A combined OR query.

### createWildcardQuery(int count) {#createWildcardQuery-int-}
```
public static SearchQuery createWildcardQuery(int count)
```


구문 검색을 위한 와일드카드를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | count | int | 와일드카드의 단어 수. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

### createWildcardQuery(int minCount, int maxCount) {#createWildcardQuery-int-int-}
```
public static SearchQuery createWildcardQuery(int minCount, int maxCount)
```


구문 검색을 위한 와일드카드를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | minCount | int | 와일드카드의 최소 단어 수. |
|
|  | maxCount | int | 와일드카드의 최대 단어 수. |
|

**Returns:**
[SearchQuery](../../com.groupdocs.search/searchquery) - A wildcard for the phrase search.

