---
title: "AttributeChangeBatch"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "속성 변경을 위한 컨테이너를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.common/attributechangebatch/
---
**Inheritance:**
java.lang.Object
```
public class AttributeChangeBatch
```

속성 변경을 위한 컨테이너를 나타냅니다.


**Learn more**

* [Document attributes](../https://docs.groupdocs.com/display/searchjava/Document+attributes)
* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [AttributeChangeBatch()](#AttributeChangeBatch--) | AttributeChangeBatch 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [AttributeChangeBatch(Object data)](#AttributeChangeBatch-java.lang.Object-) | AttributeChangeBatch 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [add(String path, String[] attributes)](#add-java.lang.String-java.lang.String...-) | 지정된 속성을 지정된 인덱싱된 문서에 추가합니다. |
|
|  | [add(String[] paths, String[] attributes)](#add-java.lang.String---java.lang.String...-) | 지정된 속성을 지정된 인덱싱된 문서들에 추가합니다. |
|
|  | [addToAll(String[] attributes)](#addToAll-java.lang.String...-) | 인덱스의 모든 문서에 지정된 속성을 추가합니다. |
|
|  | [remove(String path, String[] attributes)](#remove-java.lang.String-java.lang.String...-) | 지정된 인덱싱된 문서에서 지정된 속성을 제거합니다. |
|
|  | [remove(String[] paths, String[] attributes)](#remove-java.lang.String---java.lang.String...-) | 지정된 인덱싱된 문서들에서 지정된 속성을 제거합니다. |
|
|  | [removeAll(String path)](#removeAll-java.lang.String-) | 지정된 인덱싱된 문서에서 모든 속성을 제거합니다. |
|
|  | [removeAll(String[] paths)](#removeAll-java.lang.String---) | 지정된 인덱싱된 문서들에서 모든 속성을 제거합니다. |
|
|  | [removeFromAll(String[] attributes)](#removeFromAll-java.lang.String...-) | 인덱스의 모든 문서에서 지정된 속성을 제거합니다. |
|
|  | [clear()](#clear--) | 인덱스의 모든 문서에서 모든 속성을 제거합니다. |
|
| [getCore()](#getCore--) |  |
### AttributeChangeBatch() {#AttributeChangeBatch--}
```
public AttributeChangeBatch()
```


AttributeChangeBatch 클래스의 새 인스턴스를 초기화합니다.


### AttributeChangeBatch(Object data) {#AttributeChangeBatch-java.lang.Object-}
```
public AttributeChangeBatch(Object data)
```


AttributeChangeBatch 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### add(String path, String[] attributes) {#add-java.lang.String-java.lang.String...-}
```
public void add(String path, String[] attributes)
```


지정된 속성을 지정된 인덱싱된 문서에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 문서 경로입니다. |
|
|  | 속성 | java.lang.String[] | 추가할 속성들. |
|

### add(String[] paths, String[] attributes) {#add-java.lang.String---java.lang.String...-}
```
public void add(String[] paths, String[] attributes)
```


지정된 속성을 지정된 인덱싱된 문서들에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | paths | java.lang.String[] | 문서 경로들. |
|
|  | 속성 | java.lang.String[] | 추가할 속성들. |
|

### addToAll(String[] attributes) {#addToAll-java.lang.String...-}
```
public void addToAll(String[] attributes)
```


인덱스의 모든 문서에 지정된 속성을 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 속성 | java.lang.String[] | 추가할 속성들. |
|

### remove(String path, String[] attributes) {#remove-java.lang.String-java.lang.String...-}
```
public void remove(String path, String[] attributes)
```


지정된 인덱싱된 문서에서 지정된 속성을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 문서 경로입니다. |
|
|  | 속성 | java.lang.String[] | 제거할 속성들. |
|

### remove(String[] paths, String[] attributes) {#remove-java.lang.String---java.lang.String...-}
```
public void remove(String[] paths, String[] attributes)
```


지정된 인덱싱된 문서들에서 지정된 속성을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | paths | java.lang.String[] | 문서 경로들. |
|
|  | 속성 | java.lang.String[] | 제거할 속성들. |
|

### removeAll(String path) {#removeAll-java.lang.String-}
```
public void removeAll(String path)
```


지정된 인덱싱된 문서에서 모든 속성을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 문서 경로입니다. |
|

### removeAll(String[] paths) {#removeAll-java.lang.String---}
```
public void removeAll(String[] paths)
```


지정된 인덱싱된 문서들에서 모든 속성을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | paths | java.lang.String[] | 문서 경로들. |
|

### removeFromAll(String[] attributes) {#removeFromAll-java.lang.String...-}
```
public void removeFromAll(String[] attributes)
```


인덱스의 모든 문서에서 지정된 속성을 제거합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 속성 | java.lang.String[] | 제거할 속성들. |
|

### clear() {#clear--}
```
public void clear()
```


인덱스의 모든 문서에서 모든 속성을 제거합니다.


### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
