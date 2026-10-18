---
title: "PathDeleteResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에서 인덱싱된 파일 또는 폴더를 삭제하는 작업 결과를 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

인덱스에서 인덱싱된 파일 또는 폴더를 삭제하는 작업 결과를 나타냅니다.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [isSuccess()](#isSuccess--) | 삭제 작업의 성공 지표를 반환합니다. |
|
|  | [getError()](#getError--) | 삭제 오류에 대한 설명을 반환합니다. |
|
|  | [getPath()](#getPath--) | 삭제할 파일 또는 폴더의 경로를 반환합니다. |
|
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


삭제 작업의 성공 지표를 반환합니다.


**Returns:**
boolean - 삭제 작업이 성공하면 true; 그렇지 않으면 false를 반환합니다.

### getError() {#getError--}
```
public final String getError()
```


삭제 오류에 대한 설명을 반환합니다.


**Returns:**
java.lang.String - 삭제 오류에 대한 설명.

### getPath() {#getPath--}
```
public final String getPath()
```


삭제할 파일 또는 폴더의 경로를 반환합니다.


**Returns:**
java.lang.String - 삭제할 파일 또는 폴더의 경로.

