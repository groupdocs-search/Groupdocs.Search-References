---
title: "SimilarityLevel"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "유사 검색 알고리즘을 나타내며, 유사성 수준을 지정합니다."
type: docs
weight: 35
url: /ko/java/com.groupdocs.search.options/similaritylevel/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class SimilarityLevel extends FuzzyAlgorithm
```

유사도 수준을 지정하는 퍼지 검색 알고리즘을 나타냅니다. 유사도 수준 알고리즘은 단어 길이에 반비례하여 단어당 허용되는 최대 실수 개수를 계산합니다.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스를 생성합니다.
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 퍼지 검색 활성화
options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8)); // 퍼지 검색 알고리즘 생성
// 이 함수는 1~4자 단어에 대해 최대 실수 개수를 0으로 지정합니다.
// 5~9자 단어에 대해 최대 실수 개수를 1로 지정합니다.
// 10~14자 단어에 대해 최대 실수 개수를 2로 지정합니다. 이후 동일하게 적용됩니다.
SearchResult result = index.search(query, options); // 인덱스에서 검색
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [SimilarityLevel(double value)](#SimilarityLevel-double-) | SimilarityLevel 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [SimilarityLevel(Object data)](#SimilarityLevel-java.lang.Object-) | SimilarityLevel 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 지정된 용어 길이에 대한 유사도 수준 값을 가져옵니다. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 지정된 용어 길이에 허용되는 최대 실수 개수를 가져옵니다. |
|
### SimilarityLevel(double value) {#SimilarityLevel-double-}
```
public SimilarityLevel(double value)
```


SimilarityLevel 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | double | 유사도 수준 값입니다. |
|

### SimilarityLevel(Object data) {#SimilarityLevel-java.lang.Object-}
```
public SimilarityLevel(Object data)
```


SimilarityLevel 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


지정된 용어 길이에 대한 유사도 수준 값을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | termLength | int | 용어 길이입니다. |
|

**Returns:**
double - 유사도 수준 값입니다.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


지정된 용어 길이에 허용되는 최대 실수 개수를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | termLength | int | 용어 길이입니다. |
|

**Returns:**
int - 허용되는 최대 실수 수.

