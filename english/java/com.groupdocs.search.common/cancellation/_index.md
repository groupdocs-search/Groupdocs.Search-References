---
title: Cancellation
second_title: GroupDocs.Search for Java API Reference
description: Represents an object for requesting cancellation of an operation.
type: docs
weight: 11
url: /java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Represents an object for requesting cancellation of an operation.

**Learn more**

 *  [Indexing options][]
 *  [Search options][]


[Indexing options]: https://docs.groupdocs.com/display/searchjava/Indexing+options
[Search options]: https://docs.groupdocs.com/display/searchjava/Search+options
## Constructors

| Constructor | Description |
| --- | --- |
| [Cancellation()](#Cancellation--) | Initializes a new instance of the  Cancellation  class. |
## Methods

| Method | Description |
| --- | --- |
| [isCancelled()](#isCancelled--) | Gets a value indicating that cancellation has been requested. |
| [cancel()](#cancel--) | Makes a request for cancellation. |
| [cancelAfter(int milliseconds)](#cancelAfter-int-) | Makes a request for cancellation after the expiration of specified number of milliseconds. |
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Initializes a new instance of the  Cancellation  class.

### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Gets a value indicating that cancellation has been requested.

**Returns:**
boolean - A value indicating that cancellation has been requested.
### cancel() {#cancel--}
```
public final void cancel()
```


Makes a request for cancellation.

### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Makes a request for cancellation after the expiration of specified number of milliseconds.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| milliseconds | int | The number of milliseconds after which an operation will be cancelled. |

