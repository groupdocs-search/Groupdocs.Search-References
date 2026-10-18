---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "출력을 파일에 수집하는 출력 어댑터를 나타냅니다."
type: docs
weight: 21
url: /ko/java/com.groupdocs.search.common/fileoutputadapter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.common.OutputAdapter](../../com.groupdocs.search.common/outputadapter)

**All Implemented Interfaces:**
[com.groupdocs.search.common.IFileOutputAdapter](../../com.groupdocs.search.common/ifileoutputadapter)
```
public class FileOutputAdapter extends OutputAdapter implements IFileOutputAdapter
```

출력을 파일에 수집하는 출력 어댑터를 나타냅니다.


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
FileOutputAdapter adapter = new FileOutputAdapter("c:\\DocumentText.htm"); // 파일 출력 어댑터를 생성합니다
index.getDocumentText(documents[0], adapter); // 문서 텍스트를 출력 파일에 생성합니다
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [FileOutputAdapter(OutputFormat outputFormat, String filePath)](#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-) | FileOutputAdapter 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getFilePath()](#getFilePath--) | 출력 파일 경로를 가져옵니다. |
|
### FileOutputAdapter(OutputFormat outputFormat, String filePath) {#FileOutputAdapter-com.groupdocs.search.options.OutputFormat-java.lang.String-}
```
public FileOutputAdapter(OutputFormat outputFormat, String filePath)
```


FileOutputAdapter 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 출력 형식입니다. |
|
|  | filePath | java.lang.String | 출력 파일 경로입니다. |
|

### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


출력 파일 경로를 가져옵니다.


**Returns:**
java.lang.String - 출력 파일 경로입니다.

