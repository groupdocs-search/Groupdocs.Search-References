---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search för Java API-referens"
description: "Representerar argument för en händelse när söknätverkets status ändras."
type: docs
weight: 17
url: /sv/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Representerar argument för en händelse när söknätverkets status ändras.

## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Hämtar den gamla söknätsstatusen. |
|
|  | [getNewStatus()](#getNewStatus--) | Hämtar den nya söknätsstatusen. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Hämtar den gamla söknätsstatusen.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Hämtar den nya söknätsstatusen.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

