---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search for Java API Referansı"
description: "Arama ağı durum değişikliği olayının argümanlarını temsil eder."
type: docs
weight: 17
url: /tr/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Arama ağı durum değişikliği olayının argümanlarını temsil eder.

## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Eski arama ağı durumunu alır. |
|
|  | [getNewStatus()](#getNewStatus--) | Yeni arama ağı durumunu alır. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Eski arama ağı durumunu alır.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Yeni arama ağı durumunu alır.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

