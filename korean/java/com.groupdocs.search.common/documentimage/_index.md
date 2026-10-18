---
title: "DocumentImage"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 이미지 데이터를 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.search.common/documentimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentImage
```

문서 이미지 데이터를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentImage()](#DocumentImage--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getImageIndex()](#getImageIndex--) | 문서 내 이미지의 순번을 가져옵니다. |
|
|  | [getFields()](#getFields--) | 추출된 필드를 가져옵니다. |
|
|  | [getFrames()](#getFrames--) | 이미지 프레임을 가져옵니다. |
|
### DocumentImage() {#DocumentImage--}
```
public DocumentImage()
```


### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


문서 내 이미지의 순번을 가져옵니다.


**Returns:**
int - 문서 내 이미지의 순번.

### getFields() {#getFields--}
```
public abstract DocumentField[] getFields()
```


추출된 필드를 가져옵니다.


**Returns:**
com.groupdocs.search.common.DocumentField[] - 추출된 필드입니다.

### getFrames() {#getFrames--}
```
public abstract ImageFrame[] getFrames()
```


이미지 프레임을 가져옵니다.


**Returns:**
com.groupdocs.search.common.ImageFrame[] - 이미지 프레임.

