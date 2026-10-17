---
title: "StatusChangedEventArgs"
second_title: "مرجع API لـ GroupDocs.Search للـ Java"
description: "يمثل المعلمات لحدث تغيير حالة شبكة البحث."
type: docs
weight: 17
url: /ar/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

يمثل المعلمات لحدث تغيير حالة شبكة البحث.

## طرق

| طريقة | الوصف |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | يحصل على حالة شبكة البحث القديمة. |
|
|  | [getNewStatus()](#getNewStatus--) | يحصل على حالة شبكة البحث الجديدة. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


يحصل على حالة شبكة البحث القديمة.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


يحصل على حالة شبكة البحث الجديدة.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

