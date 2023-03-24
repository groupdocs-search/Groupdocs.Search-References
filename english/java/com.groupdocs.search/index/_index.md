---
title: Index
second_title: GroupDocs.Search for Java API Reference
description: Represents the main class for indexing documents and search through them.
type: docs
weight: 18
url: /java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Represents the main class for indexing documents and search through them.

**Learn more**

 *  [Creating an index][]
 *  [Indexing][]
 *  [Searching][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchResult result = index.search(query); // Searching in index
 
```


[Creating an index]: https://docs.groupdocs.com/display/searchjava/Creating+an+index
[Indexing]: https://docs.groupdocs.com/display/searchjava/Indexing
[Searching]: https://docs.groupdocs.com/display/searchjava/Searching
## Constructors

| Constructor | Description |
| --- | --- |
| [Index()](#Index--) | Initializes a new instance of the  Index  class in memory. |
| [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Initializes a new instance of the  Index  class in memory with particular index settings. |
| [Index(String indexFolder)](#Index-java.lang.String-) | Initializes a new instance of the  Index  class. |
| [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Initializes a new instance of the  Index  class. |
| [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Initializes a new instance of the  Index  class. |
| [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Initializes a new instance of the  Index  class. |
## Methods

| Method | Description |
| --- | --- |
| [getEvents()](#getEvents--) | Gets the event hub for subscribing to events. |
| [getIndexInfo()](#getIndexInfo--) | Gets the basic information on the index. |
| [getRepository()](#getRepository--) | Gets the index repository object if the index is contained in it. |
| [getIndexSettings()](#getIndexSettings--) | Gets the index settings. |
| [getDictionaries()](#getDictionaries--) | Gets the dictionary repository. |
| [close()](#close--) | Releases all resources used by the  Index . |
| [add(String path)](#add-java.lang.String-) | Performs indexing operation. |
| [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Performs indexing operation. |
| [add(String[] paths)](#add-java.lang.String---) | Performs indexing operation. |
| [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Performs indexing operation. |
| [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Performs indexing operation. |
| [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Performs indexing operation. |
| [update()](#update--) | Re-indexes documents that have been changed or deleted since last update. |
| [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Re-indexes documents that have been changed or deleted since last update. |
| [getIndexingReports()](#getIndexingReports--) | Gets the reports on indexing operations. |
| [getSearchReports()](#getSearchReports--) | Gets the reports on search operations. |
| [search(String query)](#search-java.lang.String-) | Searches in index. |
| [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Searches in index. |
| [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Searches in index. |
| [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Searches in index. |
| [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Performs a reverse image search in the index. |
| [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Continues the chunk search started with method Search. |
| [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Continues the chunk search started with method Search. |
| [optimize()](#optimize--) | Minimizes the number of index segments by merging them one with another. |
| [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Minimizes the number of index segments by merging them one with another. |
| [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Merges the specified index into the current index. |
| [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Merges indexes from the specified index repository into the current index. |
| [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Generates HTML formatted text with highlighted found terms. |
| [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Generates HTML formatted text with highlighted found terms. |
| [getIndexedDocuments()](#getIndexedDocuments--) | Gets an array of all indexed documents. |
| [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Gets an array of a document items. |
| [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Generates HTML formatted text for indexed document and transfers it through the output adapter. |
| [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Generates HTML formatted text for indexed document and transfers it through the output adapter. |
| [getIndexedPaths()](#getIndexedPaths--) | Gets an array of indexed paths - documents or folders. |
| [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Deletes indexed files or folders from the index. |
| [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Deletes documents indexed from streams or structures. |
| [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Passes the specified notification object to the index to perform the notification. |
| [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Applies the specified batch of attribute changes to indexed documents without reindexing during the update operation. |
| [getAttributes(String path)](#getAttributes-java.lang.String-) | Gets all the attributes associated with the specified indexed document. |
### Index() {#Index--}
```
public Index()
```


Initializes a new instance of the  Index  class in memory.

The example demonstrates how to create index in memory without saving files to disk.

```

 Index index = new Index();
 
```

### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Initializes a new instance of the  Index  class in memory with particular index settings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | The index settings object.

The example demonstrates how to create index in memory without saving files to disk with particular index settings.

```

 IndexSettings settings = new IndexSettings();
 settings.setIndexType(IndexType.CompactIndex);
 Index index = new Index(settings);
 
``` |

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Initializes a new instance of the  Index  class. Creates a new or opens an existing index on disk.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder path.

The example demonstrates how to create an index on a disk or open an existing index.

```

 String indexFolder = "c:\\MyIndex\\";
 Index index = new Index(indexFolder);
 
``` |

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Initializes a new instance of the  Index  class. Creates a new index with particular settings or opens an existing index on disk.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder path. |
| settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | The index settings object.

The example demonstrates how to create an index on a disk with particular index settings.

```

 String indexFolder = "c:\\MyIndex\\";
 IndexSettings settings = new IndexSettings();
 settings.setIndexType(IndexType.CompactIndex);
 Index index = new Index(indexFolder, settings);
 
``` |

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Initializes a new instance of the  Index  class. Loads an existing index from disk if  overwriteIfExists  is  false ; creates a new index on disk otherwise.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder path. |
| overwriteIfExists | boolean | The flag of overwriting the index folder.

The example demonstrates how to create a new index in a folder that already contains another index.

```

 String indexFolder = "c:\\MyIndex\\";
 Index index = new Index(indexFolder, true);
 
``` |

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Initializes a new instance of the  Index  class. Loads an existing index from disk if  overwriteIfExists  is  false ; creates a new index on disk with particular index settings otherwise.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder path. |
| settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | The index settings object. |
| overwriteIfExists | boolean | The flag of overwriting the index folder.

The example demonstrates how to create an index on a disk with particular index settings.

```

 String indexFolder = "c:\\MyIndex\\";
 IndexSettings settings = new IndexSettings();
 settings.setIndexType(IndexType.CompactIndex);
 Index index = new Index(indexFolder, settings, true);
 
``` |

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Gets the event hub for subscribing to events.

**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.
### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Gets the basic information on the index.

**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.
### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Gets the index repository object if the index is contained in it.

**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.
### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Gets the index settings.

**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.
### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Gets the dictionary repository.

**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.
### close() {#close--}
```
public final void close()
```


Releases all resources used by the  Index .

### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to a file or folder to be indexed.

The example demonstrates how to add documents to an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String folderPath = "c:\\MyDocuments\\";
 String filePath = "c:\\Documents\\MyFile.txt";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(folderPath); // Indexing documents in the specified folder
 index.add(filePath); // Indexing the specified document
 
``` |

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Performs indexing operation. Adds a file or folder by an absolute or relative path. Documents from all subfolders will be indexed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The path to a file or folder to be indexed. |
| options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | The indexing options.

The example demonstrates how to add documents to an index with particular indexing options.

```

 String indexFolder = "c:\\MyIndex\\";
 String folderPath = "c:\\MyDocuments\\";
 String filePath = "c:\\Documents\\MyFile.txt";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 IndexingOptions options = new IndexingOptions();
 options.setThreads(2); // Setting the number of indexing threads
 index.add(folderPath, options); // Indexing documents in the specified folder
 index.add(filePath, options); // Indexing the specified document
 
``` |

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| paths | java.lang.String[] | The paths to a files or folders to be indexed.

The example demonstrates how to add documents to an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String folderPath = "c:\\MyDocuments\\";
 String filePath = "c:\\Documents\\MyFile.txt";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 String[] paths = new String[] { folderPath, filePath };
 index.add(paths); // Indexing documents at the specified paths
 
``` |

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Performs indexing operation. Adds files or folders by an absolute or relative path. Documents from all subfolders will be indexed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| paths | java.lang.String[] | The paths to a files or folders to be indexed. |
| options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | The indexing options.

The example demonstrates how to add documents to an index with particular indexing options.

```

 String indexFolder = "c:\\MyIndex\\";
 String folderPath = "c:\\MyDocuments\\";
 String filePath = "c:\\Documents\\MyFile.txt";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 IndexingOptions options = new IndexingOptions();
 options.setThreads(2); // Setting the number of indexing threads
 String[] paths = new String[] { folderPath, filePath };
 index.add(paths, options); // Indexing documents at the specified paths
 
``` |

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Performs indexing operation. Adds documents from file system, stream or structure.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documents | [Document\[\]](../../com.groupdocs.search/document) | The documents from file system, stream or structure. |
| options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | The indexing options. |

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Performs indexing operation. Adds the extracted data to the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | The extracted data. |
| options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | The indexing options. |

### update() {#update--}
```
public final void update()
```


Re-indexes documents that have been changed or deleted since last update. Adds new files that have been added to the indexed folders.

The example demonstrates how to update an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 // Delete documents from the documents folder or modify them or add new documents to the folder
 index.update(); // Updating the index
 
```

### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Re-indexes documents that have been changed or deleted since last update. Adds new files that have been added to the indexed folders.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | The update options.

The example demonstrates how to update an index with particular update options.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 // Delete documents from the documents folder or modify them or add new documents to the folder
 UpdateOptions options = new UpdateOptions();
 options.setThreads(2); // Setting the number of indexing threads
 index.update(options); // Updating the index
 
``` |

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Gets the reports on indexing operations.

**Returns:**
com.groupdocs.search.common.IndexingReport[] - The indexing reports.

The example demonstrates how to get indexing reports.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 IndexingReport[] reports = index.getIndexingReports(); // Getting indexing reports
 
```
### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Gets the reports on search operations.

**Returns:**
com.groupdocs.search.common.SearchReport[] - The search reports.

The example demonstrates how to get search reports.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query1 = "Einstein";
 String query2 = "Newton";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchResult result1 = index.search(query1); // Searching
 SearchResult result2 = index.search(query2);
 SearchResult result3 = index.search(query1 + " & " + query2);
 SearchReport[] reports = index.getSearchReports(); // Getting search reports
 
```
### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Searches in index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | java.lang.String | The search query.

The following example demonstrates how to perform simple search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchResult result = index.search(query); // Searching
 
```

The following example demonstrates how to perform Regex search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 String query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
 SearchResult result = index.search(query); // Searching
 
```

The following example demonstrates how to perform faceted search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 String query = "content:Newton"; // The word before the colon in the query means the document field name to search
 SearchResult result = index.search(query); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Searches in index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | java.lang.String | The search query. |
| options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | The search options.

The following example demonstrates how to perform fuzzy search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.getFuzzySearch().setEnabled(true); // Enabling the fuzzy search
 options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Setting the number of possible differences for each word
 // Double quotes at the beginning and end tells the index that it is phrase search query
 String query = "\"The Pursuit of Happiness\"";
 SearchResult result = index.search(query, options); // Searching
 
```

The following example demonstrates how to perform synonym search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.setUseSynonymSearch(true); // Enabling the synonym search
 String query = "cry";
 SearchResult result = index.search(query, options); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Searches in index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The search query.

The following example demonstrates how to perform search using query in object form.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 // Creating subquery 1
 SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
 subquery1.setSearchOptions(new SearchOptions()); // Setting search options only for subquery 1
 subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Enabling the fuzzy search
 subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Setting maximum number of differences
 // Creating subquery 2
 SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
 // Creating subquery 3
 SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
 // Combining subqueries into one query
 SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 SearchResult result = index.search(query); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Searches in index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The search query. |
| options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | The search options.

The following example demonstrates how to perform search using query in object form.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 // Creating subquery of date range search
 SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
 // Creating subquery of wildcard with number of missed words from 0 to 2
 SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
 // Creating subquery of simple word
 SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
 subquery3.setSearchOptions(new SearchOptions()); // Setting search options only for subquery 3
 subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
 subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
 // Combining subqueries into one query
 SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
 // Creating search options object with increased capacity of found occurrences
 SearchOptions options = new SearchOptions(); // Overall search options
 options.setMaxOccurrenceCountPerTerm(1000000);
 options.setMaxTotalOccurrenceCount(10000000);
 SearchResult result = index.search(query, options); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Performs a reverse image search in the index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| image | [SearchImage](../../com.groupdocs.search.common/searchimage) | The image to search. |
| options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | The image search options. |

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.
### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Continues the chunk search started with method Search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | The chunk search token.

The example demonstrates how to perform chunk search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.setChunkSearch(true); // Enabling chunk search
 SearchResult result = index.search(query, options); // Starting chunk search
 System.out.println("Document count: " + result.getDocumentCount());
 System.out.println("Occurrence count: " + result.getOccurrenceCount());
 while (result.getNextChunkSearchToken() != null) {
     result = index.searchNext(result.getNextChunkSearchToken()); // Continuing chunk search
     System.out.println("Document count: " + result.getDocumentCount());
     System.out.println("Occurrence count: " + result.getOccurrenceCount());
 }
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Continues the chunk search started with method Search.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | The chunk search token. |
| cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | The cancellation object.

The example demonstrates how to perform search using query in object form.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 Cancellation cancellation = new Cancellation(); // This cancellation object aborts all search continuations if canceled
 SearchOptions options = new SearchOptions();
 options.setChunkSearch(true); // Enabling chunk search
 options.setCancellation(cancellation);
 SearchResult result = index.search(query, options); // Starting chunk search
 System.out.println("Document count: " + result.getDocumentCount());
 System.out.println("Occurrence count: " + result.getOccurrenceCount());
 while (result.getNextChunkSearchToken() != null) {
     result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Continuing chunk search
     System.out.println("Document count: " + result.getDocumentCount());
     System.out.println("Occurrence count: " + result.getOccurrenceCount());
 }
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### optimize() {#optimize--}
```
public final void optimize()
```


Minimizes the number of index segments by merging them one with another. This operation improves search performance.

The example demonstrates how to merge segments of an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder1 = "c:\\MyDocuments1\\";
 String documentsFolder2 = "c:\\MyDocuments2\\";
 String documentsFolder3 = "c:\\MyDocuments3\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder1); // Indexing documents from the specified folder
 index.add(documentsFolder2); // Each call to AddToIndex creates at least one new segment in the index
 index.add(documentsFolder3);
 // Merging segments of the index
 index.optimize();
 
```

### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Minimizes the number of index segments by merging them one with another. This operation improves search performance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | The merge options.

The example demonstrates how to merge segments of an index with particular merge options.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder1 = "c:\\MyDocuments1\\";
 String documentsFolder2 = "c:\\MyDocuments2\\";
 String documentsFolder3 = "c:\\MyDocuments3\\";
 Index index = new Index(indexFolder); // Creating index in the specified folder
 index.add(documentsFolder1); // Indexing documents from the specified folder
 index.add(documentsFolder2); // Each call to AddToIndex creates at least one new segment in the index
 index.add(documentsFolder3);
 MergeOptions options = new MergeOptions();
 options.setAsync(true); // Asynchronous operation
 options.setCancellation(new Cancellation()); // Creating cancellation object
 // Merging segments of the index
 index.optimize(options); // This method will return before the operation is completed
 options.getCancellation().cancelAfter(10000); // Setting maximum duration of the operation to 10 seconds
 
``` |

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Merges the specified index into the current index. Note that the other index will not be changed.

If the other index has a previous version, it must be updated before merging with  IndexUpdater .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | [Index](../../com.groupdocs.search/index) | The index to merge into. |
| options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | The merge options.

The example demonstrates how to merge an index into the current index.

```

 String indexFolder1 = "c:\\MyIndex1\\";
 String indexFolder2 = "c:\\MyIndex2\\";
 String documentsFolder1 = "c:\\MyDocuments1\\";
 String documentsFolder2 = "c:\\MyDocuments2\\";
 Index index1 = new Index(indexFolder1); // Creating index1
 index1.add(documentsFolder1); // Indexing documents
 Index index2 = new Index(indexFolder2); // Creating index2
 index2.add(documentsFolder2); // Indexing documents
 MergeOptions options = new MergeOptions();
 options.setCancellation(new Cancellation()); // Creating cancellation object
 // Merging index2 into index1. Note that index2 files will not be changed.
 index1.merge(index2, options);
 
``` |

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Merges indexes from the specified index repository into the current index. Note that indexes in the repository will not be changed.

If other indexes have a previous version, they must be updated before merging with  IndexUpdater .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | The index repository to merge into. |
| options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | The merge options.

The example demonstrates how to merge an index repository into the current index.

```

 String indexFolder1 = "c:\\MyIndex1\\";
 String indexFolder2 = "c:\\MyIndex2\\";
 String indexFolder3 = "c:\\MyIndex3\\";
 String documentsFolder1 = "c:\\MyDocuments1\\";
 String documentsFolder2 = "c:\\MyDocuments2\\";
 String documentsFolder3 = "c:\\MyDocuments3\\";
 Index index1 = new Index(indexFolder1); // Creating index1
 index1.add(documentsFolder1); // Indexing documents
 IndexRepository repository = new IndexRepository(); // Creating index repository
 Index index2 = repository.create(indexFolder2); // Creating index2
 index2.add(documentsFolder2); // Indexing documents
 Index index3 = repository.create(indexFolder3); // Creating index3
 index3.add(documentsFolder3); // Indexing documents
 MergeOptions options = new MergeOptions();
 options.setCancellation(new Cancellation()); // Creating cancellation object
 // Merging all indexes in the index repository into index1. Note that index2 and index3 will not be changed.
 index1.merge(repository, options);
 
``` |

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Generates HTML formatted text with highlighted found terms.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | The found document. |
| highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | The search result highlighter.

The example demonstrates how to highlight occurrences in HTML formatted text.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentFolder);
 // Search for the word 'eternity'
 SearchResult result = index.search("eternity");
 // Highlighting occurrences in text
 if (result.getDocumentCount() > 0) {
     FoundDocument document = result.getFoundDocument(0); // Getting the first found document
     OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Creating an output adapter to the file
     Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creating the highlighter object
     index.highlight(document, highlighter); // Generating HTML formatted text with highlighted occurrences
 }
 
