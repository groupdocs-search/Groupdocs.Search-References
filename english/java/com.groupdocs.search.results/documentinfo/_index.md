---
title: DocumentInfo
second_title: GroupDocs.Search for Java API Reference
description: Represents a descriptor for an indexed document.
type: docs
weight: 11
url: /java/com.groupdocs.search.results/documentinfo/
---
**Inheritance:**
java.lang.Object
```
public class DocumentInfo
```

Represents a descriptor for an indexed document.

**Learn more**

 *  [Search results][]
 *  [Getting indexed documents][]


[Search results]: https://docs.groupdocs.com/display/searchjava/Search+results
[Getting indexed documents]: https://docs.groupdocs.com/display/searchjava/Getting+indexed+documents
## Methods

| Method | Description |
| --- | --- |
| [toString()](#toString--) | Returns a  System.String  that represents the current  DocumentInfo . |
| [getFilePath()](#getFilePath--) | Gets the file path for indexed from file or the document key for indexed from stream or structure. |
| [getFileType()](#getFileType--) | Gets the file type. |
| [getFormatFamily()](#getFormatFamily--) | Gets the document format family. |
| [getInnerPath()](#getInnerPath--) | Gets the inner path for the container document item. |
| [getInnerPathParts()](#getInnerPathParts--) | Gets the inner path parts for the container document item. |
| [getDocumentSourceKind()](#getDocumentSourceKind--) | Gets the document source kind. |
| [getIndexedWithError()](#getIndexedWithError--) | Gets the indicator of indexing error. |
| [serialize()](#serialize--) | Serializes the current instance to a byte array. |
| [deserialize(byte[] array)](#deserialize-byte---) | Deserializes an instance from a byte array. |
### toString() {#toString--}
```
public String toString()
```


Returns a  System.String  that represents the current  DocumentInfo .

**Returns:**
java.lang.String - A  System.String  that represents the current  DocumentInfo .
### getFilePath() {#getFilePath--}
```
public final String getFilePath()
```


Gets the file path for indexed from file or the document key for indexed from stream or structure.

**Returns:**
java.lang.String - The file path or document key.
### getFileType() {#getFileType--}
```
public final FileType getFileType()
```


Gets the file type.

**Returns:**
[FileType](../../com.groupdocs.search.results/filetype) - The file type.
### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Gets the document format family.

**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.
### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Gets the inner path for the container document item.

**Returns:**
java.lang.String - The inner path.
### getInnerPathParts() {#getInnerPathParts--}
```
public final String[] getInnerPathParts()
```


Gets the inner path parts for the container document item.

**Returns:**
java.lang.String[] - The inner path parts.
### getDocumentSourceKind() {#getDocumentSourceKind--}
```
public final DocumentSourceKind getDocumentSourceKind()
```


Gets the document source kind.

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind) - The document source kind.
### getIndexedWithError() {#getIndexedWithError--}
```
public final boolean getIndexedWithError()
```


Gets the indicator of indexing error.

**Returns:**
boolean - The indicator of indexing error.
### serialize() {#serialize--}
```
public final byte[] serialize()
```


Serializes the current instance to a byte array.

**Returns:**
byte[] - A byte array representing the current instance.
### deserialize(byte[] array) {#deserialize-byte---}
```
public static DocumentInfo deserialize(byte[] array)
```


Deserializes an instance from a byte array.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| array | byte[] | A byte array to deserialize from. |

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - An instance deserialized from a byte array.
