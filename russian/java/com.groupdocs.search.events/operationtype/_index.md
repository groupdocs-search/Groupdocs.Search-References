---
title: "OperationType"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет тип операции индекса."
type: docs
weight: 23
url: /ru/java/com.groupdocs.search.events/operationtype/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum OperationType extends Enum<OperationType>
```

Представляет тип операции индекса.

## Fields

| Field | Описание |
| --- | --- |
|  | [Indexing](#Indexing) | Добавление документов в индекс. |
|
|  | [Updating](#Updating) | Обновление документов в индексе. |
|
|  | [Merging](#Merging) | Объединение индексов. |
|
|  | [Optimizing](#Optimizing) | Оптимизация индекса. |
|
|  | [Deleting](#Deleting) | Удаление путей из индекса. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Indexing {#Indexing}
```
public static final OperationType Indexing
```


Добавление документов в индекс.


### Updating {#Updating}
```
public static final OperationType Updating
```


Обновление документов в индексе.


### Merging {#Merging}
```
public static final OperationType Merging
```


Объединение индексов.


### Optimizing {#Optimizing}
```
public static final OperationType Optimizing
```


Оптимизация индекса.


### Deleting {#Deleting}
```
public static final OperationType Deleting
```


Удаление путей из индекса.


### values() {#values--}
```
public static OperationType[] values()
```




**Returns:**
com.groupdocs.search.events.OperationType[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static OperationType valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[OperationType](../../com.groupdocs.search.events/operationtype)
