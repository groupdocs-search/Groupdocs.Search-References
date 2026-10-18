---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search für Java API-Referenz"
description: "Stellt Argumente für ein Ereignis zur Statusänderung des Suchnetzwerks dar."
type: docs
weight: 17
url: /de/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Stellt Argumente für ein Ereignis zur Statusänderung des Suchnetzwerks dar.

## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Ermittelt den alten Suchnetzwerk-Status. |
|
|  | [getNewStatus()](#getNewStatus--) | Ermittelt den neuen Suchnetzwerk-Status. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Ermittelt den alten Suchnetzwerk-Status.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Ermittelt den neuen Suchnetzwerk-Status.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

