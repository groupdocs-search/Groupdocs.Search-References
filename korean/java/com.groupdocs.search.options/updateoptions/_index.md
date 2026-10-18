---
title: "UpdateOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "업데이트 작업에 대한 옵션을 제공합니다."
type: docs
weight: 43
url: /ko/java/com.groupdocs.search.options/updateoptions/
---
**Inheritance:**
java.lang.Object
```
public class UpdateOptions
```

업데이트 작업에 대한 옵션을 제공합니다.


**Learn more**

* [Update index](../https://docs.groupdocs.com/display/searchjava/Update+index)
* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [UpdateOptions()](#UpdateOptions--) | UpdateOptions 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [UpdateOptions(Object data)](#UpdateOptions-java.lang.Object-) | UpdateOptions 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getThreads()](#getThreads--) | 인덱싱에 사용되는 스레드 수를 가져옵니다. |
|
|  | [setThreads(int value)](#setThreads-int-) | 인덱싱에 사용되는 스레드 수를 설정합니다. |
|
|  | [isAsync()](#isAsync--) | 작업을 비동기적으로 수행하는 플래그를 가져옵니다. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | 작업을 비동기적으로 수행하는 플래그를 설정합니다. |
|
|  | [getCancellation()](#getCancellation--) | 작업 취소 객체를 가져옵니다. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | 작업 취소 객체를 설정합니다. |
|
|  | [getAutoDetectEncoding()](#getAutoDetectEncoding--) | 인코딩을 자동으로 감지할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | 인코딩을 자동으로 감지할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getEncoding()](#getEncoding--) | 텍스트 문서에서 텍스트를 추출하는 데 사용되는 인코딩을 가져옵니다. |
|
|  | [setEncoding(String value)](#setEncoding-java.lang.String-) | 텍스트 문서에서 텍스트를 추출하는 데 사용되는 인코딩을 설정합니다. |
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
### UpdateOptions() {#UpdateOptions--}
```
public UpdateOptions()
```


UpdateOptions 클래스의 새 인스턴스를 초기화합니다.


### UpdateOptions(Object data) {#UpdateOptions-java.lang.Object-}
```
public UpdateOptions(Object data)
```


UpdateOptions 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 데이터 | java.lang.Object | 직렬화된 데이터입니다. |
|

### getThreads() {#getThreads--}
```
public int getThreads()
```


인덱싱에 사용되는 스레드 수를 가져옵니다. 기본값은 1입니다.


**Returns:**
int - 인덱싱에 사용되는 스레드 수.

### setThreads(int value) {#setThreads-int-}
```
public void setThreads(int value)
```


인덱싱에 사용되는 스레드 수를 설정합니다. 기본값은 1입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 인덱싱에 사용되는 스레드 수. |
|

### isAsync() {#isAsync--}
```
public boolean isAsync()
```


작업을 비동기적으로 수행하는 플래그를 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 작업을 비동기적으로 수행하는 플래그.

### setAsync(boolean value) {#setAsync-boolean-}
```
public void setAsync(boolean value)
```


작업을 비동기적으로 수행하는 플래그를 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 작업을 비동기적으로 수행하는 플래그. |
|

### getCancellation() {#getCancellation--}
```
public Cancellation getCancellation()
```


작업 취소 객체를 가져옵니다. 기본값은 null입니다.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public void setCancellation(Cancellation value)
```


작업 취소 객체를 설정합니다. 기본값은 null입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | 작업 취소 객체. |
|

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public boolean getAutoDetectEncoding()
```


인코딩을 자동으로 감지할지 여부를 나타내는 값을 가져옵니다. 기본값은 false입니다.


**Returns:**
boolean - 인코딩을 자동으로 감지할지 여부를 나타내는 값.

### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public void setAutoDetectEncoding(boolean value)
```


인코딩을 자동으로 감지할지 여부를 나타내는 값을 설정합니다. 기본값은 false입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 인코딩을 자동으로 감지할지 여부를 나타내는 값. |
|

### getEncoding() {#getEncoding--}
```
public String getEncoding()
```


텍스트 문서에서 텍스트를 추출하는 데 사용되는 인코딩을 가져옵니다. 기본값은 null이며, 이는 기본 인코딩인 UTF-8이 사용됨을 의미합니다. AutoDetectEncoding이 true이면 이 값이 기본 인코딩으로 사용됩니다.


**Returns:**
java.lang.String - 텍스트 문서에서 텍스트를 추출하는 데 사용되는 인코딩.

### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public void setEncoding(String value)
```


텍스트 문서에서 텍스트를 추출하는 데 사용되는 인코딩을 설정합니다. 기본값은 null이며, 이는 기본 인코딩인 UTF-8이 사용됨을 의미합니다. AutoDetectEncoding이 true이면 이 값이 기본 인코딩으로 사용됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | java.lang.String | 텍스트 문서에서 텍스트를 추출하는 데 사용되는 인코딩. |
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
