---
title: "DocumentField"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 필드 데이터를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.search.common/documentfield/
---
**Inheritance:**
java.lang.Object
```
public class DocumentField
```

문서 필드 데이터를 나타냅니다.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)
* [Indexing additional fields](../https://docs.groupdocs.com/display/searchjava/Indexing+additional+fields)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [DocumentField(String name, String value)](#DocumentField-java.lang.String-java.lang.String-) | DocumentField 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [DocumentField(Object data)](#DocumentField-java.lang.Object-) | DocumentField 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getName()](#getName--) | 필드 이름을 가져옵니다. |
|
|  | [getValue()](#getValue--) | 필드 값을 가져옵니다. |
|
| [getCore()](#getCore--) |  |
### DocumentField(String name, String value) {#DocumentField-java.lang.String-java.lang.String-}
```
public DocumentField(String name, String value)
```


DocumentField 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | name | java.lang.String | 필드 이름. |
|
|  | 값 | java.lang.String | 필드 값. |
|

### DocumentField(Object data) {#DocumentField-java.lang.Object-}
```
public DocumentField(Object data)
```


DocumentField 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getName() {#getName--}
```
public String getName()
```


필드 이름을 가져옵니다.


**Returns:**
java.lang.String - 필드 이름입니다.

### getValue() {#getValue--}
```
public String getValue()
```


필드 값을 가져옵니다.


**Returns:**
java.lang.String - 필드 값.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
