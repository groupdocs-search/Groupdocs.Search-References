---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "java.io.OutputStream에 출력을 수집하는 출력 어댑터를 나타냅니다."
type: docs
weight: 31
url: /ko/java/com.groupdocs.search.common/streamoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IStreamOutputAdapter](../../com.groupdocs.search.common/istreamoutputadapter)
```
public class StreamOutputAdapter extends OutputAdapter implements IStreamOutputAdapter
```

출력을 java.io.OutputStream에 수집하는 출력 어댑터를 나타냅니다.


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
final ByteArrayOutputStream stream = new ByteArrayOutputStream(); // 출력 스트림을 생성합니다
StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // 스트림 출력 어댑터를 생성합니다
index.getDocumentText(documents[0], adapter); // 스트림에 문서 텍스트를 생성합니다
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)](#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-) | StreamOutputAdapter 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getStream()](#getStream--) | 출력 스트림을 가져옵니다. |
|
### StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream) {#StreamOutputAdapter-com.groupdocs.search.options.OutputFormat-java.io.OutputStream-}
```
public StreamOutputAdapter(OutputFormat outputFormat, OutputStream stream)
```


StreamOutputAdapter 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 출력 형식입니다. |
|
|  | stream | java.io.OutputStream | 출력 스트림입니다. |
|

### getStream() {#getStream--}
```
public final OutputStream getStream()
```


출력 스트림을 가져옵니다.


**Returns:**
java.io.OutputStream - 출력 스트림입니다.

