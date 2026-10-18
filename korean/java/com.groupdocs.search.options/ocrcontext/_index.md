---
title: "OcrContext"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "OCR 처리 컨텍스트를 나타냅니다."
type: docs
weight: 30
url: /ko/java/com.groupdocs.search.options/ocrcontext/
---
**Inheritance:**
java.lang.Object
```
public class OcrContext
```

OCR 처리 컨텍스트를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)](#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-) | 새 인스턴스를 초기화합니다 |
OcrContext
클래스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getImageStream()](#getImageStream--) | 처리할 이미지를 포함하는 스트림을 가져옵니다. |
|
|  | [getImageLocation()](#getImageLocation--) | 이미지의 위치를 가져옵니다. |
|
|  | [getImageFileExtension()](#getImageFileExtension--) | 이미지의 파일 확장자를 가져옵니다. |
|
### OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension) {#OcrContext-java.io.InputStream-com.groupdocs.search.options.ImageLocation-java.lang.String-}
```
public OcrContext(InputStream imageStream, ImageLocation imageLocation, String imageFileExtension)
```


새 인스턴스를 초기화합니다
OcrContext
클래스.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | 처리할 이미지를 포함하는 스트림. |
|
|  | imageLocation | [ImageLocation](../../com.groupdocs.search.options/imagelocation) | 이미지의 위치. |
|
|  | imageFileExtension | java.lang.String | 이미지의 파일 확장자. |
|

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


처리할 이미지를 포함하는 스트림을 가져옵니다.


**Returns:**
java.io.InputStream - 처리할 이미지를 포함하는 스트림.

### getImageLocation() {#getImageLocation--}
```
public final ImageLocation getImageLocation()
```


이미지의 위치를 가져옵니다.


**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation) - The location of the image.

### getImageFileExtension() {#getImageFileExtension--}
```
public final String getImageFileExtension()
```


이미지의 파일 확장자를 가져옵니다.
이 값은 이미지 유형을 결정하는 데 사용할 수 있습니다.


**Returns:**
java.lang.String - 이미지의 파일 확장자.

