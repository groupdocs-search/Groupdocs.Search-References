---
title: "ExtractorSettings"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서 데이터 추출기 설정을 포함합니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

문서 데이터 추출기 설정을 포함합니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getIndexType()](#getIndexType--) | 추출기에 사용되는 인덱스 유형을 가져옵니다. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | 추출기에 사용되는 인덱스 유형을 설정합니다. |
|
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


추출기에 사용되는 인덱스 유형을 가져옵니다. 기본값은 GroupDocs.Search.Options.IndexType.NormalIndex 입니다.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


추출기에 사용되는 인덱스 유형을 설정합니다. 기본값은 GroupDocs.Search.Options.IndexType.NormalIndex 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | 추출기에 사용되는 인덱스 유형. |
|

