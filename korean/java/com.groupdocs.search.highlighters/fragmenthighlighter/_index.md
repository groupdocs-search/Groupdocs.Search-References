---
title: "FragmentHighlighter"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "텍스트 조각에서 검색 결과를 강조 표시하는 검색 결과 하이라이터를 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.groupdocs.search.highlighters/fragmenthighlighter/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.ResultBuilderFactory](../../com.groupdocs.search.common/resultbuilderfactory), [com.groupdocs.search.highlighters.Highlighter](../../com.groupdocs.search.highlighters/highlighter)

**All Implemented Interfaces:**
[com.groupdocs.search.highlighters.IFragmentHighlighter](../../com.groupdocs.search.highlighters/ifragmenthighlighter)
```
public class FragmentHighlighter extends Highlighter implements IFragmentHighlighter
```

텍스트 조각에서 검색 결과를 강조 표시하는 검색 결과 하이라이터를 나타냅니다.


**Learn more**

* [Highlighting search results](../https://docs.groupdocs.com/display/searchjava/Highlighting+search+results)

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 'Einstein' 단어 검색
SearchResult result = index.search("Einstein");
// 하이라이트 옵션 할당
HighlightOptions options = new HighlightOptions();
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
// 문서 텍스트에서 찾은 단어 강조
FoundDocument document = result.getFoundDocument(0);
FragmentHighlighter highlighter = new FragmentHighlighter(OutputFormat.Html);
index.highlight(document, highlighter, options);
// 결과 가져오기
FragmentContainer[] fragmentContainers = highlighter.getResult();
for (int i = 0; i < fragmentContainers.length; i++) {
FragmentContainer container = fragmentContainers[i];
String[] fragments = container.getFragments();
if (fragments.length > 0) {
System.out.println(container.getFieldName());
System.out.println();
for (int j = 0; j < fragments.length; j++) {
// 콘솔에 HTML 마크업을 출력합니다
System.out.println(fragments[j]);
System.out.println();
}
}
}
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [FragmentHighlighter(OutputFormat outputFormat)](#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-) | 새로운  FragmentHighlighter  클래스의 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getResult()](#getResult--) | 결과 fragment containers의 배열을 가져옵니다. |
|
### FragmentHighlighter(OutputFormat outputFormat) {#FragmentHighlighter-com.groupdocs.search.options.OutputFormat-}
```
public FragmentHighlighter(OutputFormat outputFormat)
```


새로운  FragmentHighlighter  클래스의 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | outputFormat | [OutputFormat](../../com.groupdocs.search.options/outputformat) | 출력 형식입니다. |
|

### getResult() {#getResult--}
```
public final FragmentContainer[] getResult()
```


결과 fragment containers의 배열을 가져옵니다.


**Returns:**
com.groupdocs.search.common.FragmentContainer[] - 결과 fragment containers의 배열.

