---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search for Java Riferimento API"
description: "Rappresenta gli argomenti per un evento di cambiamento dello stato della rete di ricerca."
type: docs
weight: 17
url: /it/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Rappresenta gli argomenti per un evento di cambiamento dello stato della rete di ricerca.

## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Restituisce lo stato precedente della rete di ricerca. |
|
|  | [getNewStatus()](#getNewStatus--) | Restituisce lo stato nuovo della rete di ricerca. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Restituisce lo stato precedente della rete di ricerca.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Restituisce lo stato nuovo della rete di ricerca.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

