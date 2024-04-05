---
title: OperationFinishedEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for the event of the indexing operation is finished.
type: docs
weight: 17
url: /java/com.groupdocs.search.events/operationfinishedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationFinishedEventArgs extends BaseIndexEventArgs
```

Represents arguments for the event of the indexing operation is finished.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getMessage()](#getMessage--) | Gets the message. |
| [getOperationType()](#getOperationType--) | Gets the operation type. |
### getMessage() {#getMessage--}
```
public final String getMessage()
```


Gets the message.

**Returns:**
java.lang.String - The message.
### getOperationType() {#getOperationType--}
```
public final OperationType getOperationType()
```


Gets the operation type.

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype) - The operation type.
