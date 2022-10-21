---
title: BaseIndexEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents the base class of event arguments.
type: docs
weight: 10
url: /java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object
```
public class BaseIndexEventArgs
```

Represents the base class of event arguments.

**Learn more**

 *  [Search index events][]


[Search index events]: https://docs.groupdocs.com/display/searchjava/Search+index+events
## Methods

| Method | Description |
| --- | --- |
| [getTime()](#getTime--) | Gets the time of an event. |
| [getIndexId()](#getIndexId--) | Gets the index ID. |
| [getIndexFolder()](#getIndexFolder--) | Gets the index folder. |
| [getStatus()](#getStatus--) | Gets the index status. |
### getTime() {#getTime--}
```
public final Date getTime()
```


Gets the time of an event.

**Returns:**
java.util.Date - The time of an event.
### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Gets the index ID.

**Returns:**
java.util.UUID - The index ID.
### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Gets the index folder.

**Returns:**
java.lang.String - The index folder.
### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Gets the index status.

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.
