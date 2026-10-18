---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 인덱싱 시작 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 14
url: /ko/java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

문서 인덱싱 시작 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocument()](#getDocument--) | 문서를 가져옵니다. |
|
|  | [getDocumentFullPath()](#getDocumentFullPath--) | 문서의 전체 경로를 가져옵니다. |
|
|  | [getDocumentKey()](#getDocumentKey--) | 문서 키를 가져옵니다. |
|
|  | [getSkipIndexing()](#getSkipIndexing--) | 문서 인덱싱을 건너뛰어야 함을 나타내는 값을 가져옵니다. |
|
|  | [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | 문서 인덱싱을 건너뛰어야 함을 나타내는 값을 설정합니다. |
|
|  | [getEncoding()](#getEncoding--) | 문서의 인코딩을 가져옵니다. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | 문서의 인코딩을 설정합니다. |
|
|  | [getCustomExtractor()](#getCustomExtractor--) | 사용자 정의 텍스트 추출기를 가져옵니다. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | 사용자 정의 텍스트 추출기를 설정합니다. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | 문서에 대한 추가 필드를 가져옵니다. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | 문서에 대한 추가 필드를 설정합니다. |
|
|  | [getAttributes()](#getAttributes--) | 문서의 속성을 가져옵니다. |
|
|  | [setAttributes(String[] value)](#setAttributes-java.lang.String---) | 문서의 속성을 설정합니다. |
|
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


문서를 가져옵니다.


**Returns:**
[Document](../../com.groupdocs.search/document) - The document.

### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


문서의 전체 경로를 가져옵니다.


**Returns:**
java.lang.String - 문서의 전체 경로.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


문서 키를 가져옵니다.


**Returns:**
java.lang.String - 문서 키.

### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


문서 인덱싱을 건너뛰어야 함을 나타내는 값을 가져옵니다.


**Returns:**
boolean - 문서 인덱싱을 건너뛰어야 함을 나타내는 값.

### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


문서 인덱싱을 건너뛰어야 함을 나타내는 값을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 문서 인덱싱을 건너뛰어야 함을 나타내는 값. |
|

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


문서의 인코딩을 가져옵니다.


**Returns:**
java.lang.String - 문서의 인코딩.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


문서의 인코딩을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 문서의 인코딩. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


사용자 정의 텍스트 추출기를 가져옵니다.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


사용자 정의 텍스트 추출기를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 사용자 정의 텍스트 추출기입니다. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


문서에 대한 추가 필드를 가져옵니다.


**Returns:**
com.groupdocs.search.common.DocumentField[] - 문서에 대한 추가 필드.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


문서에 대한 추가 필드를 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 문서에 대한 추가 필드입니다. |
|

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


문서의 속성을 가져옵니다.


**Returns:**
java.lang.String[] - 문서의 속성입니다.

### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


문서의 속성을 설정합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String[] | 문서의 속성입니다. |
|

