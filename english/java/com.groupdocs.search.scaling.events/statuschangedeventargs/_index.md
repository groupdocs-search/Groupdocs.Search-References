---
title: StatusChangedEventArgs
second_title: GroupDocs.Search for Java API Reference
description: Represents arguments for a search network status change event.
type: docs
weight: 17
url: /java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Represents arguments for a search network status change event.
## Methods

| Method | Description |
| --- | --- |
| [getOldStatus()](#getOldStatus--) | Gets the old search network status. |
| [getNewStatus()](#getNewStatus--) | Gets the new search network status. |
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Gets the old search network status.

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.
### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Gets the new search network status.

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.
