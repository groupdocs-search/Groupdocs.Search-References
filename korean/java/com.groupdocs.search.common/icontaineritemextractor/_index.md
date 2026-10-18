---
title: "IContainerItemExtractor"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "컨테이너 문서에서 항목을 추출하는 메서드를 제공합니다."
type: docs
weight: 35
url: /ko/java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

컨테이너 문서에서 항목을 추출하는 메서드를 제공합니다.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | 문서 형식 패밀리를 가져옵니다. |
|
|  | [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | 컨테이너 문서에서 항목을 추출합니다. |
|
|  | [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | 컨테이너 문서에서 항목을 추출합니다. |
|
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


문서 형식 패밀리를 가져옵니다.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.

### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


컨테이너 문서에서 항목을 추출합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | filePath | java.lang.String | 파일 경로. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - 추출된 항목들의 배열.

### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


컨테이너 문서에서 항목을 추출합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | stream | java.io.InputStream | 문서 스트림입니다. |
|

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - 추출된 항목들의 배열.

