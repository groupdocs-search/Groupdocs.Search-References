---
title: "Index"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "문서를 인덱싱하고 검색하기 위한 주요 클래스를 나타냅니다."
type: docs
weight: 17
url: /ko/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

문서를 인덱싱하고 검색하기 위한 주요 클래스를 나타냅니다.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchResult result = index.search(query); // 인덱스에서 검색
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [Index()](#Index--) | 메모리에서  Index  클래스의 새 인스턴스를 초기화합니다. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | 특정 인덱스 설정을 사용하여 메모리에서  Index  클래스의 새 인스턴스를 초기화합니다. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Index 클래스의 새 인스턴스를 초기화합니다. |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | 새 인스턴스를 초기화합니다 |
Index
클래스.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | 새 인스턴스를 초기화합니다 |
Index
클래스.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | 새 인스턴스를 초기화합니다 |
Index
클래스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEvents()](#getEvents--) | 이벤트 구독을 위한 이벤트 허브를 가져옵니다. |
|
|  | [getIndexInfo()](#getIndexInfo--) | 인덱스에 대한 기본 정보를 가져옵니다. |
|
|  | [getRepository()](#getRepository--) | 인덱스가 포함된 경우 인덱스 리포지토리 객체를 가져옵니다. |
|
|  | [getIndexSettings()](#getIndexSettings--) | 인덱스 설정을 가져옵니다. |
|
|  | [getDictionaries()](#getDictionaries--) | 사전 리포지토리를 가져옵니다. |
|
|  | [close()](#close--) | 사용되는 모든 리소스를 해제합니다 |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | 인덱싱 작업을 수행합니다. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | 인덱싱 작업을 수행합니다. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | 인덱싱 작업을 수행합니다. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | 인덱싱 작업을 수행합니다. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | 인덱싱 작업을 수행합니다. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | 인덱싱 작업을 수행합니다. |
|
|  | [update()](#update--) | 마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | 마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다. |
|
|  | [getIndexingReports()](#getIndexingReports--) | 인덱싱 작업에 대한 보고서를 가져옵니다. |
|
|  | [getSearchReports()](#getSearchReports--) | 검색 작업에 대한 보고서를 가져옵니다. |
|
|  | [search(String query)](#search-java.lang.String-) | 인덱스에서 검색합니다. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 인덱스에서 검색합니다. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | 인덱스에서 검색합니다. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 인덱스에서 검색합니다. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | 인덱스에서 역 이미지 검색을 수행합니다. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Search 메서드로 시작된 청크 검색을 계속합니다. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Search 메서드로 시작된 청크 검색을 계속합니다. |
|
|  | [optimize()](#optimize--) | 인덱스 세그먼트 수를 서로 병합하여 최소화합니다. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | 인덱스 세그먼트 수를 서로 병합하여 최소화합니다. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | 지정된 인덱스를 현재 인덱스에 병합합니다. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | 지정된 인덱스 저장소의 인덱스를 현재 인덱스로 병합합니다. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | 검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | 검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | 전체 인덱싱된 문서 배열을 가져옵니다. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | 문서 항목 배열을 가져옵니다. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | 문서 키를 사용하여 인덱싱된 문서를 가져옵니다. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | 인덱싱된 문서의 텍스트를 생성하고 출력 어댑터를 통해 전달합니다. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | 인덱싱된 문서에 대한 HTML 형식 텍스트를 생성하고 출력 어댑터를 통해 전송합니다. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | 인덱싱된 경로(문서 또는 폴더) 배열을 가져옵니다. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | 인덱스에서 인덱싱된 파일 또는 폴더를 삭제합니다. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | 스트림 또는 구조에서 인덱싱된 문서를 삭제합니다. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | 지정된 알림 객체를 인덱스로 전달하여 알림을 수행합니다. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | 업데이트 작업 중 재인덱싱 없이 지정된 속성 변경 배치를 인덱싱된 문서에 적용합니다. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | 지정된 인덱싱된 문서와 연결된 모든 속성을 가져옵니다. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | 전체 인덱스를 메모리로 로드합니다. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | 전체 인덱스를 메모리로 로드합니다. |
|
### Index() {#Index--}
```
public Index()
```


메모리에서  Index  클래스의 새 인스턴스를 초기화합니다.


예제는 파일을 디스크에 저장하지 않고 메모리에서 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


특정 인덱스 설정을 사용하여 메모리에서  Index  클래스의 새 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 인덱스 설정 객체. |


예제는 특정 인덱스 설정을 사용하여 파일을 디스크에 저장하지 않고 메모리에서 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


새로운 Index 클래스 인스턴스를 초기화합니다. 새 인덱스를 만들거나 디스크에 있는 기존 인덱스를 엽니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더 경로입니다. |


예제는 디스크에 인덱스를 생성하거나 기존 인덱스를 여는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


새 인스턴스를 초기화합니다
Index
클래스.
특정 설정으로 새 인덱스를 만들거나 디스크에 있는 기존 인덱스를 엽니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더 경로입니다. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 인덱스 설정 객체. |

예제는 특정 인덱스 설정을 사용하여 디스크에 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


새 인스턴스를 초기화합니다
Index
클래스.
디스크에서 기존 인덱스를 로드합니다
overwriteIfExists
은
false
;
그렇지 않으면 디스크에 새 인덱스를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더 경로입니다. |
|
|  | overwriteIfExists | boolean | 인덱스 폴더를 덮어쓰는 플래그입니다. |

예제는 이미 다른 인덱스를 포함하고 있는 폴더에 새 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


새 인스턴스를 초기화합니다
Index
클래스.
디스크에서 기존 인덱스를 로드합니다
overwriteIfExists
은
false
;
그렇지 않으면 특정 인덱스 설정으로 디스크에 새 인덱스를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더 경로입니다. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 인덱스 설정 객체. |
|
|  | overwriteIfExists | boolean | 인덱스 폴더를 덮어쓰는 플래그입니다. |

예제는 특정 인덱스 설정을 사용하여 디스크에 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


이벤트 구독을 위한 이벤트 허브를 가져옵니다.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


인덱스에 대한 기본 정보를 가져옵니다.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


인덱스가 포함된 경우 인덱스 리포지토리 객체를 가져옵니다.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


인덱스 설정을 가져옵니다.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


사전 리포지토리를 가져옵니다.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


사용되는 모든 리소스를 해제합니다
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


인덱싱 작업을 수행합니다.
절대 경로나 상대 경로를 사용하여 파일 또는 폴더를 추가합니다.
모든 하위 폴더의 문서가 인덱싱됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 인덱싱할 파일 또는 폴더의 경로입니다. |

예제는 인덱스에 문서를 추가하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(folderPath); // 지정된 폴더의 문서를 색인합니다
index.add(filePath); // 지정된 문서를 색인합니다
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


인덱싱 작업을 수행합니다.
절대 경로나 상대 경로를 사용하여 파일 또는 폴더를 추가합니다.
모든 하위 폴더의 문서가 인덱싱됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 인덱싱할 파일 또는 폴더의 경로입니다. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 색인 옵션입니다. |

예제는 특정 색인 옵션을 사용하여 문서를 인덱스에 추가하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // 인덱싱 스레드 수 설정
index.add(folderPath, options); // 지정된 폴더의 문서를 색인합니다
index.add(filePath, options); // 지정된 문서를 색인합니다
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


인덱싱 작업을 수행합니다.
절대 경로나 상대 경로를 사용하여 파일 또는 폴더를 추가합니다.
모든 하위 폴더의 문서가 인덱싱됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | paths | java.lang.String[] | 색인할 파일 또는 폴더의 경로입니다. |

예제는 인덱스에 문서를 추가하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // 지정된 경로에 있는 문서를 색인합니다
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


인덱싱 작업을 수행합니다.
절대 경로나 상대 경로를 사용하여 파일 또는 폴더를 추가합니다.
모든 하위 폴더의 문서가 인덱싱됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | paths | java.lang.String[] | 색인할 파일 또는 폴더의 경로입니다. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 색인 옵션입니다. |

예제는 특정 색인 옵션을 사용하여 문서를 인덱스에 추가하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // 인덱싱 스레드 수 설정
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // 지정된 경로에 있는 문서를 색인합니다
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


인덱싱 작업을 수행합니다.
파일 시스템, 스트림 또는 구조에서 문서를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | 파일 시스템, 스트림 또는 구조의 문서입니다. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 색인 옵션입니다. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


인덱싱 작업을 수행합니다.
추출된 데이터를 인덱스에 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | 추출된 데이터입니다. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | 색인 옵션입니다. |
|

### update() {#update--}
```
public final void update()
```


마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다.
인덱싱된 폴더에 추가된 새 파일을 추가합니다.

예제는 인덱스를 업데이트하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
// 문서 폴더에서 문서를 삭제하거나 수정하거나 새 문서를 폴더에 추가합니다
index.update(); // 인덱스를 업데이트합니다
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


마지막 업데이트 이후 변경되거나 삭제된 문서를 다시 인덱싱합니다.
인덱싱된 폴더에 추가된 새 파일을 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 업데이트 옵션. |

예제는 특정 업데이트 옵션을 사용하여 인덱스를 업데이트하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
// 문서 폴더에서 문서를 삭제하거나 수정하거나 새 문서를 폴더에 추가합니다
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // 인덱싱 스레드 수 설정
index.update(options); // 인덱스를 업데이트합니다
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


인덱싱 작업에 대한 보고서를 가져옵니다.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - 색인 보고서입니다.

예제는 색인 보고서를 가져오는 방법을 보여줍니다

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
IndexingReport[] reports = index.getIndexingReports(); // 색인 보고서를 가져옵니다
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


검색 작업에 대한 보고서를 가져옵니다.


**Returns:**
com.groupdocs.search.common.SearchReport[] - 검색 보고서.

예제는 검색 보고서를 가져오는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchResult result1 = index.search(query1); // 검색 중
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // 검색 보고서 가져오기
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


인덱스에서 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | java.lang.String | 검색 쿼리. |

다음 예제는 간단한 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchResult result = index.search(query); // 검색 중
 
```
 
````

다음 예제는 정규식 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
String query = "^[0-9]{3,}"; // 검색 쿼리 시작 부분의 캐럿 기호는 인덱스에 정규식 쿼리임을 알려줍니다.
SearchResult result = index.search(query); // 검색 중
 
```
 
````

다음 예제는 페이싯 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
String query = "content:Newton"; // 쿼리에서 콜론 앞의 단어는 검색할 문서 필드 이름을 의미합니다.
SearchResult result = index.search(query); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


인덱스에서 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | java.lang.String | 검색 쿼리. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |

다음 예제는 퍼지 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // 퍼지 검색 활성화
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // 각 단어에 대한 가능한 차이 수 설정
// 시작과 끝의 큰따옴표는 인덱스에 구문 검색 쿼리임을 알려줍니다
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // 검색 중
 
```
 
````

다음 예제는 동의어 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // 동의어 검색 활성화
String query = "cry";
SearchResult result = index.search(query, options); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


인덱스에서 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 검색 쿼리. |

다음 예제는 객체 형태의 쿼리를 사용하여 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
// 서브쿼리 1 생성
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // subquery 1에만 검색 옵션을 설정합니다
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // 퍼지 검색을 활성화합니다
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // 최대 차이 수를 설정합니다
// subquery 2 생성
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// subquery 3 생성
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// 여러 하위 쿼리를 하나의 쿼리로 결합
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


인덱스에서 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 검색 쿼리. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |

다음 예제는 객체 형태의 쿼리를 사용하여 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
// 날짜 범위 검색의 하위 쿼리 생성
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// 누락된 단어 수가 0에서 2까지인 와일드카드 하위 쿼리 생성
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// 간단한 단어의 하위 쿼리 생성
SearchQuery subquery3 = SearchQuery.createWordQuery(\"birth\");
subquery3.setSearchOptions(new SearchOptions()); // 하위 쿼리 3에만 검색 옵션 설정
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// 여러 하위 쿼리를 하나의 쿼리로 결합
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// 발견된 발생 횟수 용량이 증가된 검색 옵션 객체 생성
SearchOptions options = new SearchOptions(); // 전체 검색 옵션
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


인덱스에서 역 이미지 검색을 수행합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | 검색할 이미지. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | 이미지 검색 옵션. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Search 메서드로 시작된 청크 검색을 계속합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | 청크 검색 토큰. |

예제는 청크 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // 청크 검색을 활성화합니다
SearchResult result = index.search(query, options); // 청크 검색을 시작합니다
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // 청크 검색을 계속합니다
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Search 메서드로 시작된 청크 검색을 계속합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | 청크 검색 토큰. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | 취소 객체. |

예제는 객체 형태의 쿼리를 사용하여 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder); // 지정된 폴더에서 문서 인덱싱
Cancellation cancellation = new Cancellation(); // 이 취소 객체는 취소될 경우 모든 검색 연속을 중단합니다
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // 청크 검색을 활성화합니다
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // 청크 검색을 시작합니다
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // 청크 검색을 계속합니다
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


인덱스 세그먼트 수를 서로 병합하여 최소화합니다.
이 작업은 검색 성능을 향상시킵니다.

예제는 인덱스의 세그먼트를 병합하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder1); // 지정된 폴더에서 문서 색인
index.add(documentsFolder2); // 각 AddToIndex 호출은 인덱스에 최소 하나의 새 세그먼트를 생성합니다
index.add(documentsFolder3);
// 인덱스 세그먼트 병합
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


인덱스 세그먼트 수를 서로 병합하여 최소화합니다.
이 작업은 검색 성능을 향상시킵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | 병합 옵션. |

이 예제는 특정 병합 옵션을 사용하여 인덱스의 세그먼트를 병합하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // 지정된 폴더에 인덱스 생성
index.add(documentsFolder1); // 지정된 폴더에서 문서 색인
index.add(documentsFolder2); // 각 AddToIndex 호출은 인덱스에 최소 하나의 새 세그먼트를 생성합니다
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // 비동기 작업
options.setCancellation(new Cancellation()); // 취소 객체 생성
// 인덱스 세그먼트 병합
index.optimize(options); // 이 메서드는 작업이 완료되기 전에 반환됩니다
options.getCancellation().cancelAfter(10000); // 작업의 최대 지속 시간을 10초로 설정
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


지정된 인덱스를 현재 인덱스에 병합합니다.
다른 인덱스는 변경되지 않을 것임을 유의하십시오.


다른 인덱스에 이전 버전이 있는 경우, 병합하기 전에 업데이트해야 합니다
IndexUpdater
.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | 병합 대상 인덱스. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | 병합 옵션. |

이 예제는 현재 인덱스로 인덱스를 병합하는 방법을 보여줍니다.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // index1 생성
index1.add(documentsFolder1); // 문서 색인
Index index2 = new Index(indexFolder2); // index2 생성
index2.add(documentsFolder2); // 문서 색인
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // 취소 객체 생성
// index2를 index1에 병합합니다. index2 파일은 변경되지 않을 것임을 유의하십시오.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


지정된 인덱스 저장소의 인덱스를 현재 인덱스로 병합합니다.
리포지토리의 인덱스는 변경되지 않을 것임을 참고하세요.


다른 인덱스에 이전 버전이 있는 경우, 병합하기 전에 업데이트해야 합니다.
IndexUpdater
.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | 병합할 대상 인덱스 리포지토리. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | 병합 옵션. |

이 예제는 인덱스 리포지토리를 현재 인덱스로 병합하는 방법을 보여줍니다.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // index1 생성
index1.add(documentsFolder1); // 문서 색인
IndexRepository repository = new IndexRepository(); // 인덱스 리포지토리 생성
Index index2 = repository.create(indexFolder2); // index2 생성
index2.add(documentsFolder2); // 문서 색인
Index index3 = repository.create(indexFolder3); // index3 생성
index3.add(documentsFolder3); // 문서 색인
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // 취소 객체 생성
// 인덱스 리포지토리의 모든 인덱스를 index1에 병합합니다. index2와 index3는 변경되지 않을 것임을 참고하세요.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | 찾은 문서. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 검색 결과 하이라이터. |

이 예제는 HTML 형식 텍스트에서 발생을 강조 표시하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentFolder);
// 'eternity' 단어 검색
SearchResult result = index.search("eternity");
// 텍스트에서 발생 강조
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // 첫 번째 찾은 문서 가져오기
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // 파일에 대한 출력 어댑터 생성
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // 하이라이터 객체를 생성합니다
index.highlight(document, highlighter); // 하이라이트된 발생을 포함한 HTML 형식 텍스트를 생성합니다
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


검색된 용어를 강조 표시한 HTML 형식 텍스트를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | 찾은 문서. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | 검색 결과 하이라이터. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | 하이라이트 옵션입니다. |

이 예제는 HTML 형식 텍스트에서 발생을 강조 표시하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentFolder);
// 'eternity' 단어 검색
SearchResult result = index.search("eternity");
// 텍스트에서 발생 강조
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // 첫 번째 찾은 문서 가져오기
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // 파일에 대한 출력 어댑터 생성
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // 하이라이터 객체를 생성합니다
HighlightOptions options = new HighlightOptions(); // 하이라이트 옵션 객체를 생성합니다
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // 하이라이트된 발생을 포함한 HTML 형식 텍스트를 생성합니다
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


전체 인덱싱된 문서 배열을 가져옵니다.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - 전체 인덱싱된 문서들의 배열.

이 예제는 인덱스에서 인덱싱된 문서 목록을 가져오는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 인덱싱된 문서 목록을 가져오기
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


문서 항목 배열을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | 문서 정보입니다. |

이 예제는 인덱스에서 인덱싱된 문서의 항목 목록을 가져오는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 인덱싱된 문서 목록을 가져오기
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // 문서 항목 목록을 가져옵니다
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - 문서 항목들의 배열.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


문서 키를 사용하여 인덱싱된 문서를 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentKey | java.lang.String | 문서 키입니다. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


인덱싱된 문서의 텍스트를 생성하고 출력 어댑터를 통해 전달합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | 인덱싱된 문서 정보입니다. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 출력 어댑터입니다. |

이 예제는 인덱스에서 인덱싱된 문서의 텍스트를 가져오는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 색인
index.add(documentsFolder);
// 인덱싱된 문서 목록을 가져오기
DocumentInfo[] documents = index.getIndexedDocuments();
// 문서 텍스트 가져오기
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


인덱싱된 문서에 대한 HTML 형식 텍스트를 생성하고 출력 어댑터를 통해 전송합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | 인덱싱된 문서 정보입니다. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | 출력 어댑터입니다. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | 텍스트 검색 옵션. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


인덱싱된 경로(문서 또는 폴더) 배열을 가져옵니다.


**Returns:**
java.lang.String[] - 인덱스된 경로 배열.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


인덱스에서 인덱스된 파일 또는 폴더를 삭제합니다. 그런 다음 삭제된 경로 없이 인덱스를 업데이트합니다.
폴더의 일부로 인덱스에 추가된 경우 개별 문서는 인덱스에서 삭제할 수 없다는 점에 유의하세요.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | paths | java.lang.String[] | 삭제할 파일 또는 폴더의 경로. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 업데이트 옵션. |

예제는 인덱스에서 인덱스된 경로를 삭제하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder);
// 지정된 폴더에서 문서 인덱싱
index.add(documentsFolder1);
index.add(documentsFolder2);
// 인덱스에서 인덱스된 경로 가져오기
String[] indexedPaths1 = index.getIndexedPaths();
// 인덱스된 경로를 콘솔에 출력
System.out.println("인덱스된 경로:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// 인덱스에서 인덱스 경로 삭제
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// 삭제 후 인덱스된 경로 가져오기
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\n삭제된 경로: " + deleteResult.getSuccessCount());
System.out.println("\nIndexed paths:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


스트림 또는 구조에서 인덱싱된 문서를 삭제합니다. 그런 다음 삭제된 문서 없이 인덱스를 업데이트합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 업데이트 옵션. |
|
|  | documentKeys | java.lang.String[] | 스트림 또는 구조에서 추가된 문서의 키입니다. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


지정된 알림 객체를 인덱스로 전달하여 알림을 수행합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | 알림 객체입니다. |
|

**Returns:**
boolean - 알림이 성공적으로 수행되면  true  를 반환하고, 그렇지 않으면  false  를 반환합니다.

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


업데이트 작업 중 재인덱싱 없이 지정된 속성 변경 배치를 인덱싱된 문서에 적용합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | 속성 변경 배치입니다. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


지정된 인덱싱된 문서와 연결된 모든 속성을 가져옵니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | path | java.lang.String | 문서 경로입니다. |
|

**Returns:**
java.lang.String[] - 문서와 연관된 속성입니다.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


전체 인덱스를 메모리로 로드합니다.
인덱스에 대한 모든 변경 사항은 원본 폴더에 자동으로 저장되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더 경로입니다. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


전체 인덱스를 메모리로 로드합니다.
인덱스에 대한 모든 변경 사항은 원본 폴더에 자동으로 저장되지 않습니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더 경로입니다. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 인덱스 설정 객체. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

