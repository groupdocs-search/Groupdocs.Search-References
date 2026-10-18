---
title: "VersionUpdateResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스 버전 업데이트 작업의 결과를 나타냅니다."
type: docs
weight: 42
url: /ko/java/com.groupdocs.search.common/versionupdateresult/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum VersionUpdateResult extends Enum<VersionUpdateResult>
```

인덱스 버전 업데이트 작업의 결과를 나타냅니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Updated](#Updated) | 인덱스 버전이 업데이트되었습니다. |
|
|  | [AlreadyUpToDate](#AlreadyUpToDate) | 인덱스 버전이 이미 최신 상태입니다. |
|
|  | [Unsupported](#Unsupported) | 인덱스 버전을 지원하지 않거나 디렉터리에 유효한 인덱스 데이터가 포함되어 있지 않습니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Updated {#Updated}
```
public static final VersionUpdateResult Updated
```


인덱스 버전이 업데이트되었습니다.


### AlreadyUpToDate {#AlreadyUpToDate}
```
public static final VersionUpdateResult AlreadyUpToDate
```


인덱스 버전이 이미 최신 상태입니다.


### Unsupported {#Unsupported}
```
public static final VersionUpdateResult Unsupported
```


인덱스 버전을 지원하지 않거나 디렉터리에 유효한 인덱스 데이터가 포함되어 있지 않습니다.


### values() {#values--}
```
public static VersionUpdateResult[] values()
```




**Returns:**
com.groupdocs.search.common.VersionUpdateResult[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static VersionUpdateResult valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VersionUpdateResult](../../com.groupdocs.search.common/versionupdateresult)
