---
title: Highlight
second_title: GroupDocs..NET API 참조 검색
description: 찾은 용어를 강조 표시하여 HTML 형식의 텍스트를 생성합니다.
type: docs
weight: 180
url: /ko/net/groupdocs.search/index/highlight/
---
## Highlight(FoundDocument, Highlighter) {#highlight}

찾은 용어를 강조 표시하여 HTML 형식의 텍스트를 생성합니다.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| document | FoundDocument | 발견된 문서입니다. |
| highlighter | Highlighter | 검색 결과 하이라이터. |

### 예

이 예는 HTML 형식의 텍스트에서 항목을 강조 표시하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// 인덱스 생성
Index index = new Index(indexFolder);

// 지정된 폴더에서 문서 인덱싱
index.Add(documentFolder);

// '영원'이라는 단어 검색
SearchResult result = index.Search("eternity");

// 텍스트에서 강조 표시
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // 처음 찾은 문서 가져오기
    OutputAdapter outputAdapter = new FileOutputAdapter(@"c:\Highlighted.html"); // 파일에 대한 출력 어댑터 생성
    Highlighter highlighter = new HtmlHighlighter(outputAdapter); // 하이라이터 객체 생성
    index.Highlight(document, highlighter); // 강조 표시된 항목이 있는 HTML 형식의 텍스트 생성
}
```

### 또한보십시오

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

---

## Highlight(FoundDocument, Highlighter, HighlightOptions) {#highlight_1}

찾은 용어를 강조 표시하여 HTML 형식의 텍스트를 생성합니다.

```csharp
public void Highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```

| 모수 | 유형 | 설명 |
| --- | --- | --- |
| document | FoundDocument | 발견된 문서입니다. |
| highlighter | Highlighter | 검색 결과 하이라이터. |
| options | HighlightOptions | 하이라이트 옵션. |

### 예

이 예는 HTML 형식의 텍스트에서 항목을 강조 표시하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentFolder = @"c:\MyDocuments\";

// 인덱스 생성
Index index = new Index(indexFolder);

// 지정된 폴더에서 문서 인덱싱
index.Add(documentFolder);

// '영원'이라는 단어 검색
SearchResult result = index.Search("eternity");

// 텍스트에서 강조 표시
if (result.DocumentCount > 0)
{
    FoundDocument document = result.GetFoundDocument(0); // 처음 찾은 문서 가져오기
    OutputAdapter outputAdapter = new FileOutputAdapter(@"c:\Highlighted.html"); // 파일에 대한 출력 어댑터 생성
    Highlighter highlighter = new HtmlHighlighter(outputAdapter); // 하이라이터 객체 생성
    HighlightOptions options = new HighlightOptions(); // 하이라이트 옵션 객체 생성
    options.TermsBefore = 5;
    options.TermsAfter = 5;
    options.TermsTotal = 15;
    index.Highlight(document, highlighter, options); // 강조 표시된 항목이 있는 HTML 형식의 텍스트 생성
}
```

### 또한보십시오

* class [FoundDocument](../../../groupdocs.search.results/founddocument)
* class [Highlighter](../../../groupdocs.search.highlighters/highlighter)
* class [HighlightOptions](../../../groupdocs.search.options/highlightoptions)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->