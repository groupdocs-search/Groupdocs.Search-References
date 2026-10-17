---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search pour Java Référence API"
description: "Représente les arguments d'un événement de changement d'état du réseau de recherche."
type: docs
weight: 17
url: /fr/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Représente les arguments d'un événement de changement d'état du réseau de recherche.

## Méthodes

| Méthode | Description |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Obtient l'ancien statut du réseau de recherche. |
|
|  | [getNewStatus()](#getNewStatus--) | Obtient le nouveau statut du réseau de recherche. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Obtient l'ancien statut du réseau de recherche.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Obtient le nouveau statut du réseau de recherche.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

