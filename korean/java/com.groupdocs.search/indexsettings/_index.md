---
title: "IndexSettings"
second_title: "GroupDocs.Search for Java API 레퍼런스"
description: "인덱싱 작업을 사용자 정의할 수 있게 하는 인덱스 설정을 나타냅니다."
type: docs
weight: 19
url: /ko/java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

인덱싱 작업을 사용자 정의할 수 있게 하는 인덱스 설정을 나타냅니다.


**Learn more**

* [Search index settings](../https://docs.groupdocs.com/display/searchjava/Search+index+settings)


예제는 이 클래스의 일반적인 사용법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex); // 인덱스 유형 설정
Index index = new Index(indexFolder, settings); // 인덱스 생성
 
```
 
````


## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [IndexSettings()](#IndexSettings--) | 새로운  IndexSettings  클래스의 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getInMemoryIndex()](#getInMemoryIndex--) | 인덱스가 메모리 또는 디스크에 저장되는지 여부를 나타내는 값을 가져옵니다. |
|
|  | [getUseStopWords()](#getUseStopWords--) | 불용어를 사용할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | 불용어를 사용할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | 인덱싱 보고서의 최대 개수를 가져옵니다. |
|
|  | [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | 인덱싱 보고서의 최대 개수를 설정합니다. |
|
|  | [getMaxSearchReportCount()](#getMaxSearchReportCount--) | 검색 보고서의 최대 개수를 가져옵니다. |
|
|  | [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | 검색 보고서의 최대 개수를 설정합니다. |
|
|  | [getUseCharacterReplacements()](#getUseCharacterReplacements--) | 문자 교체를 사용할지 여부를 나타내는 값을 가져옵니다. |
|
|  | [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | 문자 교체를 사용할지 여부를 나타내는 값을 설정합니다. |
|
|  | [getDocumentFilter()](#getDocumentFilter--) | 문서 필터를 가져옵니다. |
|
|  | [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | 문서 필터를 설정합니다. |
|
|  | [getTextStorageSettings()](#getTextStorageSettings--) | 텍스트 저장 설정을 가져옵니다. |
|
|  | [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | 텍스트 저장 설정을 설정합니다. |
|
|  | [getIndexType()](#getIndexType--) | 인덱스 유형을 가져옵니다. |
|
|  | [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | 인덱스 유형을 설정합니다. |
|
|  | [getSearchThreads()](#getSearchThreads--) | 검색에 사용되는 스레드 수를 가져옵니다. |
|
|  | [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | 검색에 사용되는 스레드 수를 설정합니다. |
|
|  | [getCustomExtractors()](#getCustomExtractors--) | 사용자 정의 추출기 컬렉션을 가져옵니다. |
|
|  | [getLogger()](#getLogger--) | 인덱스에서 이벤트와 오류를 기록하는 로거를 가져옵니다. |
|
|  | [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | 인덱스에서 이벤트와 오류를 기록하는 로거를 설정합니다. |
|
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


새로운  IndexSettings  클래스의 인스턴스를 초기화합니다.


### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


인덱스가 메모리 또는 디스크에 저장되는지 여부를 나타내는 값을 가져옵니다.


**Returns:**
boolean - 인덱스가 메모리 또는 디스크에 저장되는지를 나타내는 값입니다.

### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


불용어를 사용할지 여부를 나타내는 값을 가져옵니다. 기본값은 true 입니다.


**Returns:**
boolean - 불용어를 사용할지 여부를 나타내는 값입니다.

### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


불용어를 사용할지 여부를 나타내는 값을 설정합니다. 기본값은 true 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 불용어를 사용할지 여부를 나타내는 값입니다. |
|

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


인덱싱 보고서의 최대 개수를 가져옵니다. 기본값은 5 입니다.


**Returns:**
int - 인덱싱 보고서의 최대 개수입니다.

### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


인덱싱 보고서의 최대 개수를 설정합니다. 기본값은 5 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 인덱싱 보고서의 최대 개수입니다. |
|

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


검색 보고서의 최대 개수를 가져옵니다. 기본값은 10 입니다.


**Returns:**
int - 검색 보고서의 최대 개수입니다.

### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


검색 보고서의 최대 개수를 설정합니다. 기본값은 10 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | int | 검색 보고서의 최대 개수입니다. |
|

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


문자 교체를 사용할지 여부를 나타내는 값을 가져옵니다. 기본값은 false 입니다.


**Returns:**
boolean - 문자 교체를 사용할지 여부를 나타내는 값입니다.

### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


문자 교체를 사용할지 여부를 나타내는 값을 설정합니다. 기본값은 false 입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | 값 | boolean | 문자 교체를 사용할지 여부를 나타내는 값입니다. |
|

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


문서 필터를 가져옵니다. DocumentFilter는 포함 로직에서 작동합니다. DocumentFilter 클래스를 사용하여 문서 필터 인스턴스를 생성하십시오. 기본값은 null이며, 이는 추가된 모든 문서가 인덱싱된다는 의미입니다.


**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

예제는 문서 필터를 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 확장자 '.doc', '.docx', '.rtf'를 가진 문서를 건너뛰는 필터를 생성합니다
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // 파일 확장자 필터 생성
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // 파일 확장자 필터 반전
settings.setDocumentFilter(invertedFilter);
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder, settings);
// 문서 인덱싱
index.add(documentsFolder);
// 검색
SearchResult result = index.search("Einstein");
 
```
 
