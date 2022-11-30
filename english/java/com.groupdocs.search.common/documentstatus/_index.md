---
title: DocumentStatus
second_title: GroupDocs.Search for Java API Reference
description: Represents a document processing status.
type: docs
weight: 42
url: /java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Represents a document processing status.
## Fields

| Field | Description |
| --- | --- |
| [SuccessfullyProcessed](#SuccessfullyProcessed) | Document successfully indexed. |
| [Skipped](#Skipped) | Document skipped. |
| [ProcessedWithError](#ProcessedWithError) | Error occurred during document indexing. |
## Methods

| Method | Description |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Document successfully indexed.

### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Document skipped.

### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Error occurred during document indexing.

### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
