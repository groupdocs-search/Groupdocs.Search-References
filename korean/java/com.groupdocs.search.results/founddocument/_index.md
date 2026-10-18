---
title: "FoundDocument"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색된 문서를 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.results/founddocument/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundDocument
```

검색된 문서를 나타냅니다.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FoundDocument()](#FoundDocument--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | 문서 정보를 가져옵니다. |
|
|  | [getRelevance()](#getRelevance--) | 검색 결과의 관련성을 가져옵니다. |
|
|  | [getOccurrenceCount()](#getOccurrenceCount--) | 발견된 발생 횟수를 가져옵니다. |
|
|  | [getFoundFields()](#getFoundFields--) | 찾은 문서 필드를 가져옵니다. |
|
|  | [getTerms()](#getTerms--) | 발견된 용어를 가져옵니다. |
|
|  | [getTermSequences()](#getTermSequences--) | 발견된 용어 시퀀스를 가져옵니다. |
|
|  | [getAttributes()](#getAttributes--) | 찾은 문서와 연결된 속성을 가져옵니다. |
|
|  | [toString()](#toString--) | 찾은 문서의 문자열 표현을 반환합니다. |
|
|  | [serialize()](#serialize--) | 현재 인스턴스를 바이트 배열로 직렬화합니다. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 바이트 배열에서 인스턴스를 역직렬화합니다. |
|
### FoundDocument() {#FoundDocument--}
```
public FoundDocument()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


문서 정보를 가져옵니다.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getRelevance() {#getRelevance--}
```
public abstract double getRelevance()
```


검색 결과의 관련성을 가져옵니다.


**Returns:**
double - 검색 결과의 관련성.

### getOccurrenceCount() {#getOccurrenceCount--}
```
public abstract int getOccurrenceCount()
```


발견된 발생 횟수를 가져옵니다.


**Returns:**
int - 발견된 발생 횟수.

### getFoundFields() {#getFoundFields--}
```
public abstract FoundDocumentField[] getFoundFields()
```


찾은 문서 필드를 가져옵니다.


**Returns:**
com.groupdocs.search.results.FoundDocumentField[] - 찾은 문서 필드.

### getTerms() {#getTerms--}
```
public abstract String[] getTerms()
```


찾은 용어를 가져옵니다. 값은 속성이 접근될 때마다 평가됩니다.


**Returns:**
java.lang.String[] - 발견된 용어.

### getTermSequences() {#getTermSequences--}
```
public abstract String[][] getTermSequences()
```


발견된 용어 시퀀스를 가져옵니다.


**Returns:**
java.lang.String[][] - 발견된 용어 시퀀스.

### getAttributes() {#getAttributes--}
```
public abstract String[] getAttributes()
```


찾은 문서와 연결된 속성을 가져옵니다. 속성을 검색하려면 검색 옵션에서 해당 옵션을 활성화해야 합니다.


**Returns:**
java.lang.String[] - 찾은 문서와 연결된 속성.

### toString() {#toString--}
```
public abstract String toString()
```


찾은 문서의 문자열 표현을 반환합니다.


**Returns:**
java.lang.String - 찾은 문서를 나타내는 문자열.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


현재 인스턴스를 바이트 배열로 직렬화합니다.


**Returns:**
byte[] - 현재 인스턴스를 나타내는 바이트 배열.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static FoundDocument deserialize(byte[] array)
```


바이트 배열에서 인스턴스를 역직렬화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 배열 | byte[] | 역직렬화에 사용할 바이트 배열. |
|

**Returns:**
[FoundDocument](../../com.groupdocs.search.results/founddocument) - An instance deserialized from a byte array.

