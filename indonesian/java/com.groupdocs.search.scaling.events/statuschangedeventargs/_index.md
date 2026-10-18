---
title: "StatusChangedEventArgs"
second_title: "Referensi API GroupDocs.Search untuk Java"
description: "Mewakili argumen untuk peristiwa perubahan status jaringan pencarian."
type: docs
weight: 17
url: /id/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Mewakili argumen untuk peristiwa perubahan status jaringan pencarian.

## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Mendapatkan status jaringan pencarian lama. |
|
|  | [getNewStatus()](#getNewStatus--) | Mendapatkan status jaringan pencarian baru. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Mendapatkan status jaringan pencarian lama.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Mendapatkan status jaringan pencarian baru.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

