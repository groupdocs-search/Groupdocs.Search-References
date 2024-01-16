---
title: ExtractorSettings
second_title: GroupDocs.Search for Java API Reference
description: Contains settings for the document data extractor.
type: docs
weight: 19
url: /java/com.groupdocs.search.common/extractorsettings/
---
**Inheritance:**
java.lang.Object
```
public abstract class ExtractorSettings
```

Contains settings for the document data extractor.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtractorSettings()](#ExtractorSettings--) |  |
## Methods

| Method | Description |
| --- | --- |
| [getIndexType()](#getIndexType--) | Gets the index type the extractor is used for. |
| [setIndexType(IndexType value)](#setIndexType-com.groupdocs.search.options.IndexType-) | Sets the index type the extractor is used for. |
### ExtractorSettings() {#ExtractorSettings--}
```
public ExtractorSettings()
```


### getIndexType() {#getIndexType--}
```
public abstract IndexType getIndexType()
```


Gets the index type the extractor is used for. The default value is  GroupDocs.Search.Options.IndexType.NormalIndex .

**Returns:**
[IndexType](../../com.groupdocs.search.options/indextype) - The index type the extractor is used for.
### setIndexType(IndexType value) {#setIndexType-com.groupdocs.search.options.IndexType-}
```
public abstract void setIndexType(IndexType value)
```


Sets the index type the extractor is used for. The default value is  GroupDocs.Search.Options.IndexType.NormalIndex .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IndexType](../../com.groupdocs.search.options/indextype) | The index type the extractor is used for. |

