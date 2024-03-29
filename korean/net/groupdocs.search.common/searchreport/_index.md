---
title: SearchReport
second_title: GroupDocs..NET API 참조 검색
description: 검색 동작에 대한 상세 정보를 나타냅니다.
type: docs
weight: 290
url: /ko/net/groupdocs.search.common/searchreport/
---
## SearchReport class

검색 동작에 대한 상세 정보를 나타냅니다.

```csharp
public class SearchReport
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [DocumentCount](../../groupdocs.search.common/searchreport/documentcount) { get; } | 찾은 문서 수를 가져옵니다. |
| [EndTime](../../groupdocs.search.common/searchreport/endtime) { get; } | 검색 종료 시간을 가져옵니다. |
| [ObjectQuery](../../groupdocs.search.common/searchreport/objectquery) { get; } | 개체 형태로 검색 쿼리를 가져옵니다. |
| [OccurrenceCount](../../groupdocs.search.common/searchreport/occurrencecount) { get; } | 발견된 총 발생 수를 가져옵니다. |
| [SearchDuration](../../groupdocs.search.common/searchreport/searchduration) { get; } | 검색 기간을 가져옵니다. |
| [SearchOptions](../../groupdocs.search.common/searchreport/searchoptions) { get; } | 검색 옵션을 가져옵니다. |
| [StartTime](../../groupdocs.search.common/searchreport/starttime) { get; } | 검색 시작 시간을 가져옵니다. |
| [TextQuery](../../groupdocs.search.common/searchreport/textquery) { get; } | 검색 쿼리를 텍스트 형식으로 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| override [ToString](../../groupdocs.search.common/searchreport/tostring)() | 반환String 현재를 나타내는[`SearchReport`](../searchreport) . |

### 비고

**더 알아보기**

* [보고서 검색](https://docs.groupdocs.com/display/searchnet/Search+reports)

### 예

이 예제는 클래스의 일반적인 사용법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);

// 지정된 폴더에서 문서 인덱싱
index.Add(documentsFolder);

// 인덱스에서 검색
SearchResult result1 = index.Search("Einstein");
SearchResult result2 = index.Search("\"Theory of Relativity\"");

// 검색 보고서 가져오기
SearchReport[] reports = index.GetSearchReports();

// 콘솔에 보고서 출력
foreach (SearchReport report in reports)
{
    Console.WriteLine("Query: " + report.TextQuery);
    Console.WriteLine("Time: " + report.StartTime);
    Console.WriteLine("Duration: " + report.SearchDuration);
    Console.WriteLine("Documents: " + report.DocumentCount);
    Console.WriteLine("Occurrences: " + report.OccurrenceCount);
    Console.WriteLine();
}
```

### 또한보십시오

* 네임스페이스 [GroupDocs.Search.Common](../../groupdocs.search.common)
* 집회 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
