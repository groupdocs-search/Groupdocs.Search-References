---
title: Event
second_title: GroupDocs.Search for Java API Reference
description: This class is intended to be inherited when subscribing to events.
type: docs
weight: 11
url: /java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

This class is intended to be inherited when subscribing to events.
## Constructors

| Constructor | Description |
| --- | --- |
| [Event()](#Event--) | Initializes a new instance of the  Event  class. |
## Methods

| Method | Description |
| --- | --- |
| [add(T delegate)](#add-T-) | Adds a listener for the event. |
| [remove(T delegate)](#remove-T-) | Removes a listener for the event. |
| [isEmpty()](#isEmpty--) | Checks for presence of at least one listener. |
### Event() {#Event--}
```
public Event()
```


Initializes a new instance of the  Event  class.

### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Adds a listener for the event.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| delegate | T | A listener for the event to add. |

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Removes a listener for the event.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| delegate | T | A listener for the event to remove. |

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Checks for presence of at least one listener.

**Returns:**
boolean - A value indicating that at least one listener added for the event.
