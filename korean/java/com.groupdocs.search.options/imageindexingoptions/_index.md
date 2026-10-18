---
title: "ImageIndexingOptions"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "역 이미지 검색을 위한 이미지 인덱싱 옵션을 제공합니다."
type: docs
weight: 23
url: /ko/java/com.groupdocs.search.options/imageindexingoptions/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageIndexingOptions
```

역 이미지 검색을 위한 이미지 인덱싱 옵션을 제공합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ImageIndexingOptions()](#ImageIndexingOptions--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEnabledForSeparateImages()](#getEnabledForSeparateImages--) | 별도의 이미지 파일을 인덱싱할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabledForSeparateImages(boolean value)](#setEnabledForSeparateImages-boolean-) | 별도의 이미지 파일을 인덱싱할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getEnabledForContainerItemImages()](#getEnabledForContainerItemImages--) | 컨테이너 내 항목인 이미지(예: ZIP 아카이브의 이미지)를 인덱싱할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabledForContainerItemImages(boolean value)](#setEnabledForContainerItemImages-boolean-) | 컨테이너 내 항목인 이미지(예: ZIP 아카이브의 이미지)를 인덱싱할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getEnabledForEmbeddedImages()](#getEnabledForEmbeddedImages--) | 내장된 이미지(예: DOCX 문서의 이미지)를 인덱싱할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setEnabledForEmbeddedImages(boolean value)](#setEnabledForEmbeddedImages-boolean-) | 내장된 이미지(예: DOCX 문서의 이미지)를 인덱싱할지 여부를 나타내는 값을 설정합니다. |
|
### ImageIndexingOptions() {#ImageIndexingOptions--}
```
public ImageIndexingOptions()
```


### getEnabledForSeparateImages() {#getEnabledForSeparateImages--}
```
public abstract boolean getEnabledForSeparateImages()
```


별도의 이미지 파일을 인덱싱할지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 별도의 이미지 파일을 인덱싱할지 여부를 나타내는 값.

### setEnabledForSeparateImages(boolean value) {#setEnabledForSeparateImages-boolean-}
```
public abstract void setEnabledForSeparateImages(boolean value)
```


별도의 이미지 파일을 인덱싱할지 여부를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 별도의 이미지 파일을 인덱싱할지 여부를 나타내는 값. |
|

### getEnabledForContainerItemImages() {#getEnabledForContainerItemImages--}
```
public abstract boolean getEnabledForContainerItemImages()
```


컨테이너 내 항목인 이미지(예: ZIP 아카이브의 이미지)를 인덱싱할지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 컨테이너 내 항목인 이미지들을 인덱싱할지 여부를 나타내는 값.

### setEnabledForContainerItemImages(boolean value) {#setEnabledForContainerItemImages-boolean-}
```
public abstract void setEnabledForContainerItemImages(boolean value)
```


컨테이너 내 항목인 이미지들을 인덱싱할지 여부를 나타내는 값을 설정합니다 (예: ZIP 아카이브의 이미지). 기본값은  false  입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 컨테이너 내 항목인 이미지들을 인덱싱할지 여부를 나타내는 값. |
|

### getEnabledForEmbeddedImages() {#getEnabledForEmbeddedImages--}
```
public abstract boolean getEnabledForEmbeddedImages()
```


내장된 이미지들을 인덱싱할지 여부를 나타내는 값을 가져옵니다 (예: DOCX 문서의 이미지). 기본값은  false  입니다.


**Returns:**
boolean - 내장된 이미지들을 인덱싱할지 여부를 나타내는 값.

### setEnabledForEmbeddedImages(boolean value) {#setEnabledForEmbeddedImages-boolean-}
```
public abstract void setEnabledForEmbeddedImages(boolean value)
```


내장된 이미지들을 인덱싱할지 여부를 나타내는 값을 설정합니다 (예: DOCX 문서의 이미지). 기본값은  false  입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 내장된 이미지들을 인덱싱할지 여부를 나타내는 값. |
|

