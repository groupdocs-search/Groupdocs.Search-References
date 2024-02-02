---
title: ErrorOccurredEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of an error occurs in one of the nodes of the search network.
type: docs
weight: 13
url: /java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Represents arguments for the event of an error occurs in one of the nodes of the search network.
## Methods

| Method | Description |
| --- | --- |
| [getNodeIndex()](#getNodeIndex--) | Gets the index of the search network node. |
| [getServiceIndex()](#getServiceIndex--) | Gets the index of the search network node service. |
| [getMessage()](#getMessage--) | Gets the error message. |
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
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Gets the error message.

**Returns:**
java.lang.String - The error message.
