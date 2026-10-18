---
title: "TableDiscreteFunction"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "단어 길이와 허용 가능한 오류 수 사이의 대응 관계를 포함하는 퍼지 검색 알고리즘을 나타냅니다."
type: docs
weight: 40
url: /ko/java/com.groupdocs.search.options/tablediscretefunction/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.options.FuzzyAlgorithm](../../com.groupdocs.search.options/fuzzyalgorithm)
```
public class TableDiscreteFunction extends FuzzyAlgorithm
```

단어 길이와 허용 가능한 실수 수 사이의 대응 관계를 포함하는 퍼지 검색 알고리즘을 나타냅니다. 이 알고리즘은 출력 값 표 또는 단계 함수로 지정할 수 있습니다.


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
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1, new Step(5, 2), new Step(8, 3))); // 퍼지 검색 알고리즘을 생성합니다.
// 이 함수는 1~4자 단어에 대해 최대 실수 개수를 1로 지정합니다.
// 이 함수는 5~7자 단어에 대해 최대 실수 개수를 2로 지정합니다.
// 이 함수는 8자 이상 단어에 대해 최대 실수 개수를 3으로 지정합니다.
SearchResult result = index.search(query, options); // 인덱스에서 검색
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)](#TableDiscreteFunction-int-int---) | TableDiscreteFunction 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TableDiscreteFunction(int firstStepLevel, Step[] steps)](#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-) | TableDiscreteFunction 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 지정된 용어 길이에 대한 유사도 수준을 가져옵니다. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 지정된 용어 길이에 대한 허용 가능한 최대 실수 수를 가져옵니다. |
|
### TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs) {#TableDiscreteFunction-int-int---}
```
public TableDiscreteFunction(int offsetOfInputs, int[] tableOfOutputs)
```


TableDiscreteFunction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | offsetOfInputs | int | 입력 값에 상대적인 테이블 인덱스의 오프셋입니다. |
|
|  | tableOfOutputs | int[] | 출력 값의 테이블입니다. |
|

### TableDiscreteFunction(int firstStepLevel, Step[] steps) {#TableDiscreteFunction-int-com.groupdocs.search.options.Step...-}
```
public TableDiscreteFunction(int firstStepLevel, Step[] steps)
```


TableDiscreteFunction 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | firstStepLevel | int | 스텝 함수의 첫 번째 단계 수준입니다. |
|
|  | steps | [Step\[\]](../../com.groupdocs.search.options/step) | 스텝 함수의 다음 단계들입니다. |
|

### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public double getSimilarityLevel(int termLength)
```


지정된 용어 길이에 대한 유사도 수준을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | termLength | int | 용어 길이입니다. |
|

**Returns:**
double - 유사도 수준.

### getMaxMistakeCount(int termLength) {#getMaxMistakeCount-int-}
```
public int getMaxMistakeCount(int termLength)
```


지정된 용어 길이에 대한 허용 가능한 최대 실수 수를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | termLength | int | 용어 길이입니다. |
|

**Returns:**
int - 허용 가능한 최대 실수 수.

