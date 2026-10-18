---
title: "DocumentSourceKind"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 소스의 종류를 정의합니다."
type: docs
weight: 39
url: /ko/java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

문서 소스의 종류를 정의합니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [File](#File) | 파일 문서 소스입니다. |
|
|  | [Stream](#Stream) | 스트림 문서 소스입니다. |
|
|  | [Structure](#Structure) | 구조 문서 소스입니다. |
|
|  | [ExtractedData](#ExtractedData) | 이전에 추출된 데이터의 문서 소스입니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


파일 문서 소스입니다.


### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


스트림 문서 소스입니다.


### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


구조 문서 소스입니다.


### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


이전에 추출된 데이터의 문서 소스입니다.


### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
