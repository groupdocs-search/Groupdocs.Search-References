---
title: "StatusChangedEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события изменения статуса поисковой сети."
type: docs
weight: 17
url: /ru/java/com.groupdocs.search.scaling.events/statuschangedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class StatusChangedEventArgs extends EventArgs
```

Представляет аргументы события изменения статуса поисковой сети.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getOldStatus()](#getOldStatus--) | Получает старый статус поисковой сети. |
|
|  | [getNewStatus()](#getNewStatus--) | Получает новый статус поисковой сети. |
|
### getOldStatus() {#getOldStatus--}
```
public final SearchNetworkStatus getOldStatus()
```


Получает старый статус поисковой сети.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The old search network status.

### getNewStatus() {#getNewStatus--}
```
public final SearchNetworkStatus getNewStatus()
```


Получает новый статус поисковой сети.


**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus) - The new search network status.

