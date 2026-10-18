---
title: "FragmentContainer"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "하나의 문서 필드에서 찾은 용어가 강조 표시된 텍스트 조각을 위한 컨테이너를 나타냅니다."
type: docs
weight: 22
url: /ko/java/com.groupdocs.search.common/fragmentcontainer/
---
**Inheritance:**
java.lang.Object
```
public abstract class FragmentContainer
```

하나의 문서 필드에서 찾은 용어가 강조 표시된 텍스트 조각을 위한 컨테이너를 나타냅니다.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FragmentContainer()](#FragmentContainer--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFieldName()](#getFieldName--) | 문서 필드 이름을 가져옵니다. |
|
|  | [getCount()](#getCount--) | 포함된 텍스트 조각의 수를 가져옵니다. |
|
|  | [getFragments()](#getFragments--) | 포함된 텍스트 조각들의 배열을 가져옵니다. |
|
### FragmentContainer() {#FragmentContainer--}
```
public FragmentContainer()
```


### getFieldName() {#getFieldName--}
```
public abstract String getFieldName()
```


문서 필드 이름을 가져옵니다.


**Returns:**
java.lang.String - 문서 필드 이름.

### getCount() {#getCount--}
```
public abstract int getCount()
```


포함된 텍스트 조각의 수를 가져옵니다.


**Returns:**
int - 포함된 텍스트 조각의 수.

### getFragments() {#getFragments--}
```
public abstract String[] getFragments()
```


포함된 텍스트 조각들의 배열을 가져옵니다.


**Returns:**
java.lang.String[] - 포함된 텍스트 조각들의 배열.

