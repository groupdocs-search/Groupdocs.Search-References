---
title: DocumentFilter
second_title: GroupDocs.Search for Java API Reference
description: Represents the base class for document filters.
type: docs
weight: 14
url: /java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Represents the base class for document filters. Contains methods for creation document filter instances.

**Learn more**

 *  [Document filtering during indexing][]


[Document filtering during indexing]: https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Methods

| Method | Description |
| --- | --- |
| [toString()](#toString--) | Returns string representation of a document filter. |
| [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Creates a filter for skipping documents with creation date earlier than the lower bound. |
| [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Creates a filter for skipping documents with creation date later than the upper bound. |
| [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Creates a filter for skipping documents with creation date out of the specified range. |
| [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Creates a filter for skipping documents with modification date earlier than the lower bound. |
| [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Creates a filter for skipping documents with modification date later than the upper bound. |
| [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Creates a filter for skipping documents with modification date out of the specified range. |
| [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Creates a filter for skipping documents that are not match a regular expression. |
| [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Creates a filter for skipping documents that are not match a regular expression. |
| [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Creates a filter for skipping documents with the length less than the lower bound. |
| [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Creates a filter for skipping documents with the length greater than the upper bound. |
| [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Creates a filter for skipping documents out of the specified document length range. |
| [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Creates a filter for skipping documents that do not have allowable extension. |
| [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Creates a filter that has inverse logic in relation to the specified inner filter. |
| [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Creates a logical conjunction of the specified filters. |
| [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Creates a logical disjunction of the specified filters. |
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Returns string representation of a document filter.

**Returns:**
java.lang.String - String representation of a document filter.
### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Creates a filter for skipping documents with creation date earlier than the lower bound.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lowerBound | java.util.Date | The lower bound of the document creation time. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.
### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Creates a filter for skipping documents with creation date later than the upper bound.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperBound | java.util.Date | The upper bound of the document creation time. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.
### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Creates a filter for skipping documents with creation date out of the specified range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lowerBound | java.util.Date | The lower bound of the document creation time. |
| upperBound | java.util.Date | The upper bound of the document creation time. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.
### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Creates a filter for skipping documents with modification date earlier than the lower bound.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lowerBound | java.util.Date | The lower bound of the document modification time. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.
### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Creates a filter for skipping documents with modification date later than the upper bound.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperBound | java.util.Date | The upper bound of the document modification time. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.
### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Creates a filter for skipping documents with modification date out of the specified range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lowerBound | java.util.Date | The lower bound of the document modification time. |
| upperBound | java.util.Date | The upper bound of the document modification time. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.
### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Creates a filter for skipping documents that are not match a regular expression. The regular expression is applied to the full path of a document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | The regular expression pattern. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.
### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Creates a filter for skipping documents that are not match a regular expression. The regular expression is applied to the full path of a document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pattern | java.lang.String | The regular expression pattern. |
| options | int | The regular expression options. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.
### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Creates a filter for skipping documents with the length less than the lower bound.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lowerBound | long | The lower bound of the document length. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.
### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Creates a filter for skipping documents with the length greater than the upper bound.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperBound | long | The upper bound of the document length. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.
### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Creates a filter for skipping documents out of the specified document length range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| lowerBound | long | The lower bound of the document length. |
| upperBound | long | The upper bound of the document length. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.
### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Creates a filter for skipping documents that do not have allowable extension.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extensions | java.lang.String[] | The list of allowable extensions. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.
### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Creates a filter that has inverse logic in relation to the specified inner filter.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | The inner document filter. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.
### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Creates a logical conjunction of the specified filters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | The document filters. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.
### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Creates a logical disjunction of the specified filters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | The document filters. |

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.
