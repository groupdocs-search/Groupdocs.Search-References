---
title: "SearchImage"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색할 이미지를 나타냅니다."
type: docs
weight: 29
url: /ko/java/com.groupdocs.search.common/searchimage/
---
**Inheritance:**
java.lang.Object
```
public abstract class SearchImage
```

검색할 이미지를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [SearchImage()](#SearchImage--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [create(String filePath)](#create-java.lang.String-) | 검색을 위해 파일에서 이미지를 생성합니다. |
|
|  | [create(String filePath, int imageIndex)](#create-java.lang.String-int-) | 검색을 위해 파일에서 이미지를 생성합니다. |
|
|  | [create(InputStream stream)](#create-java.io.InputStream-) | 검색을 위해 스트림에서 이미지를 생성합니다. |
|
|  | [create(InputStream stream, int imageIndex)](#create-java.io.InputStream-int-) | 검색을 위해 스트림에서 이미지를 생성합니다. |
|
### SearchImage() {#SearchImage--}
```
public SearchImage()
```


### create(String filePath) {#create-java.lang.String-}
```
public static SearchImage create(String filePath)
```


검색을 위해 파일에서 이미지를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 이미지 파일 경로. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(String filePath, int imageIndex) {#create-java.lang.String-int-}
```
public static SearchImage create(String filePath, int imageIndex)
```


검색을 위해 파일에서 이미지를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 이미지 파일 경로. |
|
|  | imageIndex | int | 다중 페이지 이미지에서 이미지 인덱스. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream) {#create-java.io.InputStream-}
```
public static SearchImage create(InputStream stream)
```


검색을 위해 스트림에서 이미지를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 이미지 스트림. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

### create(InputStream stream, int imageIndex) {#create-java.io.InputStream-int-}
```
public static SearchImage create(InputStream stream, int imageIndex)
```


검색을 위해 스트림에서 이미지를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 이미지 스트림. |
|
|  | imageIndex | int | 다중 페이지 이미지에서 이미지 인덱스. |
|

**Returns:**
[SearchImage](../../com.groupdocs.search.common/searchimage) - An image to search.

