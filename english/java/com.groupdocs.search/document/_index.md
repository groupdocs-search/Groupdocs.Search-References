---
title: Document
second_title: GroupDocs.Search for Java API Reference
description: Represents the base class for documents added to an index from file system stream or structure.
type: docs
weight: 13
url: /java/com.groupdocs.search/document/
---
**Inheritance:**
java.lang.Object
```
public abstract class Document
```

Represents the base class for documents added to an index from file system, stream, or structure. Contains static methods for creating documents from different types of sources.

**Learn more**

 *  [Indexing from different sources][]


[Indexing from different sources]: https://docs.groupdocs.com/search/java/indexing-from-different-sources/
## Methods

| Method | Description |
| --- | --- |
| [getDocumentSourceKind()](#getDocumentSourceKind--) | Gets the document source kind. |
| [getDocumentKey()](#getDocumentKey--) | Gets the document key that is used to identify the document within an index. |
| [isLazy()](#isLazy--) | Gets a value indicating whether the document is loaded as needed or not. |
| [getModificationDate()](#getModificationDate--) | Gets the last modification date of the document. |
| [getExtension()](#getExtension--) | Gets the extension used for this document type. |
| [getAdditionalFields()](#getAdditionalFields--) | Gets the additional fields for the document. |
| [setAdditionalFields(DocumentField[] value)](#setAdditionalFields-com.groupdocs.search.common.DocumentField---) | Sets the additional fields for the document. |
| [getAttributes()](#getAttributes--) | Gets the attributes of the document. |
| [setAttributes(String[] value)](#setAttributes-java.lang.String---) | Sets the attributes of the document. |
| [createFromFile(String filePath)](#createFromFile-java.lang.String-) | Creates a document from a file. |
| [createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)](#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-) | Creates a document from a stream. |
| [createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)](#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---) | Creates a document from a structure that is an array of text fields. |
| [createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)](#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-) | Creates a lazy-loaded document. |
| [toString()](#toString--) | Returns a  java.lang.String  that represents the current  Document . |
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public abstract DocumentSourceKind getDocumentSourceKind()
```


Gets the document source kind.

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.
### getDocumentKey() {#getDocumentKey--}
```
public abstract String getDocumentKey()
```


Gets the document key that is used to identify the document within an index.

**Returns:**
java.lang.String - The document key that is used to identify the document within an index.
### isLazy() {#isLazy--}
```
public abstract boolean isLazy()
```


Gets a value indicating whether the document is loaded as needed or not.

**Returns:**
boolean - A value indicating whether the document is loaded as needed or not.
### getModificationDate() {#getModificationDate--}
```
public abstract Date getModificationDate()
```


Gets the last modification date of the document.

**Returns:**
java.util.Date - The last modification date of the document.
### getExtension() {#getExtension--}
```
public abstract String getExtension()
```


Gets the extension used for this document type.

**Returns:**
java.lang.String - The extension used for this document type.
### getAdditionalFields() {#getAdditionalFields--}
```
public DocumentField[] getAdditionalFields()
```


Gets the additional fields for the document.

**Returns:**
com.groupdocs.search.common.DocumentField[] - The additional fields for the document.
### setAdditionalFields(DocumentField[] value) {#setAdditionalFields-com.groupdocs.search.common.DocumentField---}
```
public void setAdditionalFields(DocumentField[] value)
```


Sets the additional fields for the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | The additional fields for the document. |

### getAttributes() {#getAttributes--}
```
public String[] getAttributes()
```


Gets the attributes of the document.

**Returns:**
java.lang.String[] - The attributes of the document.
### setAttributes(String[] value) {#setAttributes-java.lang.String---}
```
public void setAttributes(String[] value)
```


Sets the attributes of the document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String[] | The attributes of the document. |

### createFromFile(String filePath) {#createFromFile-java.lang.String-}
```
public static Document createFromFile(String filePath)
```


Creates a document from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The document file path. |

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.
### createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream) {#createFromStream-java.lang.String-java.util.Date-java.lang.String-java.io.InputStream-}
```
public static Document createFromStream(String documentKey, Date modificationDate, String extension, InputStream stream)
```


Creates a document from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentKey | java.lang.String | The document key. |
| modificationDate | java.util.Date | The document modification date. |
| extension | java.lang.String | The document extension. |
| stream | java.io.InputStream | The document stream. |

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.
### createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields) {#createFromStructure-java.lang.String-java.util.Date-com.groupdocs.search.common.DocumentField---}
```
public static Document createFromStructure(String documentKey, Date modificationDate, DocumentField[] fields)
```


Creates a document from a structure that is an array of text fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentKey | java.lang.String | The document key. |
| modificationDate | java.util.Date | The document modification date. |
| fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | The document fields. |

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.
### createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader) {#createLazy-com.groupdocs.search.common.DocumentSourceKind-java.lang.String-com.groupdocs.search.common.IDocumentLoader-}
```
public static Document createLazy(DocumentSourceKind documentSourceKind, String documentKey, IDocumentLoader documentLoader)
```


Creates a lazy-loaded document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| documentSourceKind | [DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) | The document source kind. This value must match the kind of the loaded document. |
| documentKey | java.lang.String | The document key. This value must match the key of the loaded document. |
| documentLoader | [IDocumentLoader](../../com.groupdocs.search.common/idocumentloader) | The document loader. |

**Returns:**
[Document](../../com.groupdocs.search/document) - The created document.
### toString() {#toString--}
```
public String toString()
```


Returns a  java.lang.String  that represents the current  Document .

**Returns:**
java.lang.String - A  java.lang.String  that represents the current  Document .
