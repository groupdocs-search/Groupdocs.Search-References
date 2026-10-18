---
title: "StatusChangedEventArgs"
second_title: "Referencia de la API de GroupDocs.Search para Java"
description: "Representa los argumentos de un evento de cambio de estado de la red de búsqueda."
type: docs
weight: 17
url: /es/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Representa los argumentos de un evento de cambio de estado de la red de búsqueda.

## Métodos

| Método | Descripción |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Obtiene el estado anterior de la red de búsqueda. |
|
|  | [getNewStatus()](#getNewStatus--) | Obtiene el estado nuevo de la red de búsqueda. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Obtiene el estado anterior de la red de búsqueda.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Obtiene el estado nuevo de la red de búsqueda.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

