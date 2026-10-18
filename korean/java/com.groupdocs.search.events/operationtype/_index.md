---
title: "OperationType"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스 작업 유형을 나타냅니다."
type: docs
weight: 23
url: /ko/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

인덱스 작업 유형을 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Indexing](#Indexing) | 인덱스에 문서를 추가합니다. |
|
|  | [Updating](#Updating) | 인덱스의 문서를 업데이트합니다. |
|
|  | [Merging](#Merging) | 인덱스를 병합합니다. |
|
|  | [Optimizing](#Optimizing) | 인덱스를 최적화합니다. |
|
|  | [Deleting](#Deleting) | 인덱스에서 경로를 삭제합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


인덱스에 문서를 추가합니다.


### Updating {#Updating}
```
public static final OperationType Updating
```


인덱스의 문서를 업데이트합니다.


### Merging {#Merging}
```
public static final OperationType Merging
```


인덱스를 병합합니다.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


인덱스를 최적화합니다.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


인덱스에서 경로를 삭제합니다.


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
