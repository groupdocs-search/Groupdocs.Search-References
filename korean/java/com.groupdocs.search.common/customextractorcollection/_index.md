---
title: "CustomExtractorCollection"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "맞춤 추출기의 컬렉션을 포함합니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.common/customextractorcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class CustomExtractorCollection implements Iterable
```

사용자 정의 추출기 컬렉션을 포함합니다. 컬렉션에 기본 제공 추출기가 지원하는 파일 확장자에 대한 추출기가 포함되어 있는 경우, 해당 추출기가 기본 제공 추출기 대신 사용됩니다.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [CustomExtractorCollection()](#CustomExtractorCollection--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [size()](#size--) | 컬렉션에 포함된 추출기 수를 가져옵니다. |
|
|  | [isReadOnly()](#isReadOnly--) | 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
|
|  | [iterator()](#iterator--) | 이 컬렉션에 대한 반복자를 반환합니다. |
|
|  | [addItem(IFieldExtractor extractor)](#addItem-com.groupdocs.search.common.IFieldExtractor-) | 추출기를 컬렉션에 추가합니다. |
|
|  | [clear()](#clear--) | 컬렉션에서 모든 추출기를 제거합니다. |
|
|  | [containsItem(IFieldExtractor item)](#containsItem-com.groupdocs.search.common.IFieldExtractor-) | 컬렉션에 특정 추출기가 포함되어 있는지 확인합니다. |
|
|  | [copyToTArray(IFieldExtractor[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-) | 컬렉션의 요소를 배열에 복사합니다. 복사는 지정된 배열 인덱스부터 시작합니다. |
|
|  | [removeItem(IFieldExtractor extractor)](#removeItem-com.groupdocs.search.common.IFieldExtractor-) | 컬렉션에서 추출기를 제거합니다. |
|
### CustomExtractorCollection() {#CustomExtractorCollection--}
```
public CustomExtractorCollection()
```


### size() {#size--}
```
public abstract int size()
```


컬렉션에 포함된 추출기 수를 가져옵니다.


**Returns:**
int - 컬렉션에 포함된 추출기의 수.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 컬렉션이 읽기 전용인지 여부를 나타내는 값.

### iterator() {#iterator--}
```
public abstract Iterator<IFieldExtractor> iterator()
```


이 컬렉션에 대한 반복자를 반환합니다.


**Returns:**
java.util.Iterator<com.groupdocs.search.common.IFieldExtractor> - 컬렉션을 순회하는 데 사용할 수 있는 반복자 객체.

### addItem(IFieldExtractor extractor) {#addItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract void addItem(IFieldExtractor extractor)
```


추출기를 컬렉션에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 컬렉션에 추가할 추출기. |
|

### clear() {#clear--}
```
public abstract void clear()
```


컬렉션에서 모든 추출기를 제거합니다.


### containsItem(IFieldExtractor item) {#containsItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean containsItem(IFieldExtractor item)
```


컬렉션에 특정 추출기가 포함되어 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | item | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 컬렉션에서 찾을 추출기. |
|

**Returns:**
boolean - 컬렉션에서 항목이 발견되면 true, 그렇지 않으면 false.

### copyToTArray(IFieldExtractor[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.common.IFieldExtractor---int-}
```
public abstract void copyToTArray(IFieldExtractor[] array, int arrayIndex)
```


컬렉션의 요소를 배열에 복사합니다. 복사는 지정된 배열 인덱스부터 시작합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | array | [IFieldExtractor\[\]](../../com.groupdocs.search.common/ifieldextractor) | 컬렉션에서 복사된 요소의 대상이 되는 1차원 배열입니다. 배열은 0부터 시작하는 인덱스를 가져야 합니다. |
|
|  | arrayIndex | int | 복사가 시작되는 배열의 0 기반 인덱스입니다. |
|

### removeItem(IFieldExtractor extractor) {#removeItem-com.groupdocs.search.common.IFieldExtractor-}
```
public abstract boolean removeItem(IFieldExtractor extractor)
```


컬렉션에서 추출기를 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | extractor | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 컬렉션에서 제거할 추출기. |
|

**Returns:**
boolean - 컬렉션에서 추출기가 성공적으로 제거되면 true, 그렇지 않으면 false. 원래 컬렉션에 추출기가 없으면 이 메서드는 false를 반환합니다.

