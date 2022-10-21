---
title: ExtractedItemInfo
second_title: GroupDocs.Search for Java API Reference
description: Represents a container item information.
type: docs
weight: 20
url: /java/com.groupdocs.search.common/extractediteminfo/
---
**Inheritance:**
java.lang.Object
```
public class ExtractedItemInfo
```

Represents a container item information.

**Learn more**

 *  [Custom text extractors][]


[Custom text extractors]: https://docs.groupdocs.com/display/searchjava/Custom+text+extractors
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)](#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-) | Initializes a new instance of the  ExtractedItemInfo  class. |
## Methods

| Method | Description |
| --- | --- |
| [getFormatFamily()](#getFormatFamily--) | Gets a document type. |
| [getFields()](#getFields--) | Gets an extracted fields. |
| [getItemInfo()](#getItemInfo--) | Gets an item information. |
| [getInnerPath()](#getInnerPath--) | Gets an inner path. |
### ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath) {#ExtractedItemInfo-com.groupdocs.search.results.FormatFamily-com.groupdocs.search.common.DocumentField---java.lang.String-java.lang.String-}
```
public ExtractedItemInfo(FormatFamily formatFamily, DocumentField[] fields, String itemInfo, String innerPath)
```


Initializes a new instance of the  ExtractedItemInfo  class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formatFamily | [FormatFamily](../../com.groupdocs.search.results/formatfamily) | The document format family. |
| fields | [DocumentField\[\]](../../com.groupdocs.search.common/documentfield) | The extracted fields. |
| itemInfo | java.lang.String | The item information. |
| innerPath | java.lang.String | The path to the item in the container. |

### getFormatFamily() {#getFormatFamily--}
```
public final FormatFamily getFormatFamily()
```


Gets a document type.

**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document type.
### getFields() {#getFields--}
```
public final DocumentField[] getFields()
```


Gets an extracted fields.

**Returns:**
com.groupdocs.search.common.DocumentField[] - The extracted fields.
### getItemInfo() {#getItemInfo--}
```
public final String getItemInfo()
```


Gets an item information.

**Returns:**
java.lang.String - The item information.
### getInnerPath() {#getInnerPath--}
```
public final String getInnerPath()
```


Gets an inner path.

**Returns:**
java.lang.String - The inner path.
