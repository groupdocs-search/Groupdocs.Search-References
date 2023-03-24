---
title: SearchOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for search operation.
type: docs
weight: 31
url: /java/com.groupdocs.search.options/searchoptions/
---
**Inheritance:**
java.lang.Object
```
public class SearchOptions
```

Provides options for search operation.

**Learn more**

 *  [Search options][]


[Search options]: https://docs.groupdocs.com/display/searchjava/Search+options
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchOptions()](#SearchOptions--) | Initializes a new instance of the  SearchOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getUseSynonymSearch()](#getUseSynonymSearch--) | Gets the flag of use synonyms in search. |
| [setUseSynonymSearch(boolean value)](#setUseSynonymSearch-boolean-) | Sets the flag of use synonyms in search. |
| [getUseHomophoneSearch()](#getUseHomophoneSearch--) | Gets the flag of use homophones in search. |
| [setUseHomophoneSearch(boolean value)](#setUseHomophoneSearch-boolean-) | Sets the flag of use homophones in search. |
| [getUseWordFormsSearch()](#getUseWordFormsSearch--) | Gets the flag of use different word forms in search. |
| [setUseWordFormsSearch(boolean value)](#setUseWordFormsSearch-boolean-) | Sets the flag of use different word forms in search. |
| [getFuzzySearch()](#getFuzzySearch--) | Gets the fuzzy search options. |
| [getSpellingCorrector()](#getSpellingCorrector--) | Gets the spelling corrector options. |
| [getKeyboardLayoutCorrector()](#getKeyboardLayoutCorrector--) | Gets the keyboard layout corrector options. |
| [getUseCaseSensitiveSearch()](#getUseCaseSensitiveSearch--) | Gets the flag of case sensitive search. |
| [setUseCaseSensitiveSearch(boolean value)](#setUseCaseSensitiveSearch-boolean-) | Sets the flag of case sensitive search. |
| [getMaxTotalOccurrenceCount()](#getMaxTotalOccurrenceCount--) | Gets the maximum total number of occurrences of all terms in a search query. |
| [setMaxTotalOccurrenceCount(int value)](#setMaxTotalOccurrenceCount-int-) | Sets the maximum total number of occurrences of all terms in a search query. |
| [getMaxOccurrenceCountPerTerm()](#getMaxOccurrenceCountPerTerm--) | Gets the maximum number of occurrences of each term in a search query. |
| [setMaxOccurrenceCountPerTerm(int value)](#setMaxOccurrenceCountPerTerm-int-) | Sets the maximum number of occurrences of each term in a search query. |
| [getDateFormats()](#getDateFormats--) | Gets the collection of date formats for date range search. |
| [isChunkSearch()](#isChunkSearch--) | Gets the flag of search by chunks. |
| [setChunkSearch(boolean value)](#setChunkSearch-boolean-) | Sets the flag of search by chunks. |
| [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Gets the search document filter. |
| [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Sets the search document filter. |
| [getCancellation()](#getCancellation--) | Gets the operation cancellation object. |
| [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Sets the operation cancellation object. |
### SearchOptions() {#SearchOptions--}
```
public SearchOptions()
```


Initializes a new instance of the  SearchOptions  class.

### getUseSynonymSearch() {#getUseSynonymSearch--}
```
public final boolean getUseSynonymSearch()
```


Gets the flag of use synonyms in search. The default value is  false .

**Returns:**
boolean - The flag of use synonyms in search.
### setUseSynonymSearch(boolean value) {#setUseSynonymSearch-boolean-}
```
public final void setUseSynonymSearch(boolean value)
```


Sets the flag of use synonyms in search. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of use synonyms in search. |

### getUseHomophoneSearch() {#getUseHomophoneSearch--}
```
public final boolean getUseHomophoneSearch()
```


Gets the flag of use homophones in search. The default value is  false .

**Returns:**
boolean - The flag of use homophones in search.
### setUseHomophoneSearch(boolean value) {#setUseHomophoneSearch-boolean-}
```
public final void setUseHomophoneSearch(boolean value)
```


Sets the flag of use homophones in search. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of use homophones in search. |

### getUseWordFormsSearch() {#getUseWordFormsSearch--}
```
public final boolean getUseWordFormsSearch()
```


Gets the flag of use different word forms in search. The default value is  false .

**Returns:**
boolean - The flag of use different word forms in search.
### setUseWordFormsSearch(boolean value) {#setUseWordFormsSearch-boolean-}
```
public final void setUseWordFormsSearch(boolean value)
```


Sets the flag of use different word forms in search. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of use different word forms in search. |

### getFuzzySearch() {#getFuzzySearch--}
```
public final FuzzySearchOptions getFuzzySearch()
```


Gets the fuzzy search options.

**Returns:**
[FuzzySearchOptions](../../com.groupdocs.search.options/fuzzysearchoptions) - The fuzzy search options.
### getSpellingCorrector() {#getSpellingCorrector--}
```
public final SpellingCorrectorOptions getSpellingCorrector()
```


Gets the spelling corrector options.

**Returns:**
[SpellingCorrectorOptions](../../com.groupdocs.search.options/spellingcorrectoroptions) - The spelling corrector options.
### getKeyboardLayoutCorrector() {#getKeyboardLayoutCorrector--}
```
public final KeyboardLayoutCorrectorOptions getKeyboardLayoutCorrector()
```


Gets the keyboard layout corrector options.

**Returns:**
[KeyboardLayoutCorrectorOptions](../../com.groupdocs.search.options/keyboardlayoutcorrectoroptions) - The keyboard layout corrector options.
### getUseCaseSensitiveSearch() {#getUseCaseSensitiveSearch--}
```
public final boolean getUseCaseSensitiveSearch()
```


Gets the flag of case sensitive search. The default value is  false .

**Returns:**
boolean - The flag of case sensitive search.
### setUseCaseSensitiveSearch(boolean value) {#setUseCaseSensitiveSearch-boolean-}
```
public final void setUseCaseSensitiveSearch(boolean value)
```


Sets the flag of case sensitive search. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of case sensitive search. |

### getMaxTotalOccurrenceCount() {#getMaxTotalOccurrenceCount--}
```
public final int getMaxTotalOccurrenceCount()
```


Gets the maximum total number of occurrences of all terms in a search query. The default value is  500000 .

**Returns:**
int - The maximum total number of occurrences.
### setMaxTotalOccurrenceCount(int value) {#setMaxTotalOccurrenceCount-int-}
```
public final void setMaxTotalOccurrenceCount(int value)
```


Sets the maximum total number of occurrences of all terms in a search query. The default value is  500000 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum total number of occurrences. |

### getMaxOccurrenceCountPerTerm() {#getMaxOccurrenceCountPerTerm--}
```
public final int getMaxOccurrenceCountPerTerm()
```


Gets the maximum number of occurrences of each term in a search query. The default value is  100000 .

**Returns:**
int - The maximum number of occurrences of each term in a search query.
### setMaxOccurrenceCountPerTerm(int value) {#setMaxOccurrenceCountPerTerm-int-}
```
public final void setMaxOccurrenceCountPerTerm(int value)
```


Sets the maximum number of occurrences of each term in a search query. The default value is  100000 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of occurrences of each term in a search query. |

### getDateFormats() {#getDateFormats--}
```
public final DateFormatCollection getDateFormats()
```


Gets the collection of date formats for date range search. The default date formats are 'dd.MM.yyyy', 'MM/dd/yyyy', and 'yyyy-MM-dd'.

**Returns:**
[DateFormatCollection](../../com.groupdocs.search.options/dateformatcollection) - The collection of date formats for date range search.

The example demonstrates how to set the date formats for the search.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments\\";
 String query = "Einstein";
 Index index = new Index(indexFolder); // Creating an index in the specified folder
 index.add(documentsFolder); // Indexing documents from the specified folder
 SearchOptions options = new SearchOptions();
 options.getDateFormats().clear(); // Removing default date formats
 DateFormatElement[] elements = new DateFormatElement[] {
     DateFormatElement.getMonthTwoDigits(),
     DateFormatElement.getDayOfMonthTwoDigits(),
     DateFormatElement.getYearFourDigits(),
 };
 // Creating a date format pattern 'MM/dd/yyyy'
 com.groupdocs.search.DateFormat dateFormat = new com.groupdocs.search.DateFormat(elements, "/");
 options.getDateFormats().addItem(dateFormat);
 SearchResult result = index.search(query, options); // Search in index
 
```
### isChunkSearch() {#isChunkSearch--}
```
public final boolean isChunkSearch()
```


Gets the flag of search by chunks. The default value is  false .

**Returns:**
boolean - The flag of search by chunks.
### setChunkSearch(boolean value) {#setChunkSearch-boolean-}
```
public final void setChunkSearch(boolean value)
```


Sets the flag of search by chunks. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of search by chunks. |

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public final ISearchDocumentFilter getSearchDocumentFilter()
```


Gets the search document filter.  SearchDocumentFilter  works on the inclusion logic. Use  SearchDocumentFilter  class for creation of a search document filter instances. The default value is  null , which means that all found documents will be returned.

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

The example demonstrates how to set the document filter.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments1\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents
 index.add(documentsFolder);
 // Creating a search document filter that skips documents with extensions '.doc', '.docx', '.rtf'
 SearchOptions options = new SearchOptions();
 ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
 ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inverting file extension filter
 options.setSearchDocumentFilter(invertedFilter);
 // Search in index
 SearchResult result = index.search("Einstein", options);
 
```
### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public final void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Sets the search document filter.  SearchDocumentFilter  works on the inclusion logic. Use  SearchDocumentFilter  class for creation of a search document filter instances. The default value is  null , which means that all found documents will be returned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | The search document filter.

The example demonstrates how to set the document filter.

```

 String indexFolder = "c:\\MyIndex\\";
 String documentsFolder = "c:\\MyDocuments1\\";
 // Creating an index in the specified folder
 Index index = new Index(indexFolder);
 // Indexing documents
 index.add(documentsFolder);
 // Creating a search document filter that skips documents with extensions '.doc', '.docx', '.rtf'
 SearchOptions options = new SearchOptions();
 ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.createFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
 ISearchDocumentFilter invertedFilter = SearchDocumentFilter.createNot(fileExtensionFilter); // Inverting file extension filter
 options.setSearchDocumentFilter(invertedFilter);
 // Search in index
 SearchResult result = index.search("Einstein", options);
 
``` |

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Gets the operation cancellation object. The default value is  null .

**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.
### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Sets the operation cancellation object. The default value is  null .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cancellation](../../com.groupdocs.search.common/cancellation) | The operation cancellation object. |

