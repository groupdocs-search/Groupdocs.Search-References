---
title: "IndexType"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스 유형을 지정합니다."
type: docs
weight: 49
url: /ko/java/com.groupdocs.search.options/indextype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexType extends Enum<IndexType>
```

인덱스 유형을 지정합니다.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [NormalIndex](#NormalIndex) | 문서 메타데이터와 문서 내용을 포함한 일반 인덱스로, 모든 검색 기능을 지원합니다. |
|
|  | [MetadataIndex](#MetadataIndex) | 내용 없이 문서 메타데이터만 포함하는 인덱스입니다. |
|
|  | [CompactIndex](#CompactIndex) | 디스크 공간을 크게 절약하지만 구문 검색 및 날짜 범위 검색 기능을 지원하지 않는 인덱스 유형입니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### NormalIndex {#NormalIndex}
```
public static final IndexType NormalIndex
```


문서 메타데이터와 문서 내용을 포함한 일반 인덱스로, 모든 검색 기능을 지원합니다.


### MetadataIndex {#MetadataIndex}
```
public static final IndexType MetadataIndex
```


내용 없이 문서 메타데이터만 포함하는 인덱스입니다.


### CompactIndex {#CompactIndex}
```
public static final IndexType CompactIndex
```


디스크 공간을 크게 절약하지만 구문 검색 및 날짜 범위 검색 기능을 지원하지 않는 인덱스 유형입니다.


### values() {#values--}
```
public static IndexType[] values()
```




**Returns:**
com.groupdocs.search.options.IndexType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexType valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype)
