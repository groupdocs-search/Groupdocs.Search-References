---
title: MergeOptions
second_title: GroupDocs.Search for Java API Reference
description: Provides options for merge operation.
type: docs
weight: 28
url: /java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Provides options for merge operation.

**Learn more**

 *  [Merge indexes][]
 *  [Optimize index][]


[Merge indexes]: https://docs.groupdocs.com/display/searchjava/Merge+indexes
[Optimize index]: https://docs.groupdocs.com/display/searchjava/Optimize+index
## Constructors

| Constructor | Description |
| --- | --- |
| [MergeOptions()](#MergeOptions--) | Initializes a new instance of the  MergeOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [isAsync()](#isAsync--) | Gets the flag of asynchronous performing the operation. |
| [setAsync(boolean value)](#setAsync-boolean-) | Sets the flag of asynchronous performing the operation. |
| [getCancellation()](#getCancellation--) | Gets the operation cancellation object. |
| [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Sets the operation cancellation object. |
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Initializes a new instance of the  MergeOptions  class.

### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Gets the flag of asynchronous performing the operation. The default value is  false .

**Returns:**
boolean - The flag of asynchronous performing the operation.
### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Sets the flag of asynchronous performing the operation. The default value is  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The flag of asynchronous performing the operation. |

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Gets the operation cancellation object. The default value is  null .

**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.
### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Sets the operation cancellation object. The default value is  null .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cancellation](../../com.groupdocs.search.common/cancellation) | The operation cancellation object. |

