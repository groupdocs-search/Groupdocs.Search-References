---
title: DocumentFilter
second_title: GroupDocs..NET API 참조 검색
description: 문서 필터를 가져오거나 설정합니다. DocumentFiltergroupdocs.search/indexsettings/documentfilter 포함 논리에서 작동합니다. 사용DocumentFiltergroupdocs.search.options/documentfilter 문서 필터 인스턴스 생성을 위한 클래스. 기본값은없는  추가된 모든 문서가 인덱싱됨을 의미합니다.
type: docs
weight: 40
url: /ko/net/groupdocs.search/indexsettings/documentfilter/
---
## IndexSettings.DocumentFilter property

문서 필터를 가져오거나 설정합니다. `DocumentFilter` 포함 논리에서 작동합니다. 사용[`DocumentFilter`](../../../groupdocs.search.options/documentfilter) 문서 필터 인스턴스 생성을 위한 클래스. 기본값은`없는` , 추가된 모든 문서가 인덱싱됨을 의미합니다.

```csharp
public DocumentFilter DocumentFilter { get; set; }
```

### 자산 가치

문서 필터.

### 예

이 예는 문서 필터를 설정하는 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// 확장자가 '.doc', '.docx', '.rtf'인 문서를 건너뛰는 필터 생성
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // 파일 확장자 필터 생성
DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter); // 파일 확장자 필터 반전
settings.DocumentFilter = invertedFilter;

// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder, settings);

// 문서 인덱싱
index.Add(documentsFolder);

// 검색 중
SearchResult result = index.Search("Einstein");
```

### 또한보십시오

* class [DocumentFilter](../../../groupdocs.search.options/documentfilter)
* class [IndexSettings](../../indexsettings)
* 네임스페이스 [GroupDocs.Search](../../indexsettings)
* 집회 [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->