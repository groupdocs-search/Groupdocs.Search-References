---
title: "DocumentIndexedEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события завершения индексации документа."
type: docs
weight: 12
url: /ru/java/com.groupdocs.search.scaling.events/documentindexedeventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class DocumentIndexedEventArgs extends EventArgs
```

Представляет аргументы события завершения индексации документа.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getShardIndex()](#getShardIndex--) | Получает индекс шарда. |
|
|  | [getDocumentKey()](#getDocumentKey--) | Получает ключ документа. |
|
### getShardIndex() {#getShardIndex--}
```
public final int getShardIndex()
```


Получает индекс шарда.


**Returns:**
int - Индекс шарда.

### getDocumentKey() {#getDocumentKey--}
```
public final String getDocumentKey()
```


Получает ключ документа.


**Returns:**
java.lang.String - Ключ документа.

