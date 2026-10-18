---
title: "DeleteResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에서 인덱싱된 파일 또는 폴더를 삭제하는 작업의 결과를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

인덱스에서 인덱싱된 파일 또는 폴더를 삭제하는 작업의 결과를 나타냅니다.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | 각 경로 삭제 결과를 반환합니다. |
|
|  | [getTotalCount()](#getTotalCount--) | 삭제할 경로의 총 수를 반환합니다. |
|
|  | [getSuccessCount()](#getSuccessCount--) | 성공적으로 삭제된 경로 수를 반환합니다. |
|
|  | [getFailedCount()](#getFailedCount--) | 오류로 인해 삭제되지 않은 경로 수를 반환합니다. |
|
|  | [getErrors()](#getErrors--) | 삭제 오류에 대한 설명을 반환합니다. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


각 경로 삭제 결과를 반환합니다.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - 각 경로 삭제 결과.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


삭제할 경로의 총 수를 반환합니다.


**Returns:**
int - 삭제할 경로의 총 수.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


성공적으로 삭제된 경로 수를 반환합니다.


**Returns:**
int - 성공적으로 삭제된 경로의 수.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


오류로 인해 삭제되지 않은 경로 수를 반환합니다.


**Returns:**
int - 오류로 인해 삭제되지 않은 경로의 수.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


삭제 오류에 대한 설명을 반환합니다.


**Returns:**
java.lang.String[] - 삭제 오류에 대한 설명.

