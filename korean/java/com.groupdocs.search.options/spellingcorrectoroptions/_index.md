---
title: "SpellingCorrectorOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "맞춤법 교정기에 대한 옵션을 제공합니다."
type: docs
weight: 36
url: /ko/java/com.groupdocs.search.options/spellingcorrectoroptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class SpellingCorrectorOptions
```

맞춤법 교정기에 대한 옵션을 제공합니다.


**Learn more**

* [Spell checking](../https://docs.groupdocs.com/display/searchjava/Spell+checking)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SpellingCorrectorOptions()](#SpellingCorrectorOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEnabled()](#getEnabled--) | 맞춤법 교정기가 활성화되어 있는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabled(boolean value)](#setEnabled-boolean-) | 맞춤법 교정기가 활성화되어 있는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getMaxMistakeCount()](#getMaxMistakeCount--) | 최대 실수 개수를 가져옵니다. |
|
|  | [setMaxMistakeCount(int value)](#setMaxMistakeCount-int-) | 최대 실수 개수를 설정합니다. |
|
|  | [getOnlyBestResults()](#getOnlyBestResults--) | 최고 결과만 반환되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setOnlyBestResults(boolean value)](#setOnlyBestResults-boolean-) | 최고 결과만 반환되는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getOnlyBestResultsRange()](#getOnlyBestResultsRange--) | 발견된 최소 실수 수를 초과하는 최대 값을 가져옵니다. |
|
|  | [setOnlyBestResultsRange(byte value)](#setOnlyBestResultsRange-byte-) | 발견된 최소 실수 수를 초과하는 최대 값을 설정합니다. |
|
|  | [getConsiderTranspositions()](#getConsiderTranspositions--) | 알고리즘이 인접한 두 문자 전환을 하나의 실수로 간주해야 하는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setConsiderTranspositions(boolean value)](#setConsiderTranspositions-boolean-) | 알고리즘이 인접한 두 문자 전환을 하나의 실수로 간주해야 하는지 여부를 나타내는 값을 설정합니다. |
|
### SpellingCorrectorOptions() {#SpellingCorrectorOptions--}
```
public SpellingCorrectorOptions()
```


### getEnabled() {#getEnabled--}
```
public abstract boolean getEnabled()
```


맞춤법 교정기가 활성화되어 있는지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 맞춤법 교정기가 활성화되어 있는지 여부를 나타내는 값.

### setEnabled(boolean value) {#setEnabled-boolean-}
```
public abstract void setEnabled(boolean value)
```


맞춤법 교정기가 활성화되어 있는지 여부를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 맞춤법 교정기가 활성화되어 있는지 여부를 나타내는 값. |
|

### getMaxMistakeCount() {#getMaxMistakeCount--}
```
public abstract int getMaxMistakeCount()
```


최대 실수 개수를 가져옵니다. 기본값은 2 입니다.


**Returns:**
int - 최대 실수 수.

### setMaxMistakeCount(int value) {#setMaxMistakeCount-int-}
```
public abstract void setMaxMistakeCount(int value)
```


실수의 최대 개수를 설정합니다. 기본값은 2입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 최대 실수 수. |
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


알고리즘이 인접한 두 문자 전환을 단일 실수로 간주해야 하는지 여부를 나타내는 값을 가져옵니다. 기본값은 true입니다.


**Returns:**
boolean - 알고리즘이 전환을 고려하는 경우 true; 그렇지 않으면 false.

### setConsiderTranspositions(boolean value) {#setConsiderTranspositions-boolean-}
```
public abstract void setConsiderTranspositions(boolean value)
```


알고리즘이 인접한 두 문자 전환을 단일 실수로 간주해야 하는지 여부를 설정합니다. 기본값은 true입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | true  if the spelling corrector algorithm considers transpositions; otherwise  false . |
|

