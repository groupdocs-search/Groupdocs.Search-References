---
title: "ImagePreparingEventArgs"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이미지 준비 시작 이벤트에 대한 인수를 나타냅니다."
type: docs
weight: 15
url: /ko/java/com.groupdocs.search.events/imagepreparingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class ImagePreparingEventArgs extends BaseIndexEventArgs
```

이미지 준비 시작 이벤트에 대한 인수를 나타냅니다.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentKey()](#getDocumentKey--) | 문서 키를 가져옵니다. |
|
|  | [getInnerPath()](#getInnerPath--) | 중첩된 문서의 내부 경로를 가져옵니다. |
|
|  | [getImageIndex()](#getImageIndex--) | 문서 내 이미지의 순번을 가져옵니다. |
|
|  | [getImageFrames()](#getImageFrames--) | 이미지 프레임을 가져옵니다. |
|
|  | [getImageStream()](#getImageStream--) | 이미지 스트림을 가져옵니다. |
|
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


문서 키를 가져옵니다.


**Returns:**
java.lang.String - 문서 키.

### getInnerPath() {#getInnerPath--}
```
public final String[] getInnerPath()
```


중첩된 문서의 내부 경로를 가져옵니다.


**Returns:**
java.lang.String[] - 중첩된 문서의 내부 경로.

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


문서 내 이미지의 순번을 가져옵니다.


**Returns:**
int - 문서 내 이미지의 순번.

### getImageFrames() {#getImageFrames--}
```
public final ImageFrame[] getImageFrames()
```


이미지 프레임을 가져옵니다.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - 이미지 프레임.

### getImageStream() {#getImageStream--}
```
public final InputStream getImageStream()
```


이미지 스트림을 가져옵니다.


**Returns:**
java.io.InputStream - 이미지 스트림.