``` |

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Generates HTML formatted text with highlighted found terms.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | The found document. |
| highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | The search result highlighter. |
| options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | The highlight options.

The example demonstrates how to highlight occurrences in HTML formatted text.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentFolder = "c:\\MyDocuments\\";
 // Creating an index
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentFolder);
 // Search for the word 'eternity'
 SearchResult result = index.search("eternity");
 // Highlighting occurrences in text
 if (result.getDocumentCount() > 0) {
     FoundDocument document = result.getFoundDocument(0); // Getting the first found document
     OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Creating an output adapter to the file
     Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Creating the highlighter object
     HighlightOptions options = new HighlightOptions(); // Creating the highlight options object
     options.setTermsBefore(5);
     options.setTermsAfter(5);
     options.setTermsTotal(15);
     index.highlight(document, highlighter, options); // Generating HTML formatted text with highlighted occurrences
 }
 
``` |

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Gets an array of all indexed documents.

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - An array of all indexed documents.

The example demonstrates how to get a list of indexed documents from an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Getting list of indexed documents
 DocumentInfo[] documents = index.getIndexedDocuments();
 
```
### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Gets an array of a document items.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | A document info.

The example demonstrates how to get a list of items of an indexed document from an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Getting list of indexed documents
 DocumentInfo[] documents = index.getIndexedDocuments();
 for (int i = 0; i < documents.length; i++) {
     DocumentInfo document = documents[i];
     System.out.println(document.getFilePath());
     DocumentInfo[] items = index.getIndexedDocumentItems(document); // Getting list of document items
     for (int j = 0; j < items.length; j++) {
         DocumentInfo item = items[j];
         System.out.println("\t" + item.getInnerPath());
     }
 }
 
``` |

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - An array of a document items.
### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Generates HTML formatted text for indexed document and transfers it through the output adapter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | The indexed document info. |
| adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | The output adapter.

