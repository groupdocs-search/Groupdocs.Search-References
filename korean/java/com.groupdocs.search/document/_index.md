---
title: "문서"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "파일 시스템 스트림 또는 구조에서 인덱스로 추가된 문서의 기본 클래스를 나타냅니다."
type: docs
weight: 13
url: /ko/java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

파일 시스템, 스트림 또는 구조에서 인덱스로 추가된 문서의 기본 클래스를 나타냅니다. 다양한 유형의 소스에서 문서를 생성하기 위한 정적 메서드를 포함합니다.


**Learn more**

* [Indexing from different sources](../https://docs.groupdocs.com/search/java/indexing-from-different-sources/)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentSourceKind()](#getDocumentSourceKind--) | 문서 소스 종류를 가져옵니다. |
|
|  | [getDocumentKey()](#getDocumentKey--) | 인덱스 내에서 문서를 식별하는 데 사용되는 문서 키를 가져옵니다. |
|
|  | [isLazy()](#isLazy--) | 문서가 필요에 따라 로드되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getModificationDate()](#getModificationDate--) | 문서의 마지막 수정 날짜를 가져옵니다. |
|
|  | [getExtension()](#getExtension--) | 이 문서 유형에 사용되는 확장자를 가져옵니다. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | 문서에 대한 추가 필드를 가져옵니다. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | 문서에 대한 추가 필드를 설정합니다. |
|
|  | [getAttributes()](#getAttributes--) | 문서의 속성을 가져옵니다. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | 문서의 속성을 설정합니다. |
|
|  | [createFromFile(String filePath)](#createFromFile-java.lang.String-) | 파일에서 문서를 생성합니다. |
|
|  | [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | 스트림에서 문서를 생성합니다. |
|
|  | [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | 텍스트 필드 배열인 구조에서 문서를 생성합니다. |
|
|  | [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | 지연 로드 문서를 생성합니다. |
|
|  | [toString()](#toString--) | 현재  Document 를 나타내는  java.lang.String  을 반환합니다. |
|
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


문서 소스 종류를 가져옵니다.


**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.

### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


인덱스 내에서 문서를 식별하는 데 사용되는 문서 키를 가져옵니다.


**Returns:**
java.lang.String - 인덱스 내에서 문서를 식별하는 데 사용되는 문서 키.

### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


문서가 필요에 따라 로드되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 문서가 필요에 따라 로드되는지 여부를 나타내는 값.

### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


문서의 마지막 수정 날짜를 가져옵니다.


**Returns:**
java.util.Date - 문서의 마지막 수정 날짜.

### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


이 문서 유형에 사용되는 확장자를 가져옵니다.


**Returns:**
java.lang.String - 이 문서 유형에 사용되는 확장자.

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


문서에 대한 추가 필드를 가져옵니다.


**Returns:**
com.groupdocs.search.common.DocumentField[] - 문서에 대한 추가 필드.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


문서에 대한 추가 필드를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 문서에 대한 추가 필드입니다. |
|

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


문서의 속성을 가져옵니다.


**Returns:**
java.lang.String[] - 문서의 속성입니다.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


문서의 속성을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String[] | 문서의 속성입니다. |
|

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


파일에서 문서를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 문서 파일 경로입니다. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


스트림에서 문서를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentKey | java.lang.String | 문서 키입니다. |
|
|  | modificationDate | java.util.Date | 문서 수정 날짜입니다. |
|
|  | extension | java.lang.String | 문서 확장자입니다. |
|
|  | stream | java.io.InputStream | 문서 스트림입니다. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


텍스트 필드 배열인 구조에서 문서를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentKey | java.lang.String | 문서 키입니다. |
|
|  | modificationDate | java.util.Date | 문서 수정 날짜입니다. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 문서 필드입니다. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


지연 로드 문서를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | 문서 소스 종류입니다. 이 값은 로드된 문서의 종류와 일치해야 합니다. |
|
|  | documentKey | java.lang.String | 문서 키입니다. 이 값은 로드된 문서의 키와 일치해야 합니다. |
|
|  | documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | 문서 로더입니다. |
|

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.

### toString() {#toString--}
```
public String toString()
```


현재  Document 를 나타내는  java.lang.String  을 반환합니다.


**Returns:**
java.lang.String - 현재 Document 를 나타내는 java.lang.String

