---
title: Index
second_title: GroupDocs..NET API 참조 검색
description: 문서를 인덱싱하고 검색하는 기본 클래스를 나타냅니다.
type: docs
weight: 680
url: /ko/net/groupdocs.search/index/
---
## Index class

문서를 인덱싱하고 검색하는 기본 클래스를 나타냅니다.

```csharp
public class Index : IDisposable
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [Index](index#constructor)() | 의 새 인스턴스를 초기화합니다.[`Index`](../index) 메모리의 클래스. |
| [Index](index#constructor_1)(IndexSettings) | 의 새 인스턴스를 초기화합니다.[`Index`](../index) 특정 인덱스 설정이 있는 메모리의 클래스. |
| [Index](index#constructor_2)(string) | 의 새 인스턴스를 초기화합니다.[`Index`](../index) class. 디스크에 새 인덱스를 생성하거나 기존 인덱스를 엽니다. |
| [Index](index#constructor_3)(string, bool) | 의 새 인스턴스를 초기화합니다.[`Index`](../index) class. 다음과 같은 경우 디스크에서 기존 인덱스를 로드합니다.*overwriteIfExists* ~이다`거짓`; 그렇지 않으면 디스크에 새 인덱스를 생성합니다. |
| [Index](index#constructor_4)(string, IndexSettings) | 의 새 인스턴스를 초기화합니다.[`Index`](../index) class. 특정 설정으로 새 인덱스를 생성하거나 디스크의 기존 인덱스를 엽니다. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | 의 새 인스턴스를 초기화합니다.[`Index`](../index) class. 다음과 같은 경우 디스크에서 기존 인덱스를 로드합니다.*overwriteIfExists* ~이다`거짓` ; 그렇지 않으면 특정 색인 설정으로 디스크에 새 색인을 생성합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | 사전 리포지토리를 가져옵니다. |
| [Events](../../groupdocs.search/index/events) { get; } | 이벤트를 구독하기 위한 이벤트 허브를 가져옵니다. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | 인덱스에 대한 기본 정보를 가져옵니다. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | 인덱스 설정을 가져옵니다. |
| [Repository](../../groupdocs.search/index/repository) { get; } | 인덱스가 포함된 경우 인덱스 리포지토리 개체를 가져옵니다. |

## 행동 양식

| 이름 | 설명 |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | 인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | 인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | 인덱싱 작업을 수행합니다. 파일 시스템, 스트림 또는 구조에서 문서를 추가합니다. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | 인덱싱 작업을 수행합니다. 추출된 데이터를 인덱스에 추가합니다. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | 인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | 인덱싱 작업을 수행합니다. 절대 또는 상대 경로로 파일 또는 폴더를 추가합니다. 모든 하위 폴더의 문서가 인덱싱됩니다. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | 업데이트 작업 중에 다시 인덱싱하지 않고 지정된 속성 변경 사항 배치를 인덱싱된 문서에 적용합니다. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | 색인에서 색인화된 파일 또는 폴더를 삭제합니다. 그런 다음 삭제된 경로 없이 인덱스를 업데이트합니다. 폴더의 일부로 인덱스에 추가된 개별 문서는 인덱스에서 삭제할 수 없습니다. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | 스트림 또는 구조에서 인덱싱된 문서를 삭제합니다. 그런 다음 삭제된 문서 없이 인덱스를 업데이트합니다. |
| [Dispose](../../groupdocs.search/index/dispose)() | 에서 사용하는 모든 리소스를 해제합니다.[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | 지정된 색인 문서와 관련된 모든 속성을 가져옵니다. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | 인덱싱된 문서에 대한 HTML 형식의 텍스트를 생성하고 출력 어댑터를 통해 전송합니다. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | 인덱싱된 문서에 대한 HTML 형식의 텍스트를 생성하고 출력 어댑터를 통해 전송합니다. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | 지정된 문서의 중첩 항목 배열을 가져옵니다(ZIP, OST, PST와 같은 컨테이너 문서의 경우). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | 인덱싱된 모든 문서의 배열을 가져옵니다. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | 인덱싱된 경로(문서 또는 폴더)의 배열을 가져옵니다. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | 인덱싱 작업에 대한 보고서를 가져옵니다. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | 검색 작업에 대한 보고서를 가져옵니다. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | 찾은 용어를 강조 표시하여 HTML 형식의 텍스트를 생성합니다. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | 찾은 용어를 강조 표시하여 HTML 형식의 텍스트를 생성합니다. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | 지정된 인덱스를 현재 인덱스에 병합합니다. 다른 인덱스는 변경되지 않습니다. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | 지정된 인덱스 저장소의 인덱스를 현재 인덱스로 병합합니다. 저장소의 인덱스는 변경되지 않습니다. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | 지정된 알림 개체를 인덱스에 전달하여 알림을 수행합니다. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | 인덱스 세그먼트를 병합하여 인덱스 세그먼트 수를 최소화합니다. 이 작업은 검색 성능을 향상시킵니다. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | 인덱스 세그먼트를 병합하여 인덱스 세그먼트 수를 최소화합니다. 이 작업은 검색 성능을 향상시킵니다. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | 인덱스에서 검색합니다. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | 인덱스에서 검색합니다. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | 인덱스에서 역방향 이미지 검색을 수행합니다. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | 인덱스에서 검색합니다. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | 인덱스에서 검색합니다. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Search. 메서드로 시작된 청크 검색을 계속합니다. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Search. 메서드로 시작된 청크 검색을 계속합니다. |
| [Update](../../groupdocs.search/index/update#update)() | 마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다. 인덱싱된 폴더에 추가된 새 파일을 추가합니다. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | 마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다. 인덱싱된 폴더에 추가된 새 파일을 추가합니다. |

### 비고

**더 알아보기**

* [인덱스 생성](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [인덱싱](https://docs.groupdocs.com/display/searchnet/Indexing)
* [수색](https://docs.groupdocs.com/display/searchnet/Searching)

### 예

이 예제는 클래스의 일반적인 사용법을 보여줍니다.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.Add(documentsFolder); // 지정된 폴더에서 문서 인덱싱

SearchResult result = index.Search(query); // 인덱스에서 검색
```

### 또한보십시오

* 네임스페이스 [GroupDocs.Search](../../groupdocs.search)
* 집회 [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
