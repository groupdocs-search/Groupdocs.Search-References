---
title: "TextOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱스에서 문서 텍스트를 검색하기 위한 옵션을 제공합니다."
type: docs
weight: 41
url: /ko/java/com.groupdocs.search.options/textoptions/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.groupdocs.search.options.ITextOptions](../../com.groupdocs.search.options/itextoptions)
```
public class TextOptions implements ITextOptions
```

인덱스에서 문서 텍스트를 검색하기 위한 옵션을 제공합니다.


**Learn more**

* [Getting indexed documents](../https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents)
* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [TextOptions()](#TextOptions--) | TextOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [TextOptions(Object data)](#TextOptions-java.lang.Object-) | TextOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getCustomExtractor()](#getCustomExtractor--) | 인덱싱에 사용된 사용자 정의 텍스트 추출기를 가져옵니다. |
|
|  | [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | 인덱싱에 사용된 사용자 정의 텍스트 추출기를 설정합니다. |
|
|  | [getAdditionalFields()](#getAdditionalFields--) | 인덱싱에 사용된 추가 문서 필드를 가져옵니다. |
|
|  | [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | 인덱싱에 사용된 추가 문서 필드를 설정합니다. |
|
|  | [getCancellation()](#getCancellation--) | 취소 객체를 가져옵니다. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 취소 객체를 설정합니다. |
|
|  | [getGenerateHead()](#getGenerateHead--) | 출력 HTML에 Head 태그가 생성되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setGenerateHead(boolean value)](#setGenerateHead-boolean-) | 출력 HTML에 Head 태그가 생성되는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getUseRawTextExtraction()](#getUseRawTextExtraction--) | 가능한 경우 원시 모드가 텍스트 추출에 사용되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | 가능한 경우 원시 모드가 텍스트 추출에 사용되는지 여부를 나타내는 값을 설정합니다. |
|
|  | [getMetadataIndexingOptions()](#getMetadataIndexingOptions--) | 메타데이터 필드 인덱싱 옵션을 가져옵니다. |
|
|  | [getOcrIndexingOptions()](#getOcrIndexingOptions--) | OCR 처리 및 인식된 텍스트 인덱싱 옵션을 가져옵니다. |
|
|  | [getImageIndexingOptions()](#getImageIndexingOptions--) | 역 이미지 검색을 위한 이미지 인덱싱 옵션을 가져옵니다. |
|
| [getCore()](#getCore--) |  |
### TextOptions() {#TextOptions--}
```
public TextOptions()
```


TextOptions 클래스의 새 인스턴스를 초기화합니다.


### TextOptions(Object data) {#TextOptions-java.lang.Object-}
```
public TextOptions(Object data)
```


TextOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getCustomExtractor() {#getCustomExtractor--}
```
public IFieldExtractor getCustomExtractor()
```


인덱싱에 사용된 사용자 정의 텍스트 추출기를 가져옵니다. 기본값은 null 입니다. 이 값은 문서 텍스트가 인덱스에 저장되지 않은 경우에만 사용됩니다.


**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor that was used for indexing.

### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public void setCustomExtractor(IFieldExtractor value)
```


인덱싱에 사용된 사용자 정의 텍스트 추출기를 설정합니다. 기본값은 null 입니다. 이 값은 문서 텍스트가 인덱스에 저장되지 않은 경우에만 사용됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | 인덱싱에 사용된 사용자 정의 텍스트 추출기. |
|

### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


인덱싱에 사용된 추가 문서 필드를 가져옵니다. 기본값은 null 입니다. 이 값은 문서 텍스트가 인덱스에 저장되지 않은 경우에만 사용됩니다.


**Returns:**
com.groupdocs.search.common.DocumentField[] - 인덱싱에 사용된 추가 문서 필드.

### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


인덱싱에 사용된 추가 문서 필드를 설정합니다. 기본값은 null 입니다. 이 값은 문서 텍스트가 인덱스에 저장되지 않은 경우에만 사용됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 인덱싱에 사용된 추가 문서 필드. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


취소 객체를 가져옵니다. 기본값은 null 입니다.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


취소 객체를 설정합니다. 기본값은 null 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 취소 객체. |
|

### getGenerateHead() {#getGenerateHead--}
```
public boolean getGenerateHead()
```


출력 HTML에 Head 태그가 생성되는지 여부를 나타내는 값을 가져옵니다. 기본값은 true 입니다.


**Returns:**
boolean - 출력 HTML에 Head 태그가 생성되는지 여부를 나타내는 값.

### setGenerateHead(boolean value) {#setGenerateHead-boolean-}
```
public void setGenerateHead(boolean value)
```


출력 HTML에 Head 태그가 생성되는지 여부를 나타내는 값을 설정합니다. 기본값은 true 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 출력 HTML에 Head 태그가 생성되는지 여부를 나타내는 값. |
|

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public boolean getUseRawTextExtraction()
```


가능한 경우 원시 모드가 텍스트 추출에 사용되는지 여부를 나타내는 값을 가져옵니다. 기본값은 true 입니다. 원시 모드는 인덱싱 속도를 크게 높일 수 있지만, 일반 모드는 추출된 텍스트의 형식을 개선합니다.


**Returns:**
boolean - 가능한 경우 원시 모드가 텍스트 추출에 사용되는지 여부를 나타내는 값.

### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public void setUseRawTextExtraction(boolean value)
```


가능한 경우 원시 모드가 텍스트 추출에 사용되는지 여부를 나타내는 값을 설정합니다. 기본값은 true 입니다. 원시 모드는 인덱싱 속도를 크게 높일 수 있지만, 일반 모드는 추출된 텍스트의 형식을 개선합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 가능한 경우 원시 모드가 텍스트 추출에 사용되는지 여부를 나타내는 값. |
|

### getMetadataIndexingOptions() {#getMetadataIndexingOptions--}
```
public MetadataIndexingOptions getMetadataIndexingOptions()
```


메타데이터 필드 인덱싱 옵션을 가져옵니다.


**Returns:**
[MetadataIndexingOptions](../../com.groupdocs.search.options/metadataindexingoptions) - The options for indexing metadata fields.

### getOcrIndexingOptions() {#getOcrIndexingOptions--}
```
public OcrIndexingOptions getOcrIndexingOptions()
```


OCR 처리 및 인식된 텍스트 인덱싱 옵션을 가져옵니다.


**Returns:**
[OcrIndexingOptions](../../com.groupdocs.search.options/ocrindexingoptions) - The options for OCR processing and indexing recognized text.

### getImageIndexingOptions() {#getImageIndexingOptions--}
```
public ImageIndexingOptions getImageIndexingOptions()
```


역 이미지 검색을 위한 이미지 인덱싱 옵션을 가져옵니다.


**Returns:**
[ImageIndexingOptions](../../com.groupdocs.search.options/imageindexingoptions) - The image indexing options for reverse image search.

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
