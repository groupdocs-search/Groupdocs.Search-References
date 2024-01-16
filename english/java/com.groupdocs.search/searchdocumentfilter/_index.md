---
title: SearchDocumentFilter
second_title: GroupDocs.Search for Java API Reference
description: Contains methods for creating search document filters.
type: docs
weight: 24
url: /java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Contains methods for creating search document filters.

**Learn more**

 *  [Document filtering in search result][]
 *  [Search options][]


[Document filtering in search result]: https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result
[Search options]: https://docs.groupdocs.com/display/searchjava/Search+options
## Constructors

| Constructor | Description |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Methods

| Method | Description |
| --- | --- |
| [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Creates a filter for skipping documents that are not match a regular expression. |
| [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Creates a filter for skipping documents that are not match a regular expression. |
| [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Creates a filter for skipping documents that are not in the specified list of possible extensions. |
| [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Creates a filter that has inverse logic in relation to the specified inner filter. |
| [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Creates a logical conjunction of the specified filters. |
| [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Creates a logical disjunction of the specified filters. |
| [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Creates a filter for skipping documents that do not have any value from the specified list of allowable attributes. |
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Creates a filter for skipping documents that are not match a regular expression. The regular expression is applied to the full path of a document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | The regular expression pattern. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.
### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Creates a filter for skipping documents that are not match a regular expression. The regular expression is applied to the full path of a document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | The regular expression pattern. |
| options | int | The regular expression options. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.
### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Creates a filter for skipping documents that are not in the specified list of possible extensions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extensions | java.lang.String[] | The list of possible extensions. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.
### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Creates a filter that has inverse logic in relation to the specified inner filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | The inner search document filter. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.
### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Creates a logical conjunction of the specified filters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | The search document filters. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.
### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Creates a logical disjunction of the specified filters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | The search document filters. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.
### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Creates a filter for skipping documents that do not have any value from the specified list of allowable attributes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| attributes | java.lang.String[] | The list of allowable attributes. |

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.