The example demonstrates how to get the text of an indexed document from an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folder
 index.add(documentsFolder);
 // Getting list of indexed documents
 DocumentInfo[] documents = index.getIndexedDocuments();
 // Getting a document text
 if (documents.length > 0) {
     FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
     index.getDocumentText(documents[0], outputAdapter);
 }
 
``` |

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Generates HTML formatted text for indexed document and transfers it through the output adapter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | The indexed document info. |
| adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | The output adapter. |
| options | [TextOptions](../../com.groupdocs.search.options/textoptions) | The text retrieving options. |

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Gets an array of indexed paths - documents or folders.

**Returns:**
java.lang.String[] - An array of indexed paths.
### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Deletes indexed files or folders from the index. Then updates the index without deleted paths. Note that an individual document cannot be deleted from the index if it was added to the index as part of a folder.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| paths | java.lang.String[] | The paths to files or folders to delete. |
| options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | The update options.

The example demonstrates how to delete indexed paths from an index.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder1 = "c:\\MyDocuments\\";
 String documentsFolder2 = "c:\\MyDocuments2\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents from the specified folders
 index.add(documentsFolder1);
 index.add(documentsFolder2);
 // Getting indexed paths from the index
 String[] indexedPaths1 = index.getIndexedPaths();
 // Writing indexed paths to the console
 System.out.println("Indexed paths:");
 for (String path : indexedPaths1) {
     System.out.println("\t" + path);
 }
 // Deleting index path from the index
 DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
 // Getting indexed paths after deletion
 String[] indexedPaths2 = index.getIndexedPaths();
 System.out.println("\nDeleted paths: " + deleteResult.getSuccessCount());
 System.out.println("\nIndexed paths:");
 for (String path : indexedPaths2) {
     System.out.println("\t" + path);
 }
 
``` |

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.
### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Deletes documents indexed from streams or structures. Then updates the index without deleted documents.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | The update options. |
| documentKeys | java.lang.String[] | The keys of documents added from streams or structures. |

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.
### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Passes the specified notification object to the index to perform the notification.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| notification | [Notification](../../com.groupdocs.search/notification) | The notification object. |

**Returns:**
boolean - Returns  true  if the notification was successfully performed; otherwise  false .
### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Applies the specified batch of attribute changes to indexed documents without reindexing during the update operation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | The attribute change batch. |

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Gets all the attributes associated with the specified indexed document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| path | java.lang.String | The document path. |

**Returns:**
java.lang.String[] - Attributes associated with the document.
