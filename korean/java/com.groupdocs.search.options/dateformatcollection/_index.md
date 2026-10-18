---
title: "DateFormatCollection"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "DateFormat 객체의 컬렉션을 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.options/dateformatcollection/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public abstract class DateFormatCollection implements Iterable<DateFormat>
```

DateFormat 객체 컬렉션을 나타냅니다.


**Learn more**

* [Date range search](../https://docs.groupdocs.com/display/searchjava/Date+range+search)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DateFormatCollection()](#DateFormatCollection--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [addItem(DateFormat item)](#addItem-com.groupdocs.search.options.DateFormat-) | 컬렉션에 날짜 형식 객체를 추가합니다. |
|
|  | [clear()](#clear--) | 컬렉션의 모든 요소를 제거합니다. |
|
|  | [containsItem(DateFormat item)](#containsItem-com.groupdocs.search.options.DateFormat-) | 컬렉션에 특정 항목이 포함되어 있는지 확인합니다. |
|
|  | [copyToTArray(DateFormat[] array, int arrayIndex)](#copyToTArray-com.groupdocs.search.options.DateFormat---int-) | 컬렉션의 요소를 지정된 배열에 복사하고, 특정 배열 인덱스에서 시작합니다. |
|
|  | [size()](#size--) | 컬렉션에 포함된 요소 수를 가져옵니다. |
|
|  | [isReadOnly()](#isReadOnly--) | 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
|
|  | [removeItem(DateFormat item)](#removeItem-com.groupdocs.search.options.DateFormat-) | 컬렉션에서 특정 요소의 첫 번째 발생을 제거합니다. |
|
|  | [iterator()](#iterator--) | 컬렉션을 순회하는 열거자를 반환합니다. |
|
### DateFormatCollection() {#DateFormatCollection--}
```
public DateFormatCollection()
```


### addItem(DateFormat item) {#addItem-com.groupdocs.search.options.DateFormat-}
```
public abstract void addItem(DateFormat item)
```


컬렉션에 날짜 형식 객체를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | 컬렉션에 추가할 날짜 형식 객체입니다. |
|

### clear() {#clear--}
```
public abstract void clear()
```


컬렉션의 모든 요소를 제거합니다.


### containsItem(DateFormat item) {#containsItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean containsItem(DateFormat item)
```


컬렉션에 특정 항목이 포함되어 있는지 확인합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | 컬렉션에서 찾을 항목입니다. |
|

**Returns:**
boolean - 컬렉션에서 항목을 찾으면 true, 그렇지 않으면 false.

### copyToTArray(DateFormat[] array, int arrayIndex) {#copyToTArray-com.groupdocs.search.options.DateFormat---int-}
```
public abstract void copyToTArray(DateFormat[] array, int arrayIndex)
```


컬렉션의 요소를 지정된 배열에 복사하고, 특정 배열 인덱스에서 시작합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | array | [DateFormat\[\]](../../com.groupdocs.search.options/dateformat) | 컬렉션에서 복사된 요소들의 대상이 되는 1차원 Array입니다. |
|
|  | arrayIndex | int | 복사가 시작되는 배열의 0 기반 인덱스입니다. |
|

### size() {#size--}
```
public abstract int size()
```


컬렉션에 포함된 요소 수를 가져옵니다.


**Returns:**
int - 컬렉션에 포함된 요소 수입니다.

### isReadOnly() {#isReadOnly--}
```
public abstract boolean isReadOnly()
```


컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 컬렉션이 읽기 전용이면 true, 그렇지 않으면 false.

### removeItem(DateFormat item) {#removeItem-com.groupdocs.search.options.DateFormat-}
```
public abstract boolean removeItem(DateFormat item)
```


컬렉션에서 특정 요소의 첫 번째 발생을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | item | [DateFormat](../../com.groupdocs.search.options/dateformat) | 컬렉션에서 제거할 항목입니다. |
|

**Returns:**
boolean - 컬렉션에서 항목이 성공적으로 제거되면 true, 그렇지 않으면 false. 이 메서드는 컬렉션에서 항목을 찾지 못한 경우에도 false를 반환합니다.

### iterator() {#iterator--}
```
public abstract Iterator<DateFormat> iterator()
```


컬렉션을 순회하는 열거자를 반환합니다.


**Returns:**
java.util.Iterator<com.groupdocs.search.options.DateFormat> - 컬렉션을 순회하는 데 사용할 수 있는 열거자입니다.

