---
title: "BaseIndexEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет базовый класс аргументов события."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.events/baseindexeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class BaseIndexEventArgs extends EventArgs
```

Представляет базовый класс аргументов события.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getTime()](#getTime--) | Получает время события. |
|
|  | [getIndexId()](#getIndexId--) | Получает идентификатор индекса. |
|
|  | [getIndexFolder()](#getIndexFolder--) | Получает папку индекса. |
|
|  | [getStatus()](#getStatus--) | Получает статус индекса. |
|
### getTime() {#getTime--}
```
public final Date getTime()
```


Получает время события.


**Returns:**
java.util.Date - Время события.

### getIndexId() {#getIndexId--}
```
public final UUID getIndexId()
```


Получает идентификатор индекса.


**Returns:**
java.util.UUID - Идентификатор индекса.

### getIndexFolder() {#getIndexFolder--}
```
public final String getIndexFolder()
```


Получает папку индекса.


**Returns:**
java.lang.String - Папка индекса.

### getStatus() {#getStatus--}
```
public final IndexStatus getStatus()
```


Получает статус индекса.


**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus) - The index status.

