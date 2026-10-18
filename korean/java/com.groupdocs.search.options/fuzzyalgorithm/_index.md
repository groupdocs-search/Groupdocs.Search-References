---
title: "FuzzyAlgorithm"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "퍼지 검색 알고리즘의 기본 클래스를 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.groupdocs.search.options/fuzzyalgorithm/
---
**Inheritance:**
java.lang.Object
```
public abstract class FuzzyAlgorithm
```

퍼지 검색 알고리즘의 기본 클래스를 나타냅니다.


**Learn more**

* [Fuzzy search](../https://docs.groupdocs.com/display/searchjava/Fuzzy+search)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getSimilarityLevel(int termLength)](#getSimilarityLevel-int-) | 지정된 용어 길이에 대한 유사도 수준을 가져옵니다. |
|
|  | [getMaxMistakeCount(int termLength)](#getMaxMistakeCount-int-) | 지정된 용어 길이에 허용되는 최대 실수 개수를 가져옵니다. |
|
| [getCore()](#getCore--) |  |
### getSimilarityLevel(int termLength) {#getSimilarityLevel-int-}
```
public abstract double getSimilarityLevel(int termLength)
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
public abstract int getMaxMistakeCount(int termLength)
```


지정된 용어 길이에 허용되는 최대 실수 개수를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | termLength | int | 용어 길이입니다. |
|

**Returns:**
int - 허용되는 최대 실수 수.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
