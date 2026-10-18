---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "출력을 System.String으로 수집하는 출력 어댑터를 나타냅니다."
type: docs
weight: 32
url: /ko/java/com.groupdocs.search.common/stringoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStringOutputAdapter](../../com.groupdocs.search.common/istringoutputadapter)
```
public class StringOutputAdapter extends OutputAdapter implements IStringOutputAdapter
```

출력을 System.String으로 수집하는 출력 어댑터를 나타냅니다.


**Learn more**

* [Output adapters](../https://docs.groupdocs.com/display/searchjava/Output+adapters)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스를 생성합니다.
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
DocumentInfo[] documents = index.getIndexedDocuments(); // 인덱싱된 문서에 대한 정보를 가져옵니다
StringOutputAdapter adapter = new StringOutputAdapter(); // 문자열 출력 어댑터 생성
index.getDocumentText(documents[0], adapter); // 어댑터에 문서 텍스트 생성
String result = adapter.getResult(); // 결과 가져오기
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [StringOutputAdapter(OutputFormat outputFormat)](#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-) | StringOutputAdapter 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getResult()](#getResult--) | 결과 문자열을 가져옵니다. |
|
### StringOutputAdapter(OutputFormat outputFormat) {#StringOutputAdapter-com.groupdocs.search.options.OutputFormat-}
```
public StringOutputAdapter(OutputFormat outputFormat)
```


StringOutputAdapter 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 출력 형식입니다. |
|

### getResult() {#getResult--}
```
public final String getResult()
```


결과 문자열을 가져옵니다.


**Returns:**
java.lang.String - 결과 문자열.

