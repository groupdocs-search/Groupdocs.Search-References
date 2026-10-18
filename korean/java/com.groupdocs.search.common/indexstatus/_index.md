---
title: "IndexStatus"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스 상태를 지정합니다."
type: docs
weight: 41
url: /ko/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

인덱스 상태를 지정합니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Ready](#Ready) | 인덱스가 자유롭고 변경 준비가 되었습니다. |
|
|  | [Failed](#Failed) | 오류로 인해 인덱스를 다시 로드해야 합니다. |
|
|  | [Indexing](#Indexing) | 인덱스가 색인 작업을 수행합니다. |
|
|  | [Updating](#Updating) | 인덱스가 업데이트 작업을 수행합니다. |
|
|  | [Merging](#Merging) | 인덱스가 병합 작업을 수행합니다. |
|
|  | [Optimizing](#Optimizing) | 인덱스가 최적화 작업을 수행합니다. |
|
|  | [Deleting](#Deleting) | 인덱스는 삭제 작업을 수행합니다. |
|
|  | [Renaming](#Renaming) | 인덱스는 이름 바꾸기 작업을 수행합니다. |
|
|  | [ChangingAttributes](#ChangingAttributes) | 인덱스는 속성을 변경합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


인덱스가 자유롭고 변경 준비가 되었습니다.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


오류로 인해 인덱스를 다시 로드해야 합니다.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


인덱스가 색인 작업을 수행합니다.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


인덱스가 업데이트 작업을 수행합니다.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


인덱스가 병합 작업을 수행합니다.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


인덱스가 최적화 작업을 수행합니다.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


인덱스는 삭제 작업을 수행합니다.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


인덱스는 이름 바꾸기 작업을 수행합니다.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


인덱스는 속성을 변경합니다.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
