---
title: "IndexRepository"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "여러 인덱스를 결합하고 공통 작업을 수행하기 위한 컨테이너를 나타냅니다."
type: docs
weight: 18
url: /ko/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

여러 인덱스를 결합하고 공통 작업을 수행하기 위한 컨테이너를 나타냅니다.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // 기존 인덱스를 로드합니다
repository.addToRepository(indexFolder2); // 또 다른 기존 인덱스를 로드합니다
SearchResult result = repository.search(query); // 저장소의 인덱스를 검색합니다
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | 새 인스턴스를 초기화합니다 |
IndexRepository
클래스.
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getEvents()](#getEvents--) | 이벤트 구독을 위한 이벤트 허브를 가져옵니다. |
|
|  | [getIndexes()](#getIndexes--) | 이 객체에 포함된 인덱스를 가져옵니다 |
IndexRepository
.
|
|  | [close()](#close--) | 사용되는 모든 리소스를 해제합니다 |
IndexRepository
.
|
|  | [create()](#create--) | 메모리에서 새 인덱스를 생성합니다. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | 메모리에서 새 인덱스를 생성합니다. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | 디스크에 새 인덱스를 생성합니다. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | 디스크에 새 인덱스를 생성합니다. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | 인덱스 저장소에 인덱스를 추가합니다. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | 인덱스 저장소를 열고 인덱스를 추가합니다. |
|
|  | [update()](#update--) | 저장소의 모든 인덱스를 업데이트합니다. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | 저장소의 모든 인덱스를 업데이트합니다. |
|
|  | [search(String query)](#search-java.lang.String-) | 저장소의 모든 인덱스를 검색합니다. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | 저장소의 모든 인덱스를 검색합니다. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | 저장소의 모든 인덱스를 검색합니다. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | 저장소의 모든 인덱스를 검색합니다. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


새 인스턴스를 초기화합니다
IndexRepository
클래스.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


이벤트 구독을 위한 이벤트 허브를 가져옵니다.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


이 객체에 포함된 인덱스를 가져옵니다
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - 인덱스들.

### close() {#close--}
```
public final void close()
```


사용되는 모든 리소스를 해제합니다
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


메모리에서 새 인덱스를 생성합니다.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

예제에서는 인덱스 저장소를 통해 메모리에서 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


메모리에서 새 인덱스를 생성합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 인덱스 설정. |

예제에서는 인덱스 저장소를 통해 메모리에서 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // 인덱싱 중 불용어 사용을 비활성화합니다
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


디스크에 새 인덱스를 생성합니다.
인덱스 생성 전에 인덱스 폴더가 정리됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더. |

예제에서는 인덱스 저장소를 통해 디스크에 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


디스크에 새 인덱스를 생성합니다.
인덱스 생성 전에 인덱스 폴더가 정리됩니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | 인덱스 설정. |

예제에서는 인덱스 저장소를 통해 디스크에 인덱스를 생성하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // 인덱싱 중 불용어 사용을 비활성화합니다
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


인덱스 저장소에 인덱스를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | 추가할 인덱스. |

예제에서는 인덱스 저장소에 인덱스를 추가하는 방법을 보여줍니다.

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


인덱스 저장소를 열고 인덱스를 추가합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | indexFolder | java.lang.String | 인덱스 폴더. |

예제에서는 인덱스 저장소에 인덱스를 추가하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


저장소의 모든 인덱스를 업데이트합니다.

이 예제는 저장소에서 인덱스를 업데이트하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 인덱스 생성
index.add(documentsFolder); // 문서 인덱싱
// 문서 폴더에서 문서를 삭제하거나 수정하거나 새 문서를 폴더에 추가합니다
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


저장소의 모든 인덱스를 업데이트합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | 업데이트 옵션. |

이 예제는 저장소에서 인덱스를 업데이트하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 인덱스 생성
index.add(documentsFolder); // 문서 인덱싱
// 문서 폴더에서 문서를 삭제하거나 수정하거나 새 문서를 폴더에 추가합니다
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // 인덱싱 스레드 수 설정
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


저장소의 모든 인덱스를 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | java.lang.String | 검색 쿼리. |

이 예제는 인덱스 저장소에서 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 인덱스 생성
index.add(documentsFolder); // 문서 인덱싱
SearchResult result = repository.search(query); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


저장소의 모든 인덱스를 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | java.lang.String | 검색 쿼리. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |

이 예제는 인덱스 저장소에서 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 인덱스 생성
index.add(documentsFolder); // 문서 인덱싱
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // 대소문자 구분 검색 플래그 설정
SearchResult result = repository.search(query, options); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


저장소의 모든 인덱스를 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 검색 쿼리. |

이 예제는 인덱스 저장소에서 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 인덱스 생성
index.add(documentsFolder); // 문서 인덱싱
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // 객체 형태로 검색 쿼리 생성
SearchResult result = repository.search(query); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


저장소의 모든 인덱스를 검색합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | 검색 쿼리. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | 검색 옵션. |

이 예제는 인덱스 저장소에서 검색을 수행하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // 인덱스 생성
index.add(documentsFolder); // 문서 인덱싱
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // 대소문자 구분 검색 플래그 설정
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // 객체 형태로 검색 쿼리 생성
SearchResult result = repository.search(query, options); // 검색 중
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

