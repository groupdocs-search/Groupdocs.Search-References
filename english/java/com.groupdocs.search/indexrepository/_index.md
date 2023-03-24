---
title: IndexRepository
second_title: GroupDocs.Search for Java API Reference
description: Represents a container for combining multiple indexes and performing common operations on them.
type: docs
weight: 19
url: /java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Represents a container for combining multiple indexes and performing common operations on them.

**Learn more**

 *  [Search index repository][]

The example demonstrates a typical usage of the class.

```

 String indexFolder1 = "c:\\MyIndex\\";
 String indexFolder2 = "c:\\MyIndex\\";
 String query = "Einstein";
 IndexRepository repository = new IndexRepository();
 repository.addToRepository(indexFolder1); // Loading an existing index
 repository.addToRepository(indexFolder2); // Loading another existing index
 SearchResult result = repository.search(query); // Searching in indexes of the repository
 
```


[Search index repository]: https://docs.groupdocs.com/display/searchjava/Search+index+repository
## Constructors

| Constructor | Description |
| --- | --- |
| [IndexRepository()](#IndexRepository--) | Initializes a new instance of the  IndexRepository  class. |
## Methods

| Method | Description |
| --- | --- |
| [getEvents()](#getEvents--) | Gets the event hub for subscribing to events. |
| [getIndexes()](#getIndexes--) | Gets the indexes contained in this  IndexRepository . |
| [close()](#close--) | Releases all resources used by the  IndexRepository . |
| [create()](#create--) | Creates a new index in memory. |
| [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Creates a new index in memory. |
| [create(String indexFolder)](#create-java.lang.String-) | Creates a new index on disk. |
| [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Creates a new index on disk. |
| [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Adds an index to the index repository. |
| [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Opens and adds an index to the index repository. |
| [update()](#update--) | Updates all indexes in the repository. |
| [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Updates all indexes in the repository. |
| [search(String query)](#search-java.lang.String-) | Searches in all indexes of the repository. |
| [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Searches in all indexes of the repository. |
| [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Searches in all indexes of the repository. |
| [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Searches in all indexes of the repository. |
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Initializes a new instance of the  IndexRepository  class.

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Gets the event hub for subscribing to events.

**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.
### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Gets the indexes contained in this  IndexRepository .

**Returns:**
com.groupdocs.search.Index[] - The indexes.
### close() {#close--}
```
public final void close()
```


Releases all resources used by the  IndexRepository .

### create() {#create--}
```
public final Index create()
```


Creates a new index in memory.

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

The example demonstrates how to create an index in memory through the index repository.

```

 IndexRepository indexRepository = new IndexRepository();
 Index index = indexRepository.create();
 
```
### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


Creates a new index in memory.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | The index settings.

The example demonstrates how to create an index in memory through the index repository.

```

 IndexRepository indexRepository = new IndexRepository();
 IndexSettings settings = new IndexSettings();
 settings.setUseStopWords(false); // Disabling use of stop words during indexing
 Index index = indexRepository.create(settings);
 
``` |

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.
### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


Creates a new index on disk. The index folder will be cleaned before the index creation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder.

The example demonstrates how to create an index on disk through the index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 IndexRepository indexRepository = new IndexRepository();
 Index index = indexRepository.create(indexFolder);
 
``` |

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.
### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


Creates a new index on disk. The index folder will be cleaned before the index creation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder. |
| settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | The index settings.

The example demonstrates how to create an index on disk through the index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 IndexRepository indexRepository = new IndexRepository();
 IndexSettings settings = new IndexSettings();
 settings.setUseStopWords(false); // Disabling use of stop words during indexing
 Index index = indexRepository.create(indexFolder, settings);
 
``` |

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.
### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


Adds an index to the index repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | [Index](../../com.groupdocs.search/index) | The index to add.

The example demonstrates how to add an index to the index repository.

```

 Index index = new Index();
 IndexRepository indexRepository = new IndexRepository();
 indexRepository.addToRepository(index);
 
``` |

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


Opens and adds an index to the index repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| indexFolder | java.lang.String | The index folder.

The example demonstrates how to add an index to the index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 IndexRepository indexRepository = new IndexRepository();
 indexRepository.addToRepository(indexFolder);
 
``` |

### update() {#update--}
```
public final void update()
```


Updates all indexes in the repository.

The example demonstrates how to update indexes in the repository.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 IndexRepository repository = new IndexRepository();
 Index index = repository.create(indexFolder); // Creating index
 index.add(documentsFolder); // Indexing documents
 // Delete documents from the documents folder or modify them or add new documents to the folder
 repository.update();
 
```

### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Updates all indexes in the repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | The update options.

The example demonstrates how to update indexes in the repository.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 IndexRepository repository = new IndexRepository();
 Index index = repository.create(indexFolder); // Creating index
 index.add(documentsFolder); // Indexing documents
 // Delete documents from the documents folder or modify them or add new documents to the folder
 UpdateOptions options = new UpdateOptions();
 options.setThreads(2); // Setting the number of indexing threads
 repository.update(options);
 
``` |

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Searches in all indexes of the repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | java.lang.String | The search query.

The example demonstrates how to perform search in index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 IndexRepository repository = new IndexRepository();
 Index index = repository.create(indexFolder); // Creating index
 index.add(documentsFolder); // Indexing documents
 SearchResult result = repository.search(query); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Searches in all indexes of the repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | java.lang.String | The search query. |
| options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | The search options.

The example demonstrates how to perform search in index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 IndexRepository repository = new IndexRepository();
 Index index = repository.create(indexFolder); // Creating index
 index.add(documentsFolder); // Indexing documents
 SearchOptions options = new SearchOptions();
 options.setUseCaseSensitiveSearch(true); // Setting flag of case sensitive search
 SearchResult result = repository.search(query, options); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Searches in all indexes of the repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The search query.

The example demonstrates how to perform search in index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 IndexRepository repository = new IndexRepository();
 Index index = repository.create(indexFolder); // Creating index
 index.add(documentsFolder); // Indexing documents
 SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Creating search query in object form
 SearchResult result = repository.search(query); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Searches in all indexes of the repository.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| query | [SearchQuery](../../com.groupdocs.search/searchquery) | The search query. |
| options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | The search options.

The example demonstrates how to perform search in index repository.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 IndexRepository repository = new IndexRepository();
 Index index = repository.create(indexFolder); // Creating index
 index.add(documentsFolder); // Indexing documents
 SearchOptions options = new SearchOptions();
 options.setUseCaseSensitiveSearch(true); // Setting flag of case sensitive search
 SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Creating search query in object form
 SearchResult result = repository.search(query, options); // Searching
 
``` |

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.
