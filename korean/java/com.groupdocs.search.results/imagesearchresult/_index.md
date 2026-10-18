---
title: "ImageSearchResult"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "역 이미지 검색 결과를 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.search.results/imagesearchresult/
---
**Inheritance:**
java.lang.Object
```
public abstract class ImageSearchResult
```

역 이미지 검색 결과를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ImageSearchResult()](#ImageSearchResult--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getImageCount()](#getImageCount--) | 검색된 이미지 수를 가져옵니다. |
|
|  | [getFoundImage(int index)](#getFoundImage-int-) | 인덱스로 검색된 이미지를 가져옵니다. |
|
### ImageSearchResult() {#ImageSearchResult--}
```
public ImageSearchResult()
```


### getImageCount() {#getImageCount--}
```
public abstract int getImageCount()
```


검색된 이미지 수를 가져옵니다.


**Returns:**
int - 검색된 이미지 수.

### getFoundImage(int index) {#getFoundImage-int-}
```
public abstract FoundImageFrame getFoundImage(int index)
```


인덱스로 검색된 이미지를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 인덱스 | int | 검색된 이미지의 인덱스. |
|

**Returns:**
[FoundImageFrame](../../com.groupdocs.search.results/foundimageframe) - The found image.

