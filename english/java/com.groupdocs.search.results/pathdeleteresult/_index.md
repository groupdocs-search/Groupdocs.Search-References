---
title: PathDeleteResult
second_title: GroupDocs.Search for Java API Reference
description: Represents the result of the operation to delete an indexed file or folder from an index.
type: docs
weight: 18
url: /java/com.groupdocs.search.results/pathdeleteresult/
---
**Inheritance:**
java.lang.Object
```
public class PathDeleteResult
```

Represents the result of the operation to delete an indexed file or folder from an index.

**Learn more**

 *  [Delete indexed paths][]


[Delete indexed paths]: https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths
## Methods

| Method | Description |
| --- | --- |
| [isSuccess()](#isSuccess--) | Returns the success indicator of the delete operation. |
| [getError()](#getError--) | Returns a description of deletion error. |
| [getPath()](#getPath--) | Returns the path to the file or folder to delete. |
### isSuccess() {#isSuccess--}
```
public final boolean isSuccess()
```


Returns the success indicator of the delete operation.

**Returns:**
boolean -  true  if the delete operation was successful; otherwise, returns  false .
### getError() {#getError--}
```
public final String getError()
```


Returns a description of deletion error.

**Returns:**
java.lang.String - A description of deletion error.
### getPath() {#getPath--}
```
public final String getPath()
```


Returns the path to the file or folder to delete.

**Returns:**
java.lang.String - The path to the file or folder to delete.
