---
title: "FoundImageFrame"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "검색된 이미지 프레임을 나타냅니다."
type: docs
weight: 16
url: /ko/java/com.groupdocs.search.results/foundimageframe/
---
**Inheritance:**
java.lang.Object
```
public abstract class FoundImageFrame
```

검색된 이미지 프레임을 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FoundImageFrame()](#FoundImageFrame--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getDocumentInfo()](#getDocumentInfo--) | 문서 정보를 가져옵니다. |
|
|  | [getImageIndex()](#getImageIndex--) | 문서 내 이미지의 순번을 가져옵니다. |
|
|  | [getFrameIndex()](#getFrameIndex--) | 이미지에서 프레임의 인덱스를 가져옵니다. |
|
|  | [getHashDifferences()](#getHashDifferences--) | 이미지 해시에서 일치하지 않는 비트 수를 가져옵니다. |
|
|  | [toString()](#toString--) | 현재 FoundImageFrame을 나타내는 System.String을 반환합니다. |
|
### FoundImageFrame() {#FoundImageFrame--}
```
public FoundImageFrame()
```


### getDocumentInfo() {#getDocumentInfo--}
```
public abstract DocumentInfo getDocumentInfo()
```


문서 정보를 가져옵니다.


**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The document info.

### getImageIndex() {#getImageIndex--}
```
public abstract int getImageIndex()
```


문서 내 이미지의 순번을 가져옵니다.


**Returns:**
int - 문서 내 이미지의 순번.

### getFrameIndex() {#getFrameIndex--}
```
public abstract int getFrameIndex()
```


이미지에서 프레임의 인덱스를 가져옵니다.


**Returns:**
int - 이미지에서 프레임의 인덱스.

### getHashDifferences() {#getHashDifferences--}
```
public abstract int getHashDifferences()
```


이미지 해시에서 일치하지 않는 비트 수를 가져옵니다.


**Returns:**
int - 이미지 해시에서 일치하지 않는 비트 수.

### toString() {#toString--}
```
public abstract String toString()
```


현재 FoundImageFrame을 나타내는 System.String을 반환합니다.


**Returns:**
java.lang.String - 현재 FoundImageFrame을 나타내는 System.String.

