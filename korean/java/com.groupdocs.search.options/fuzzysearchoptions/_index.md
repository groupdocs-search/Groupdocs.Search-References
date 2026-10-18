---
title: "FuzzySearchOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "퍼지 검색 옵션을 제공합니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.search.options/fuzzysearchoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzySearchOptions
```

퍼지 검색 옵션을 제공합니다.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FuzzySearchOptions()](#FuzzySearchOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | 퍼지 검색 기능이 활성화되어 있는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | 퍼지 검색 기능이 활성화되어 있는지를 나타내는 값을 설정합니다. |
|
|  | [getFuzzyAlgorithm()](#getFuzzyAlgorithm--) | 퍼지 검색 알고리즘을 가져옵니다. |
|
|  | [setFuzzyAlgorithm(FuzzyAlgorithm value)](#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-) | 퍼지 검색 알고리즘을 설정합니다. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | 최고 결과만 반환되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | 최고 결과만 반환되는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | 발견된 최소 실수 수를 초과하는 최대 값을 가져옵니다. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | 발견된 최소 실수 수를 초과하는 최대 값을 설정합니다. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | 퍼지 검색 알고리즘이 인접한 두 문자 위치 교환을 하나의 오류로 간주해야 하는지를 나타내는 값을 가져옵니다. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | 퍼지 검색 알고리즘이 인접한 두 문자 위치 교환을 하나의 오류로 간주해야 하는지를 나타내는 값을 설정합니다. |
|
### FuzzySearchOptions() {#FuzzySearchOptions--}
```
public FuzzySearchOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


퍼지 검색 기능이 활성화되어 있는지를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 퍼지 검색 기능이 활성화되어 있는지를 나타내는 값.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


퍼지 검색 기능이 활성화되어 있는지를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 퍼지 검색 기능이 활성화되어 있는지를 나타내는 값. |
|

### getFuzzyAlgorithm() {#getFuzzyAlgorithm--}
```
public abstract FuzzyAlgorithm getFuzzyAlgorithm()
```


퍼지 검색 알고리즘을 가져옵니다. 현재 사용 가능한 퍼지 검색 알고리즘은 SimilarityLevel와 TableDiscreteFunction입니다. 기본값은 유사도 수준 값이 0.5인 SimilarityLevel 인스턴스입니다.


**Returns:**
[FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) - The fuzzy search algorithm.


이 예제는 퍼지 검색 알고리즘을 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스를 생성합니다.
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 퍼지 검색 활성화
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // 퍼지 검색 알고리즘을 생성합니다.
// 이 함수는 1~4자 단어에 대해 최대 실수 개수를 1로 지정합니다.
// 이 함수는 5~7자 단어에 대해 최대 실수 개수를 2로 지정합니다.
// 이 함수는 8자 이상 단어에 대해 최대 실수 개수를 3으로 지정합니다.
SearchResult result = index.search(query, options); // 인덱스에서 검색
 
```
 
````


### setFuzzyAlgorithm(FuzzyAlgorithm value) {#setFuzzyAlgorithm-com.groupdocs.search.options.FuzzyAlgorithm-}
```
public abstract void setFuzzyAlgorithm(FuzzyAlgorithm value)
```


퍼지 검색 알고리즘을 설정합니다. 현재 사용 가능한 퍼지 검색 알고리즘은 SimilarityLevel와 TableDiscreteFunction입니다. 기본값은 유사도 수준 값이 0.5인 SimilarityLevel 인스턴스입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm) | 퍼지 검색 알고리즘. |


이 예제는 퍼지 검색 알고리즘을 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스를 생성합니다.
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 퍼지 검색 활성화
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // 퍼지 검색 알고리즘을 생성합니다.
// 이 함수는 1~4자 단어에 대해 최대 실수 개수를 1로 지정합니다.
// 이 함수는 5~7자 단어에 대해 최대 실수 개수를 2로 지정합니다.
// 이 함수는 8자 이상 단어에 대해 최대 실수 개수를 3으로 지정합니다.
SearchResult result = index.search(query, options); // 인덱스에서 검색
 
```
 
````

|

### getOnlyBestResults() {#getOnlyBestResults--}
```
public abstract boolean getOnlyBestResults()
```


최고 결과만 반환되는지 여부를 나타내는 값을 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 최고 결과만 반환되는 경우 true; 그렇지 않으면 false.

### setOnlyBestResults(boolean value) {#setOnlyBestResults-boolean-}
```
public abstract void setOnlyBestResults(boolean value)
```


최고 결과만 반환되는지 여부를 나타내는 값을 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | true  if only the best results will be returned; otherwise  false . |
|

### getOnlyBestResultsRange() {#getOnlyBestResultsRange--}
```
public abstract byte getOnlyBestResultsRange()
```


찾은 최소 실수 개수를 초과하는 최대 값을 가져옵니다. 기본값은 0입니다.


**Returns:**
byte - 찾은 최소 실수 개수를 초과하는 최대 값.

### setOnlyBestResultsRange(byte value) {#setOnlyBestResultsRange-byte-}
```
public abstract void setOnlyBestResultsRange(byte value)
```


찾은 최소 실수 개수를 초과하는 최대 값을 설정합니다. 기본값은 0입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | byte | 찾은 최소 실수 개수를 초과하는 최대 값. |
|

### getConsiderTranspositions() {#getConsiderTranspositions--}
```
public abstract boolean getConsiderTranspositions()
```


퍼지 검색 알고리즘이 인접한 두 문자 위치 교환을 하나의 오류로 간주해야 하는지를 나타내는 값을 가져옵니다. 기본값은 true 입니다.


**Returns:**
boolean - 퍼지 검색 알고리즘이 전치(transposition)를 고려하면 true, 그렇지 않으면 false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


퍼지 검색 알고리즘이 인접한 두 문자 위치 교환을 하나의 오류로 간주해야 하는지를 나타내는 값을 설정합니다. 기본값은 true 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | : 퍼지 검색 알고리즘이 전치를 고려하면 true, 그렇지 않으면 false. |
|

