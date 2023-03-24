---
title: IndexSettings
second_title: GroupDocs.Search for Java API Reference
description: Represents the index settings that allow to customize the indexing operations.
type: docs
weight: 20
url: /java/com.groupdocs.search/indexsettings/
---
**Inheritance:**
java.lang.Object
```
public class IndexSettings
```

Represents the index settings that allow to customize the indexing operations.

**Learn more**

 *  [Search index settings][]

The example demonstrates a typical usage of the class.

```

 String indexFolder = "c:\\MyIndex\\";
 IndexSettings settings = new IndexSettings();
 settings.setIndexType(IndexType.CompactIndex); // Setting the index type
 Index index = new Index(indexFolder, settings); // Creating an index
 
```


[Search index settings]: https://docs.groupdocs.com/display/searchjava/Search+index+settings
## Constructors

| Constructor | Description |
| --- | --- |
| [IndexSettings()](#IndexSettings--) | Initializes a new instance of the  IndexSettings  class. |
## Methods

| Method | Description |
| --- | --- |
| [getInMemoryIndex()](#getInMemoryIndex--) | Gets a value indicating whether the index is stored in memory or on disk. |
| [getUseStopWords()](#getUseStopWords--) | Gets a value indicating whether to use stop words or not. |
| [setUseStopWords(boolean value)](#setUseStopWords-boolean-) | Sets a value indicating whether to use stop words or not. |
| [getMaxIndexingReportCount()](#getMaxIndexingReportCount--) | Gets the maximum number of indexing reports. |
| [setMaxIndexingReportCount(int value)](#setMaxIndexingReportCount-int-) | Sets the maximum number of indexing reports. |
| [getMaxSearchReportCount()](#getMaxSearchReportCount--) | Gets the maximum number of search reports. |
| [setMaxSearchReportCount(int value)](#setMaxSearchReportCount-int-) | Sets the maximum number of search reports. |
| [getUseCharacterReplacements()](#getUseCharacterReplacements--) | Gets a value indicating whether to use character replacements or not. |
| [setUseCharacterReplacements(boolean value)](#setUseCharacterReplacements-boolean-) | Sets a value indicating whether to use character replacements or not. |
| [getAutoDetectEncoding()](#getAutoDetectEncoding--) | Gets a value indicating whether to detect encoding automatically or not. |
| [setAutoDetectEncoding(boolean value)](#setAutoDetectEncoding-boolean-) | Sets a value indicating whether to detect encoding automatically or not. |
| [getUseRawTextExtraction()](#getUseRawTextExtraction--) | Gets a value indicating whether the raw mode is used for text extraction if possible. |
| [setUseRawTextExtraction(boolean value)](#setUseRawTextExtraction-boolean-) | Sets a value indicating whether the raw mode is used for text extraction if possible. |
| [getDocumentFilter()](#getDocumentFilter--) | Gets a document filter. |
| [setDocumentFilter(DocumentFilter value)](#setDocumentFilter-com.groupdocs.search.DocumentFilter-) | Sets a document filter. |
| [getTextStorageSettings()](#getTextStorageSettings--) | Gets the text storage settings. |
| [setTextStorageSettings(TextStorageSettings value)](#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-) | Sets the text storage settings. |
| [getIndexType()](#getIndexType--) | Gets the index type. |
| [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Sets the index type. |
| [getSearchThreads()](#getSearchThreads--) | Gets the number of threads used for the search. |
| [setSearchThreads(NumberOfThreads value)](#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-) | Sets the number of threads used for the search. |
| [getCustomExtractors()](#getCustomExtractors--) | Gets the custom extractor collection. |
| [getLogger()](#getLogger--) | Gets a logger that is used for logging events and errors in the index. |
| [setLogger(ILogger value)](#setLogger-com.groupdocs.search.common.ILogger-) | Sets a logger that is used for logging events and errors in the index. |
### IndexSettings() {#IndexSettings--}
```
public IndexSettings()
```


Initializes a new instance of the  IndexSettings  class.

### getInMemoryIndex() {#getInMemoryIndex--}
```
public final boolean getInMemoryIndex()
```


Gets a value indicating whether the index is stored in memory or on disk.

**Returns:**
boolean - A value indicating whether the index is stored in memory or on disk.
### getUseStopWords() {#getUseStopWords--}
```
public final boolean getUseStopWords()
```


Gets a value indicating whether to use stop words or not. The default value is  true .

**Returns:**
boolean - A value indicating whether to use stop words or not.
### setUseStopWords(boolean value) {#setUseStopWords-boolean-}
```
public final void setUseStopWords(boolean value)
```


Sets a value indicating whether to use stop words or not. The default value is  true .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to use stop words or not. |

### getMaxIndexingReportCount() {#getMaxIndexingReportCount--}
```
public final int getMaxIndexingReportCount()
```


Gets the maximum number of indexing reports. The default value is  5 .

**Returns:**
int - The maximum number of indexing reports.
### setMaxIndexingReportCount(int value) {#setMaxIndexingReportCount-int-}
```
public final void setMaxIndexingReportCount(int value)
```


Sets the maximum number of indexing reports. The default value is  5 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of indexing reports. |

### getMaxSearchReportCount() {#getMaxSearchReportCount--}
```
public final int getMaxSearchReportCount()
```


Gets the maximum number of search reports. The default value is  10 .

**Returns:**
int - The maximum number of search reports.
### setMaxSearchReportCount(int value) {#setMaxSearchReportCount-int-}
```
public final void setMaxSearchReportCount(int value)
```


Sets the maximum number of search reports. The default value is  10 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of search reports. |

### getUseCharacterReplacements() {#getUseCharacterReplacements--}
```
public final boolean getUseCharacterReplacements()
```


Gets a value indicating whether to use character replacements or not. The default value is  false .

**Returns:**
boolean - A value indicating whether to use character replacements or not.
### setUseCharacterReplacements(boolean value) {#setUseCharacterReplacements-boolean-}
```
public final void setUseCharacterReplacements(boolean value)
```


Sets a value indicating whether to use character replacements or not. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to use character replacements or not. |

### getAutoDetectEncoding() {#getAutoDetectEncoding--}
```
public final boolean getAutoDetectEncoding()
```


Gets a value indicating whether to detect encoding automatically or not. The default value is  false .

**Returns:**
boolean - A value indicating whether to detect encoding automatically or not.
### setAutoDetectEncoding(boolean value) {#setAutoDetectEncoding-boolean-}
```
public final void setAutoDetectEncoding(boolean value)
```


Sets a value indicating whether to detect encoding automatically or not. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether to detect encoding automatically or not. |

### getUseRawTextExtraction() {#getUseRawTextExtraction--}
```
public final boolean getUseRawTextExtraction()
```


Gets a value indicating whether the raw mode is used for text extraction if possible. The default value is  true . The raw mode can significantly increase the indexing speed, but normal mode improves the formatting of the extracted text.

**Returns:**
boolean - A value indicating whether the raw mode is used for text extraction if possible.
### setUseRawTextExtraction(boolean value) {#setUseRawTextExtraction-boolean-}
```
public final void setUseRawTextExtraction(boolean value)
```


Sets a value indicating whether the raw mode is used for text extraction if possible. The default value is  true . The raw mode can significantly increase the indexing speed, but normal mode improves the formatting of the extracted text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating whether the raw mode is used for text extraction if possible. |

### getDocumentFilter() {#getDocumentFilter--}
```
public final DocumentFilter getDocumentFilter()
```


Gets a document filter. The  DocumentFilter  works on the inclusion logic. Use the  DocumentFilter  class for creation a document filter instance. The default value is  null , which means that all added documents are indexed.

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - The document filter.

The example demonstrates how to set the document filter.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating a filter that skips documents with extensions '.doc', '.docx', '.rtf'
 IndexSettings settings = new IndexSettings();
 DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
 DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inverting file extension filter
 settings.setDocumentFilter(invertedFilter);
 // Creating an index in the specified folder
 Index index = new Index(indexFolder, settings);
 // Indexing documents
 index.add(documentsFolder);
 // Searching
 SearchResult result = index.search("Einstein");
 
```
### setDocumentFilter(DocumentFilter value) {#setDocumentFilter-com.groupdocs.search.DocumentFilter-}
```
public final void setDocumentFilter(DocumentFilter value)
```


Sets a document filter. The  DocumentFilter  works on the inclusion logic. Use the  GroupDocs.Search.Options.DocumentFilter  class for creation of a document filter instances. The default value is  null , which means that all added documents are indexed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DocumentFilter](../../com.groupdocs.search/documentfilter) | The document filter.

The example demonstrates how to set the document filter.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating a filter that skips documents with extensions '.doc', '.docx', '.rtf'
 IndexSettings settings = new IndexSettings();
 DocumentFilter fileExtensionFilter = DocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
 DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter); // Inverting file extension filter
 settings.setDocumentFilter(invertedFilter);
 // Creating an index in the specified folder
 Index index = new Index(indexFolder, settings);
 // Indexing documents
 index.add(documentsFolder);
 // Searching
 SearchResult result = index.search("Einstein");
 
``` |

### getTextStorageSettings() {#getTextStorageSettings--}
```
public final TextStorageSettings getTextStorageSettings()
```


Gets the text storage settings. The default value is  null , which means that document texts are not stored.

**Returns:**
[TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) - The text storage settings.

The example demonstrates how to set the text storage settings.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating index settings instance
 IndexSettings settings = new IndexSettings();
 settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Setting high compression level for the index text storage
 // Creating an index in the specified folder
 Index index = new Index(indexFolder, settings);
 // Indexing documents
 index.add(documentsFolder);
 // Searching
 SearchResult result = index.search("Einstein");
 
```
### setTextStorageSettings(TextStorageSettings value) {#setTextStorageSettings-com.groupdocs.search.options.TextStorageSettings-}
```
public final void setTextStorageSettings(TextStorageSettings value)
```


Sets the text storage settings. The default value is  null , which means that document texts are not stored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextStorageSettings](../../com.groupdocs.search.options/textstoragesettings) | The text storage settings.

The example demonstrates how to set the text storage settings.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 // Creating index settings instance
 IndexSettings settings = new IndexSettings();
 settings.setTextStorageSettings(new TextStorageSettings(Compression.High)); // Setting high compression level for the index text storage
 // Creating an index in the specified folder
 Index index = new Index(indexFolder, settings);
 // Indexing documents
 index.add(documentsFolder);
 // Searching
 SearchResult result = index.search("Einstein");
 
``` |

### getIndexType() {#getIndexType--}
```
public final IndexType getIndexType()
```


Gets the index type. The default value is  GroupDocs.Search.Options.IndexType.NormalIndex .

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type.
### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public final void setIndexType(IndexType value)
```


Sets the index type. The default value is  GroupDocs.Search.Options.IndexType.NormalIndex .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndexType](../../com.groupdocs.search.options/indextype) | The index type. |

### getSearchThreads() {#getSearchThreads--}
```
public final NumberOfThreads getSearchThreads()
```


Gets the number of threads used for the search. The default value is  GroupDocs.Search.Options.NumberOfThreads.Default , which means that the search will be performed using the number of threads equal to the number of processor cores.

**Returns:**
[NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) - The number of threads used for the search.
### setSearchThreads(NumberOfThreads value) {#setSearchThreads-com.groupdocs.search.options.NumberOfThreads-}
```
public final void setSearchThreads(NumberOfThreads value)
```


Sets the number of threads used for the search. The default value is  GroupDocs.Search.Options.NumberOfThreads.Default , which means that the search will be performed using the number of threads equal to the number of processor cores.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NumberOfThreads](../../com.groupdocs.search.options/numberofthreads) | The number of threads used for the search. |

### getCustomExtractors() {#getCustomExtractors--}
```
public final CustomExtractorCollection getCustomExtractors()
```


Gets the custom extractor collection.

The full example of implementing a custom extractor is presented in documentation for  GroupDocs.Search.Common.IFieldExtractor  interface.

**Returns:**
[CustomExtractorCollection](../../com.groupdocs.search.common/customextractorcollection) - The custom extractor collection.
### getLogger() {#getLogger--}
```
public final ILogger getLogger()
```


Gets a logger that is used for logging events and errors in the index. Note that the logger is not saved and must be created and assigned each time the index is created or loaded.

**Returns:**
[ILogger](../../com.groupdocs.search.common/ilogger) - A logger that is used for logging events and errors in the index.
### setLogger(ILogger value) {#setLogger-com.groupdocs.search.common.ILogger-}
```
public final void setLogger(ILogger value)
```


Sets a logger that is used for logging events and errors in the index. Note that the logger is not saved and must be created and assigned each time the index is created or loaded.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ILogger](../../com.groupdocs.search.common/ilogger) | A logger that is used for logging events and errors in the index. |

