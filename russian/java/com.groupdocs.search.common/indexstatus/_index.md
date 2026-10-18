---
title: "IndexStatus"
second_title: "GroupDocs.Search для Java API Reference"
description: "Указывает статус индекса."
type: docs
weight: 41
url: /ru/java/com.groupdocs.search.common/indexstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum IndexStatus extends Enum<IndexStatus>
```

Указывает статус индекса.

## Fields

| Field | Описание |
| --- | --- |
|  | [Ready](#Ready) | Индекс свободен и готов к изменению. |
|
|  | [Failed](#Failed) | Индекс необходимо перезагрузить из‑за ошибки. |
|
|  | [Indexing](#Indexing) | Индекс выполняет операцию индексации. |
|
|  | [Updating](#Updating) | Индекс выполняет операцию обновления. |
|
|  | [Merging](#Merging) | Индекс выполняет операцию слияния. |
|
|  | [Optimizing](#Optimizing) | Индекс выполняет операцию оптимизации. |
|
|  | [Deleting](#Deleting) | Индекс выполняет операцию удаления. |
|
|  | [Renaming](#Renaming) | Индекс выполняет операцию переименования. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Индекс изменяет атрибуты. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final IndexStatus Ready
```


Индекс свободен и готов к изменению.


### Failed {#Failed}
```
public static final IndexStatus Failed
```


Индекс необходимо перезагрузить из‑за ошибки.


### Indexing {#Indexing}
```
public static final IndexStatus Indexing
```


Индекс выполняет операцию индексации.


### Updating {#Updating}
```
public static final IndexStatus Updating
```


Индекс выполняет операцию обновления.


### Merging {#Merging}
```
public static final IndexStatus Merging
```


Индекс выполняет операцию слияния.


### Optimizing {#Optimizing}
```
public static final IndexStatus Optimizing
```


Индекс выполняет операцию оптимизации.


### Deleting {#Deleting}
```
public static final IndexStatus Deleting
```


Индекс выполняет операцию удаления.


### Renaming {#Renaming}
```
public static final IndexStatus Renaming
```


Индекс выполняет операцию переименования.


### ChangingAttributes {#ChangingAttributes}
```
public static final IndexStatus ChangingAttributes
```


Индекс изменяет атрибуты.


### values() {#values--}
```
public static IndexStatus[] values()
```




**Returns:**
com.groupdocs.search.common.IndexStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static IndexStatus valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[IndexStatus](../../com.groupdocs.search.common/indexstatus)
