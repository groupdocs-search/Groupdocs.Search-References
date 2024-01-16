---
title: DocumentSourceKind
second_title: GroupDocs.Search for Java API Reference
description: Defines the kinds of document sources.
type: docs
weight: 39
url: /java/com.groupdocs.search.common/documentsourcekind/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentSourceKind extends Enum<DocumentSourceKind>
```

Defines the kinds of document sources.
## Fields

| Field | Description |
| --- | --- |
| [File](#File) | The file document source. |
| [Stream](#Stream) | The stream document source. |
| [Structure](#Structure) | The structure document source. |
| [ExtractedData](#ExtractedData) | The document source of previously extracted data. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### File {#File}
```
public static final DocumentSourceKind File
```


The file document source.

### Stream {#Stream}
```
public static final DocumentSourceKind Stream
```


The stream document source.

### Structure {#Structure}
```
public static final DocumentSourceKind Structure
```


The structure document source.

### ExtractedData {#ExtractedData}
```
public static final DocumentSourceKind ExtractedData
```


The document source of previously extracted data.

### values() {#values--}
```
public static DocumentSourceKind[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentSourceKind[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentSourceKind valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[DocumentSourceKind](../../com.groupdocs.search.common/documentsourcekind)
