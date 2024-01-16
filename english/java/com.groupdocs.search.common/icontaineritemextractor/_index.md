---
title: IContainerItemExtractor
second_title: GroupDocs.Search for Java API Reference
description: Provides methods for extracting items from container documents.
type: docs
weight: 35
url: /java/com.groupdocs.search.common/icontaineritemextractor/
---
**All Implemented Interfaces:**
[com.groupdocs.search.common.IFieldExtractor](../../com.groupdocs.search.common/ifieldextractor)
```
public interface IContainerItemExtractor extends IFieldExtractor
```

Provides methods for extracting items from container documents.

**Learn more**

 *  [Custom text extractors][]


[Custom text extractors]: https://docs.groupdocs.com/display/searchjava/Custom+text+extractors
## Methods

| Method | Description |
| --- | --- |
| [getFormatFamily()](#getFormatFamily--) | Gets the document format family. |
| [getContainerItems(String filePath)](#getContainerItems-java.lang.String-) | Extracts items from container document. |
| [getContainerItems(InputStream stream)](#getContainerItems-java.io.InputStream-) | Extracts items from container document. |
### getFormatFamily() {#getFormatFamily--}
```
public abstract FormatFamily getFormatFamily()
```


Gets the document format family.

**Returns:**
[FormatFamily](../../com.groupdocs.search.results/formatfamily) - The document format family.
### getContainerItems(String filePath) {#getContainerItems-java.lang.String-}
```
public abstract ExtractedItemInfo[] getContainerItems(String filePath)
```


Extracts items from container document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - An array of extracted items.
### getContainerItems(InputStream stream) {#getContainerItems-java.io.InputStream-}
```
public abstract ExtractedItemInfo[] getContainerItems(InputStream stream)
```


Extracts items from container document.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The document stream. |

**Returns:**
com.groupdocs.search.common.ExtractedItemInfo[] - An array of extracted items.
