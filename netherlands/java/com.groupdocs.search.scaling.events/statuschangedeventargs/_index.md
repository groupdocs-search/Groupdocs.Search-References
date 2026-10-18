---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search for Java API-referentie"
description: "Stelt de argumenten voor een zoeknetwerkstatus‑veranderings‑evenement voor."
type: docs
weight: 17
url: /nl/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Stelt de argumenten voor een zoeknetwerkstatus‑veranderings‑evenement voor.

## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Haalt de oude status van het zoeknetwerk op. |
|
|  | [getNewStatus()](#getNewStatus--) | Haalt de nieuwe status van het zoeknetwerk op. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Haalt de oude status van het zoeknetwerk op.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Haalt de nieuwe status van het zoeknetwerk op.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