````


### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


문서 필터를 설정합니다. DocumentFilter는 포함 논리에서 작동합니다. DocumentFilter 클래스인 GroupDocs.Search.Options.DocumentFilter를 사용하여 문서 필터 인스턴스를 생성합니다. 기본값은 null이며, 이는 모든 추가된 문서가 인덱싱된다는 의미입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | 문서 필터. |

예제는 문서 필터를 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 확장자 '.doc', '.docx', '.rtf'를 가진 문서를 건너뛰는 필터를 생성합니다
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // 파일 확장자 필터 생성
DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // 파일 확장자 필터 반전
settings.setDocumentFilter(invertedFilter);
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder, settings);
// 문서 인덱싱
index.add(documentsFolder);
// 검색
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


텍스트 저장 설정을 가져옵니다. 기본값은 null이며, 이는 문서 텍스트가 저장되지 않음을 의미합니다.


**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

예제는 텍스트 저장 설정을 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 설정 인스턴스 생성
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // 인덱스 텍스트 저장을 위한 높은 압축 수준 설정
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder, settings);
// 문서 인덱싱
index.add(documentsFolder);
// 검색
SearchResult result = index.search("Einstein");
 
```
 
````


### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


텍스트 저장 설정을 지정합니다. 기본값은 null이며, 이는 문서 텍스트가 저장되지 않음을 의미합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | 텍스트 저장 설정. |

예제는 텍스트 저장 설정을 설정하는 방법을 보여줍니다.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// 인덱스 설정 인스턴스 생성
IndexSettings settings = new IndexSettings();
settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // 인덱스 텍스트 저장을 위한 높은 압축 수준 설정
// 지정된 폴더에 인덱스 생성
Index index = new Index(indexFolder, settings);
// 문서 인덱싱
index.add(documentsFolder);
// 검색
SearchResult result = index.search("Einstein");
 
```
 
````

|

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


인덱스 유형을 가져옵니다. 기본값은 GroupDocs.Search.Options.IndexType.NormalIndex입니다.


**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.

### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


인덱스 유형을 설정합니다. 기본값은 GroupDocs.Search.Options.IndexType.NormalIndex입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [IndexType](../../com.groupdocs.search.options/indextype) | 인덱스 유형. |
|

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


검색에 사용되는 스레드 수를 가져옵니다. 기본값은 GroupDocs.Search.Options.NumberOfThreads.Default이며, 이는 검색이 프로세서 코어 수와 동일한 스레드 수를 사용하여 수행된다는 의미입니다.


**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.

### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


검색에 사용되는 스레드 수를 설정합니다. 기본값은 GroupDocs.Search.Options.NumberOfThreads.Default이며, 이는 검색이 프로세서 코어 수와 동일한 스레드 수를 사용하여 수행된다는 의미입니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | 검색에 사용되는 스레드 수. |
|

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


커스텀 추출기 컬렉션을 가져옵니다. 커스텀 추출기 구현에 대한 전체 예제는 GroupDocs.Search.Common.IFieldExtractor 인터페이스 문서에 제시되어 있습니다.


**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.

### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


인덱스에서 이벤트와 오류를 기록하는 데 사용되는 로거를 가져옵니다. 로거는 저장되지 않으며 인덱스가 생성되거나 로드될 때마다 생성하고 할당해야 합니다.


**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.

### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


인덱스에서 이벤트와 오류를 기록하는 로거를 설정합니다. 로거는 저장되지 않으며 인덱스를 생성하거나 로드할 때마다 생성하고 할당해야 합니다.


**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
|  | value | [ILogger](../../com.groupdocs.search.common/ilogger) | 인덱스에서 이벤트와 오류를 기록하는 로거입니다. |
|

