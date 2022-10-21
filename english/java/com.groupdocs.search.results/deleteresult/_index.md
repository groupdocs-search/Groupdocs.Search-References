---
title: DeleteResult
second_title: GroupDocs.Search for Java API Reference
description: Represents the result of the operation to delete indexed files or folders from an index.
type: docs
weight: 10
url: /java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Represents the result of the operation to delete indexed files or folders from an index.

**Learn more**

 *  [Delete indexed paths][]


[Delete indexed paths]: https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths
## Methods

| Method | Description |
| --- | --- |
| [getItemResults()](#getItemResults--) | Returns the results of deleting each path. |
| [getTotalCount()](#getTotalCount--) | Returns the total number of paths to delete. |
| [getSuccessCount()](#getSuccessCount--) | Returns the number of successfully deleted paths. |
| [getFailedCount()](#getFailedCount--) | Returns the number of paths not deleted due to errors. |
| [getErrors()](#getErrors--) | Returns descriptions of deletion errors. |
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Returns the results of deleting each path.

**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - The results of deleting each path.
### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Returns the total number of paths to delete.

**Returns:**
int - The total number of paths to delete.
### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Returns the number of successfully deleted paths.

**Returns:**
int - The number of successfully deleted paths.
### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Returns the number of paths not deleted due to errors.

**Returns:**
int - The number of paths not deleted due to errors.
### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Returns descriptions of deletion errors.

**Returns:**
java.lang.String[] - Descriptions of deletion errors.
