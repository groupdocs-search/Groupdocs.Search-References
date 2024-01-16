---
title: NetworkOptimizationProgressEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents the arguments for the progress change event of the optimization operation.
type: docs
weight: 15
url: /java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Represents the arguments for the progress change event of the optimization operation.
## Methods

| Method | Description |
| --- | --- |
| [getNodeIndex()](#getNodeIndex--) | Gets the index of the search network node. |
| [getServiceIndex()](#getServiceIndex--) | Gets the index of the search network node service. |
| [getProcessedSegments()](#getProcessedSegments--) | Gets the number of processed segments. |
| [getTotalSegments()](#getTotalSegments--) | Gets the total number of segments for processing. |
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
### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Gets the number of processed segments.

**Returns:**
int - The number of processed segments.
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Gets the total number of segments for processing.

**Returns:**
int - The total number of segments for processing.
### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Gets the percentage of the progress.

**Returns:**
double - The percentage of the progress.
