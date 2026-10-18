---
title: "ExtractedItemInfo"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "컨테이너 항목 정보를 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

컨테이너 항목 정보를 나타냅니다.


**Learn more**

* [Custom text extractors](../https://docs.groupdocs.com/display/searchjava/Custom+text+extractors)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | ExtractedItemInfo 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFormatFamily()](#getFormatFamily--) | 문서 유형을 가져옵니다. |
|
|  | [getFields()](#getFields--) | 추출된 필드를 가져옵니다. |
|
|  | [getItemInfo()](#getItemInfo--) | 항목 정보를 가져옵니다. |
|
|  | [getInnerPath()](#getInnerPath--) | 내부 경로를 가져옵니다. |
|
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


ExtractedItemInfo 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | 문서 형식 패밀리입니다. |
|
|  | fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | 추출된 필드입니다. |
|
|  | itemInfo | java.lang.String | 항목 정보입니다. |
|
|  | innerPath | java.lang.String | 컨테이너 내 항목에 대한 경로입니다. |
|

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


문서 유형을 가져옵니다.


**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.

### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


추출된 필드를 가져옵니다.


**Returns:**
com.groupdocs.search.common.DocumentField[] - 추출된 필드입니다.

### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


항목 정보를 가져옵니다.


**Returns:**
java.lang.String - 항목 정보입니다.

### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


내부 경로를 가져옵니다.


**Returns:**
java.lang.String - 내부 경로입니다.

