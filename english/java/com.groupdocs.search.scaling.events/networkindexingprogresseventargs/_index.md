---
title: NetworkIndexingProgressEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents the arguments for the progress change event of the indexing operation.
type: docs
weight: 14
url: /java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Represents the arguments for the progress change event of the indexing operation.
## Methods

| Method | Description |
| --- | --- |
| [getNodeIndex()](#getNodeIndex--) | Gets the index of the search network node. |
| [getServiceIndex()](#getServiceIndex--) | Gets the index of the search network node service. |
| [getProcessedDocuments()](#getProcessedDocuments--) | Gets the number of processed documents. |
| [getTotalDocuments()](#getTotalDocuments--) | Gets the total number of documents for processing. |
| [getProgressPercentage()](#getProgressPercentage--) | Gets the percentage of the progress. |
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Gets the index of the search network node.

**Returns:**
int - The index of the search network node.
### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Gets the index of the search network node service.

**Returns:**
int - The index of the search network node service.
### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Gets the number of processed documents.

**Returns:**
int - The number of processed documents.
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Gets the total number of documents for processing.

**Returns:**
int - The total number of documents for processing.
### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Gets the percentage of the progress.

**Returns:**
double - The percentage of the progress.
