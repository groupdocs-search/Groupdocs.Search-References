---
title: "FoundDocumentField"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색된 문서 필드를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.search.results/founddocumentfield/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocumentField
```

검색된 문서 필드를 나타냅니다.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FoundDocumentField()](#FoundDocumentField--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | 필드 이름을 가져옵니다. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 발견된 발생 횟수를 가져옵니다. |
|
|  | [getTerms()](#getTerms--) | 발견된 용어를 가져옵니다. |
|
|  | [getTermsOccurrences()](#getTermsOccurrences--) | 발견된 용어의 발생을 가져옵니다. |
|
|  | [getTermSequences()](#getTermSequences--) | 발견된 용어 시퀀스를 가져옵니다. |
|
|  | [getTermSequencesOccurrences()](#getTermSequencesOccurrences--) | 발견된 용어 시퀀스의 발생을 가져옵니다. |
|
|  | [toString()](#toString--) | 찾은 문서 필드의 문자열 표현을 반환합니다. |
|
|  | [serialize()](#serialize--) | 현재 인스턴스를 바이트 배열로 직렬화합니다. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 바이트 배열에서 인스턴스를 역직렬화합니다. |
|
### FoundDocumentField() {#FoundDocumentField--}
```
public FoundDocumentField()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


필드 이름을 가져옵니다.


**Returns:**
java.lang.String - 필드 이름입니다.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


발견된 발생 횟수를 가져옵니다.


**Returns:**
int - 발견된 발생 횟수.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


발견된 용어를 가져옵니다.


**Returns:**
java.lang.String[] - 발견된 용어.

### getTermsOccurrences() {#getTermsOccurrences--}
```
public abstract int[] getTermsOccurrences()
```


발견된 용어의 발생을 가져옵니다.


**Returns:**
int[] - 발견된 용어의 발생.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


발견된 용어 시퀀스를 가져옵니다.


**Returns:**
java.lang.String[][] - 발견된 용어 시퀀스.

### getTermSequencesOccurrences() {#getTermSequencesOccurrences--}
```
public abstract int[] getTermSequencesOccurrences()
```


발견된 용어 시퀀스의 발생을 가져옵니다.


**Returns:**
int[] - 발견된 용어 시퀀스의 발생.

### toString() {#toString--}
```
public abstract String toString()
```


찾은 문서 필드의 문자열 표현을 반환합니다.


**Returns:**
java.lang.String - 찾은 문서 필드를 나타내는 문자열.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


현재 인스턴스를 바이트 배열로 직렬화합니다.


**Returns:**
byte[] - 현재 인스턴스를 나타내는 바이트 배열.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocumentField deserialize(byte[] array)
```


바이트 배열에서 인스턴스를 역직렬화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 배열 | byte[] | 역직렬화에 사용할 바이트 배열. |
|

**Returns:**
[FoundDocumentField](../../com.groupdocs.search.results/founddocumentfield) - An instance deserialized from a byte array.

