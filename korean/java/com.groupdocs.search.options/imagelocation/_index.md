---
title: "ImageLocation"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "이미지 위치를 지정합니다."
type: docs
weight: 48
url: /ko/java/com.groupdocs.search.options/imagelocation/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ImageLocation extends Enum<ImageLocation>
```

이미지 위치를 지정합니다.

## 필드

| 필드 | 설명 |
| --- | --- |
|  | [Separate](#Separate) | 별도 파일에 있는 이미지. |
|
|  | [Embedded](#Embedded) | 다른 문서에 삽입된 이미지. |
|
|  | [ContainerItem](#ContainerItem) | 컨테이너 파일의 요소인 이미지. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Separate {#Separate}
```
public static final ImageLocation Separate
```


별도 파일에 있는 이미지.


### Embedded {#Embedded}
```
public static final ImageLocation Embedded
```


다른 문서에 삽입된 이미지.


### ContainerItem {#ContainerItem}
```
public static final ImageLocation ContainerItem
```


컨테이너 파일의 요소인 이미지.


### values() {#values--}
```
public static ImageLocation[] values()
```




**Returns:**
com.groupdocs.search.options.ImageLocation[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ImageLocation valueOf(String name)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ImageLocation](../../com.groupdocs.search.options/imagelocation)
