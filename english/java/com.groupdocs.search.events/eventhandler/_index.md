---
title: EventHandler
second_title: GroupDocs.Search for Java API Reference
description: Represents the base class of an event handler.
type: docs
weight: 12
url: /java/com.groupdocs.search.events/eventhandler/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.common.Delegate](../../com.groupdocs.search.common/delegate), [com.groupdocs.search.common.MulticastDelegate](../../com.groupdocs.search.common/multicastdelegate)
```
public abstract class EventHandler<T> extends MulticastDelegate
```

Represents the base class of an event handler.
## Constructors

| Constructor | Description |
| --- | --- |
| [EventHandler()](#EventHandler--) |  |
## Methods

| Method | Description |
| --- | --- |
| [invoke(Object sender, T args)](#invoke-java.lang.Object-T-) | Starts handling of the event. |
### EventHandler() {#EventHandler--}
```
public EventHandler()
```


### invoke(Object sender, T args) {#invoke-java.lang.Object-T-}
```
public abstract void invoke(Object sender, T args)
```


Starts handling of the event.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sender | java.lang.Object | The sender of the event. |
| args | T | Arguments of the event. |

