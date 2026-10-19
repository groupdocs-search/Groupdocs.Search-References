---
title: "Index"
second_title: "GroupDocs.Search 용 .NET API Reference"
description: "문서를 인덱싱하고 검색하는 주요 클래스를 나타냅니다."
type: docs
weight: 700
url: /ko/net/groupdocs.search/index/
---
## Index class

문서를 인덱싱하고 검색하는 주요 클래스를 나타냅니다.

```csharp
public class Index : IDisposable
```

## Constructors

| 이름 | 설명 |
| --- | --- |
| [Index](index#constructor)() | 메모리에서 [`Index`](../index) 클래스의 새 인스턴스를 초기화합니다. |
| [Index](index#constructor_1)(IndexSettings) | 특정 인덱스 설정을 사용하여 메모리에서 [`Index`](../index) 클래스의 새 인스턴스를 초기화합니다. |
| [Index](index#constructor_2)(string) | `[`Index`](../index)` 클래스의 새 인스턴스를 초기화합니다. 디스크에 새 인덱스를 만들거나 기존 인덱스를 엽니다. |
| [Index](index#constructor_3)(string, bool) | `[`Index`](../index)` 클래스의 새 인스턴스를 초기화합니다. *overwriteIfExists* 가 `false`이면 디스크에서 기존 인덱스를 로드하고; 그렇지 않으면 디스크에 새 인덱스를 생성합니다. |
| [Index](index#constructor_4)(string, IndexSettings) | `[`Index`](../index)` 클래스의 새 인스턴스를 초기화합니다. 특정 설정으로 새 인덱스를 생성하거나 디스크에 있는 기존 인덱스를 엽니다. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | `[`Index`](../index)` 클래스의 새 인스턴스를 초기화합니다. *overwriteIfExists* 가 `false`이면 디스크에서 기존 인덱스를 로드하고; 그렇지 않으면 특정 인덱스 설정으로 디스크에 새 인덱스를 생성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | 사전 저장소를 가져옵니다. |
| [Events](../../groupdocs.search/index/events) { get; } | 이벤트 구독을 위한 이벤트 허브를 가져옵니다. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | 인덱스에 대한 기본 정보를 가져옵니다. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | 인덱스 설정을 가져옵니다. |
| [Repository](../../groupdocs.search/index/repository) { get; } | 인덱스가 포함된 경우 인덱스 저장소 객체를 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | 전체 인덱스를 메모리로 로드합니다. 인덱스에 대한 변경 사항은 원본 폴더에 자동으로 저장되지 않습니다. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | 전체 인덱스를 메모리로 로드합니다. 인덱스에 대한 변경 사항은 원본 폴더에 자동으로 저장되지 않습니다. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | 인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | 인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더들을 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | 인덱싱 작업을 수행합니다. 파일 시스템, 스트림 또는 구조에서 문서를 추가합니다. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | 인덱싱 작업을 수행합니다. 추출된 데이터를 인덱스에 추가합니다. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | 인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | 인덱싱 작업을 수행합니다. 절대 경로나 상대 경로로 파일 또는 폴더들을 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | 업데이트 작업 중 재인덱싱 없이 지정된 속성 변경 배치를 인덱싱된 문서에 적용합니다. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | 디스크에서 손상된 세그먼트 파일이 있는지 인덱스를 검사합니다. *fixIndexFunctionality* 가 `true`이면 손상된 세그먼트가 있을 때 인덱스 기능을 복구하고, 그렇지 않으면 복구하지 않습니다. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | 인덱스에서 인덱싱된 파일 또는 폴더를 삭제합니다. 그런 다음 삭제된 경로 없이 인덱스를 업데이트합니다. 폴더의 일부로 인덱스에 추가된 경우 개별 문서는 인덱스에서 삭제할 수 없다는 점에 유의하십시오. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | 스트림 또는 구조에서 인덱싱된 문서를 삭제합니다. 그런 다음 삭제된 문서 없이 인덱스를 업데이트합니다. |
| [Dispose](../../groupdocs.search/index/dispose)() | `[`Index`](../index)` 에서 사용된 모든 리소스를 해제합니다. |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | 지정된 인덱싱된 문서와 연결된 모든 속성을 가져옵니다. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | 인덱싱된 문서의 텍스트를 생성하고 출력 어댑터를 통해 전달합니다. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | 인덱싱된 문서에 대한 HTML 형식 텍스트를 생성하고 출력 어댑터를 통해 전송합니다. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | 문서 키를 사용하여 인덱싱된 문서를 가져옵니다. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | 지정된 문서의 중첩 항목 배열을 가져옵니다 (ZIP, OST, PST와 같은 컨테이너 문서용). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | 전체 인덱싱된 문서의 배열을 가져옵니다. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | 인덱싱된 경로(문서 또는 폴더)의 배열을 가져옵니다. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | 인덱싱 작업에 대한 보고서를 가져옵니다. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | 검색 작업에 대한 보고서를 가져옵니다. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | 검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | 검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | 지정된 인덱스를 현재 인덱스에 병합합니다. 다른 인덱스는 변경되지 않습니다. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | 지정된 인덱스 저장소의 인덱스를 현재 인덱스로 병합합니다. 저장소의 인덱스는 변경되지 않습니다. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | 지정된 알림 객체를 인덱스로 전달하여 알림을 수행합니다. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | 인덱스 세그먼트를 서로 병합하여 수를 최소화합니다. 이 작업은 검색 성능을 향상시킵니다. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | 인덱스 세그먼트를 서로 병합하여 수를 최소화합니다. 이 작업은 검색 성능을 향상시킵니다. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | 메모리 내 인덱스를 디스크에 저장합니다. 또한 일반 인덱스를 다른 폴더에 저장합니다. 이 인덱스의 설정은 변경되지 않습니다. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | 인덱스를 검색합니다. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | 인덱스를 검색합니다. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | 인덱스에서 역 이미지 검색을 수행합니다. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | 인덱스를 검색합니다. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | 인덱스를 검색합니다. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Search 메서드로 시작된 청크 검색을 계속합니다. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Search 메서드로 시작된 청크 검색을 계속합니다. |
| [Update](../../groupdocs.search/index/update#update)() | 마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다. 인덱싱된 폴더에 추가된 새 파일을 추가합니다. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | 마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다. 인덱싱된 폴더에 추가된 새 파일을 추가합니다. |

### 비고

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### 예제

이 예제는 클래스의 일반적인 사용 방법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### 또 보기

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
