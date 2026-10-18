---
title: "DocumentHighlighter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "전체 문서 텍스트에서 검색 결과를 강조 표시하는 검색 결과 하이라이터를 나타냅니다."
type: docs
weight: 10
url: /ko/java/com.groupdocs.search.highlighters/documenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IDocumentHighlighter](../../com.groupdocs.search.highlighters/idocumenthighlighter)
```
public class DocumentHighlighter extends Highlighter implements IDocumentHighlighter
```

전체 문서 텍스트에서 검색 결과를 강조 표시하는 검색 결과 하이라이터를 나타냅니다.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 'Theory of Relativity' 구문 검색
SearchResult result = index.search("\"Theory of Relativity\"");
// 문서 텍스트에서 찾은 단어 강조
FoundDocument document = result.getFoundDocument(0);
OutputAdapter outputAdapter = new FileOutputAdapter(OutputFormat.Html, "Highlighted.html");
Highlighter highlighter = new DocumentHighlighter(outputAdapter);
index.highlight(document, highlighter);
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [DocumentHighlighter(OutputAdapter outputAdapter)](#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-) | DocumentHighlighter 클래스의 새 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getOutputAdapter()](#getOutputAdapter--) | 생성자에 전달된 출력 어댑터를 가져옵니다. |
|
### DocumentHighlighter(OutputAdapter outputAdapter) {#DocumentHighlighter-com.groupdocs.search.common.OutputAdapter-}
```
public DocumentHighlighter(OutputAdapter outputAdapter)
```


DocumentHighlighter 클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputAdapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 하이라이팅 결과를 전달하는 출력 어댑터. |
|

### getOutputAdapter() {#getOutputAdapter--}
```
public final OutputAdapter getOutputAdapter()
```


생성자에 전달된 출력 어댑터를 가져옵니다.


**Returns:**
[OutputAdapter](../../com.groupdocs.search.common/outputadapter) - The output adapter passed in the constructor.

