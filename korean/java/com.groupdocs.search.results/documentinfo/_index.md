---
title: "DocumentInfo"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱된 문서에 대한 설명자를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentInfo
```

인덱싱된 문서에 대한 설명자를 나타냅니다.


**Learn more**

* [Search results](../https://docs.groupdocs.com/display/searchjava/Search+results)
* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentInfo()](#DocumentInfo--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [toString()](#toString--) | 현재 DocumentInfo을 나타내는 System.String을 반환합니다. |
|
|  | [getFilePath()](#getFilePath--) | 파일에서 인덱싱된 경우 파일 경로를, 스트림이나 구조에서 인덱싱된 경우 문서 키를 가져옵니다. |
|
|  | [getFileType()](#getFileType--) | 파일 유형을 가져옵니다. |
|
|  | [getFormatFamily()](#getFormatFamily--) | 문서 형식 패밀리를 가져옵니다. |
|
|  | [getInnerPath()](#getInnerPath--) | 컨테이너 문서 항목의 내부 경로를 가져옵니다. |
|
|  | [getInnerPathParts()](#getInnerPathParts--) | 컨테이너 문서 항목의 내부 경로 부분을 가져옵니다. |
|
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | 문서 소스 종류를 가져옵니다. |
|
|  | [getIndexedWithError()](#getIndexedWithError--) | 인덱싱 오류 표시기를 가져옵니다. |
|
|  | [serialize()](#serialize--) | 현재 인스턴스를 바이트 배열로 직렬화합니다. |
|
|  | [deserialize(byte[] array)](#deserialize-byte---) | 바이트 배열에서 인스턴스를 역직렬화합니다. |
|
### DocumentInfo() {#DocumentInfo--}
```
public DocumentInfo()
```


### toString() {#toString--}
```
public abstract String toString()
```


현재 DocumentInfo을 나타내는 System.String을 반환합니다.


**Returns:**
java.lang.String - 현재 DocumentInfo을 나타내는 System.String.

### getFilePath() {#getFilePath--}
```
public abstract String getFilePath()
```


파일에서 인덱싱된 경우 파일 경로를, 스트림이나 구조에서 인덱싱된 경우 문서 키를 가져옵니다.


**Returns:**
java.lang.String - 파일 경로나 문서 키.

### getFileType() {#getFileType--}
```
public abstract FileType getFileType()
```


파일 유형을 가져옵니다.


**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.

### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


문서 형식 패밀리를 가져옵니다.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getInnerPath() {#getInnerPath--}
```
public abstract String getInnerPath()
```


컨테이너 문서 항목의 내부 경로를 가져옵니다.


**Returns:**
java.lang.String - 내부 경로입니다.

### getInnerPathParts() {#getInnerPathParts--}
```
public abstract String[] getInnerPathParts()
```


컨테이너 문서 항목의 내부 경로 부분을 가져옵니다.


**Returns:**
java.lang.String[] - 내부 경로 부분.

### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


문서 소스 종류를 가져옵니다.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getIndexedWithError() {#getIndexedWithError--}
```
public abstract boolean getIndexedWithError()
```


인덱싱 오류 표시기를 가져옵니다.


**Returns:**
boolean - 인덱싱 오류 표시기.

### serialize() {#serialize--}
```
public abstract byte[] serialize()
```


현재 인스턴스를 바이트 배열로 직렬화합니다.


**Returns:**
byte[] - 현재 인스턴스를 나타내는 바이트 배열.

### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


바이트 배열에서 인스턴스를 역직렬화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 배열 | byte[] | 역직렬화에 사용할 바이트 배열. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.

