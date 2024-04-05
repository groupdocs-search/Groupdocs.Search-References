---
title: OptimizationProgressEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of the indexing operation progress is updated.
type: docs
weight: 19
url: /java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event of the indexing operation progress is updated.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getTotalSegments()](#getTotalSegments--) | Gets the total number of segments for processing. |
| [getProcessedSegments()](#getProcessedSegments--) | Gets the number of processed segments. |
| [getProgressPercentage()](#getProgressPercentage--) | Gets the percentage of the progress. |
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Gets the total number of segments for processing.

**Returns:**
int - The total number of segments for processing.
### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Gets the number of processed segments.

**Returns:**
int - The number of processed segments.
### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Gets the percentage of the progress.

**Returns:**
double - The percentage of the progress.
