---
title: "OcrIndexingOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "OCR 처리 및 인식된 텍스트 인덱싱에 대한 옵션을 제공합니다."
type: docs
weight: 31
url: /ko/java/com.groupdocs.search.options/ocrindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class OcrIndexingOptions
```

OCR 처리 및 인식된 텍스트 인덱싱에 대한 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [OcrIndexingOptions()](#OcrIndexingOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | 별도의 이미지 파일에서 텍스트를 인식할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | 별도의 이미지 파일에서 텍스트를 인식할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | 컨테이너의 항목인 이미지(예: ZIP 아카이브의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | 컨테이너의 항목인 이미지(예: ZIP 아카이브의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | 내장된 이미지(예: DOCX 문서의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | 내장된 이미지(예: DOCX 문서의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR 처리를 위해 사용되는 OCR 커넥터를 가져옵니다. |
|
|  | [setOcrConnector(IOcrConnector value)](#setOcrConnector-com.groupdocs.search.options.IOcrConnector-) | OCR 처리를 위해 사용되는 OCR 커넥터를 설정합니다. |
|
### OcrIndexingOptions() {#OcrIndexingOptions--}
```
public OcrIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


별도의 이미지 파일에서 텍스트를 인식할지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 별도의 이미지 파일에서 텍스트를 인식할지 여부를 나타내는 값.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


별도의 이미지 파일에서 텍스트를 인식할지 여부를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 별도의 이미지 파일에서 텍스트를 인식할지 여부를 나타내는 값. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


컨테이너의 항목인 이미지(예: ZIP 아카이브의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 컨테이너의 항목인 이미지에서 텍스트를 인식할지 여부를 나타내는 값.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


컨테이너의 항목인 이미지(예: ZIP 아카이브의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 컨테이너의 항목인 이미지에서 텍스트를 인식할지 여부를 나타내는 값. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


내장된 이미지(예: DOCX 문서의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 내장된 이미지에서 텍스트를 인식할지 여부를 나타내는 값.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


내장된 이미지(예: DOCX 문서의 이미지)에서 텍스트를 인식할지 여부를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 내장된 이미지에서 텍스트를 인식할지 여부를 나타내는 값. |
|

### getOcrConnector() {#getOcrConnector--}
```
public abstract IOcrConnector getOcrConnector()
```


OCR 처리를 위해 사용되는 OCR 커넥터를 가져옵니다. 기본값은 null이며, 이는 OCR이 사용되지 않음을 의미합니다.


**Returns:**
[IOcrConnector](../../com.groupdocs.search.options/iocrconnector) - An OCR connector that is used for OCR processing.

### setOcrConnector(IOcrConnector value) {#setOcrConnector-com.groupdocs.search.options.IOcrConnector-}
```
public abstract void setOcrConnector(IOcrConnector value)
```


OCR 처리를 위해 사용되는 OCR 커넥터를 설정합니다. 기본값은 null이며, 이는 OCR이 사용되지 않음을 의미합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [IOcrConnector](../../com.groupdocs.search.options/iocrconnector) | OCR 처리를 위해 사용되는 OCR 커넥터입니다. |
|

