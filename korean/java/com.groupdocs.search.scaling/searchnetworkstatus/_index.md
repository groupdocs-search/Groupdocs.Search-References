---
title: "SearchNetworkStatus"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색 네트워크 상태를 지정합니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

검색 네트워크 상태를 지정합니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Ready](#Ready) | 검색 네트워크가 자유롭고 변경 준비가 되어 있습니다. |
|
|  | [Configuring](#Configuring) | 검색 네트워크가 구성 작업을 수행합니다. |
|
|  | [Indexing](#Indexing) | 검색 네트워크가 인덱싱 작업을 수행합니다. |
|
|  | [Optimizing](#Optimizing) | 검색 네트워크가 최적화 작업을 수행합니다. |
|
|  | [Deleting](#Deleting) | 검색 네트워크가 삭제 작업을 수행합니다. |
|
|  | [ChangingAttributes](#ChangingAttributes) | 검색 네트워크가 속성을 변경합니다. |
|
|  | [Synchronizing](#Synchronizing) | 검색 네트워크가 동기화 작업을 수행합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


검색 네트워크가 자유롭고 변경 준비가 되어 있습니다.


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


검색 네트워크가 구성 작업을 수행합니다.


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


검색 네트워크가 인덱싱 작업을 수행합니다.


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


검색 네트워크가 최적화 작업을 수행합니다.


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


검색 네트워크가 삭제 작업을 수행합니다.


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


검색 네트워크가 속성을 변경합니다.


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


검색 네트워크가 동기화 작업을 수행합니다.


### values() {#values--}
```
public static SearchNetworkStatus[] values()
```




**Returns:**
com.groupdocs.search.scaling.SearchNetworkStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchNetworkStatus valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
