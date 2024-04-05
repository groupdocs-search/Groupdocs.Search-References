---
title: OperationProgressEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of the indexing operation progress is updated.
type: docs
weight: 18
url: /java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event of the indexing operation progress is updated.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getTotalDocuments()](#getTotalDocuments--) | Gets the total number of documents for processing. |
| [getProcessedDocuments()](#getProcessedDocuments--) | Gets the number of successfully processed documents. |
| [getSkippedDocuments()](#getSkippedDocuments--) | Gets the number of skipped documents. |
| [getProgressPercentage()](#getProgressPercentage--) | Gets the percentage of the progress. |
| [getLastDocumentKey()](#getLastDocumentKey--) | Gets the key of the last processed document. |
| [getLastDocumentPath()](#getLastDocumentPath--) | Gets the path of the last processed document. |
| [getLastDocumentStatus()](#getLastDocumentStatus--) | Gets the status of the last processed document. |
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Gets the total number of documents for processing.

**Returns:**
int - The total number of documents for processing.
### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Gets the number of successfully processed documents.

**Returns:**
int - The number of successfully processed documents.
### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Gets the number of skipped documents.

**Returns:**
int - The number of skipped documents.
### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Gets the percentage of the progress.

**Returns:**
double - The percentage of the progress.
### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Gets the key of the last processed document.

**Returns:**
java.lang.String - The last processed document key.
### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Gets the path of the last processed document.

**Returns:**
java.lang.String - The last processed document path.
### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Gets the status of the last processed document.

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.
