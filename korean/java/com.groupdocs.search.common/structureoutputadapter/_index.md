---
title: "StructureOutputAdapter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "각 필드를 별도로 포함하는 구조체로 출력을 수집하는 출력 어댑터를 나타냅니다."
type: docs
weight: 33
url: /ko/java/com.groupdocs.search.common/structureoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStructureOutputAdapter](../../com.groupdocs.search.common/istructureoutputadapter)
```
public class StructureOutputAdapter extends OutputAdapter implements IStructureOutputAdapter
```

각 필드를 별도로 포함하는 구조체로 출력을 수집하는 출력 어댑터를 나타냅니다.

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [StructureOutputAdapter(OutputFormat outputFormat)](#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StructureOutputAdapter 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getResult()](#getResult--) | 결과 필드 배열을 가져옵니다. |
|
### StructureOutputAdapter(OutputFormat outputFormat) {#StructureOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StructureOutputAdapter(OutputFormat outputFormat)
```


StructureOutputAdapter 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 출력 형식입니다. |
|

### getResult() {#getResult--}
```
public final DocumentField[] getResult()
```


결과 필드 배열을 가져옵니다.


**Returns:**
com.groupdocs.search.common.DocumentField[] - 결과 필드 배열.

