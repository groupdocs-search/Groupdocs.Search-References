---
title: FileIndexingEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of a document indexing start.
type: docs
weight: 14
url: /java/com.groupdocs.search.events/fileindexingeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class FileIndexingEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event of a document indexing start.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getDocument()](#getDocument--) | Gets the document. |
| [getDocumentFullPath()](#getDocumentFullPath--) | Gets the document full path. |
| [getDocumentKey()](#getDocumentKey--) | Gets the document key. |
| [getSkipIndexing()](#getSkipIndexing--) | Gets a value indicating that indexing of the document should be skipped. |
| [setSkipIndexing(boolean value)](#setSkipIndexing-boolean-) | Sets a value indicating that indexing of the document should be skipped. |
| [getEncoding()](#getEncoding--) | Gets the encoding of the document. |
| [setEncoding(String value)](#setEncoding-java.lang.String-) | Sets the encoding of the document. |
| [getCustomExtractor()](#getCustomExtractor--) | Gets the custom text extractor. |
| [setCustomExtractor(IFieldExtractor value)](#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-) | Sets the custom text extractor. |
| [getAdditionalFields()](#getAdditionalFields--) | Gets the additional fields for the document. |
| [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Sets the additional fields for the document. |
| [getAttributes()](#getAttributes--) | Gets the attributes of the document. |
| [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Set the attributes of the document. |
### getDocument() {#getDocument--}
```
public final Document getDocument()
```


Gets the document.

**Returns:**
[Document](../../com.groupdocs.search/document) - The document.
### getDocumentFullPath() {#getDocumentFullPath--}
```
public final String getDocumentFullPath()
```


Gets the document full path.

**Returns:**
java.lang.String - The document full path.
### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Gets the document key.

**Returns:**
java.lang.String - The document key.
### getSkipIndexing() {#getSkipIndexing--}
```
public final boolean getSkipIndexing()
```


Gets a value indicating that indexing of the document should be skipped.

**Returns:**
boolean - A value indicating that indexing of the document should be skipped.
### setSkipIndexing(boolean value) {#setSkipIndexing-boolean-}
```
public final void setSkipIndexing(boolean value)
```


Sets a value indicating that indexing of the document should be skipped.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | A value indicating that indexing of the document should be skipped. |

### getEncoding() {#getEncoding--}
```
public final String getEncoding()
```


Gets the encoding of the document.

**Returns:**
java.lang.String - The encoding of the document.
### setEncoding(String value) {#setEncoding-java.lang.String-}
```
public final void setEncoding(String value)
```


Sets the encoding of the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | The encoding of the document. |

### getCustomExtractor() {#getCustomExtractor--}
```
public final IFieldExtractor getCustomExtractor()
```


Gets the custom text extractor.

**Returns:**
[IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) - The custom text extractor.
### setCustomExtractor(IFieldExtractor value) {#setCustomExtractor-com.groupdocs.search.common.IFieldExtractor-}
```
public final void setCustomExtractor(IFieldExtractor value)
```


Sets the custom text extractor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor) | The custom text extractor. |

### getAdditionalFields() {#getAdditionalFields--}
```
public final DocumentField[] getAdditionalFields()
```


Gets the additional fields for the document.

**Returns:**
com.groupdocs.search.common.DocumentField[] - The additional fields for the document.
### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public final void setAdditionalFields(DocumentField[] value)
```


Sets the additional fields for the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | The additional fields for the document. |

### getAttributes() {#getAttributes--}
```
public final String[] getAttributes()
```


Gets the attributes of the document.

**Returns:**
java.lang.String[] - The attributes of the document.
### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public final void setAttributes(String[] value)
```


Set the attributes of the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String[] | The attributes of the document. |

