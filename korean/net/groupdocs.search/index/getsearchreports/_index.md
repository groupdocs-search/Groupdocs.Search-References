---
title: GetSearchReports
second_title: GroupDocs..NET API 참조 검색
description: 검색 작업에 대한 보고서를 가져옵니다.
type: docs
weight: 170
url: /ko/net/groupdocs.search/index/getsearchreports/
---
## Index.GetSearchReports method

검색 작업에 대한 보고서를 가져옵니다.

```csharp
public SearchReport[] GetSearchReports()
```

### 반환 값

검색 보고서입니다.

### 예

이 예는 검색 보고서를 얻는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query1 = "Einstein";
string query2 = "Newton";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

SearchResult result1 = index.Search(query1); // 검색 중
SearchResult result2 = index.Search(query2);
SearchResult result3 = index.Search(query1 + " & " + query2);

SearchReport[] reports = index.GetSearchReports(); // 검색 보고서 가져오기
```

### 또한보십시오

* class [SearchReport](../../../groupdocs.search.common/searchreport)
* class [Index](../../index)
* 네임스페이스 [GroupDocs.Search](../../index)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->