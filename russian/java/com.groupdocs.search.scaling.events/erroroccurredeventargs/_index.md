---
title: "ErrorOccurredEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события возникновения ошибки в одном из узлов поисковой сети."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search.scaling.events/erroroccurredeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class ErrorOccurredEventArgs extends EventArgs
```

Представляет аргументы события возникновения ошибки в одном из узлов поисковой сети.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Получает индекс узла поисковой сети. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Получает индекс службы узла поисковой сети. |
|
|  | [getMessage()](#getMessage--) | Получает сообщение об ошибке. |
|
### getNodeIndex() {#getNodeIndex--}
```
public final int getNodeIndex()
```


Получает индекс узла поисковой сети.


**Returns:**
int - Индекс узла поисковой сети.

### getServiceIndex() {#getServiceIndex--}
```
public final int getServiceIndex()
```


Получает индекс службы узла поисковой сети.


**Returns:**
int - Индекс службы узла поисковой сети.

### getMessage() {#getMessage--}
```
public final String getMessage()
```


Получает сообщение об ошибке.


**Returns:**
java.lang.String - Сообщение об ошибке.

