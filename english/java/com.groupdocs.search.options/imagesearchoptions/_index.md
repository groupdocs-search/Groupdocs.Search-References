---
title: ImageSearchOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for reverse image search operation.
type: docs
weight: 22
url: /java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Provides options for reverse image search operation.
## Constructors

| Constructor | Description |
| --- | --- |
| [ImageSearchOptions()](#ImageSearchOptions--) | Initializes a new instance of the  ImageSearchOptions  class. |
| [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Initializes a new instance of the  ImageSearchOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getHashDifferences()](#getHashDifferences--) | Gets the maximum number of mismatched bits in the image hash. |
| [setHashDifferences(int value)](#setHashDifferences-int-) | Sets the maximum number of mismatched bits in the image hash. |
| [getMaxResultCount()](#getMaxResultCount--) | Gets the maximum number of found images for an image reverse search request. |
| [setMaxResultCount(int value)](#setMaxResultCount-int-) | Sets the maximum number of found images for an image reverse search request. |
| [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Gets the search document filter. |
| [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Gets or sets the search document filter. |
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Initializes a new instance of the  ImageSearchOptions  class.

### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Initializes a new instance of the  ImageSearchOptions  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | java.lang.Object | The serialized data. |

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Gets the maximum number of mismatched bits in the image hash. The default value is  5 .

**Returns:**
int - The maximum number of mismatched bits in the image hash.
### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Sets the maximum number of mismatched bits in the image hash. The default value is  5 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of mismatched bits in the image hash. |

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Gets the maximum number of found images for an image reverse search request. The default value is  1000 .

**Returns:**
int - The maximum number of found images for an image reverse search request.
### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Sets the maximum number of found images for an image reverse search request. The default value is  1000 .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The maximum number of found images for an image reverse search request. |

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Gets the search document filter.  SearchDocumentFilter  works on the inclusion logic. Use  GroupDocs.Search.Options.SearchDocumentFilter  class for creation of a search document filter instances. The default value is  null , which means that all found documents will be returned.

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.
### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Gets or sets the search document filter.  SearchDocumentFilter  works on the inclusion logic. Use  GroupDocs.Search.Options.SearchDocumentFilter  class for creation of a search document filter instances. The default value is  null , which means that all found documents will be returned.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | The search document filter. |

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
