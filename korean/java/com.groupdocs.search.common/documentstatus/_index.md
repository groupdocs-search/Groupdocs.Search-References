---
title: "DocumentStatus"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 처리 상태를 나타냅니다."
type: docs
weight: 40
url: /ko/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

문서 처리 상태를 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | 문서가 성공적으로 색인되었습니다. |
|
|  | [Skipped](#Skipped) | 문서가 건너뛰었습니다. |
|
|  | [ProcessedWithError](#ProcessedWithError) | 문서 색인 중 오류가 발생했습니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


문서가 성공적으로 색인되었습니다.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


문서가 건너뛰었습니다.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


문서 색인 중 오류가 발생했습니다.


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
