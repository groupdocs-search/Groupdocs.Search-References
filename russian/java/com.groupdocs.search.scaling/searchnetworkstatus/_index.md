---
title: "SearchNetworkStatus"
second_title: "GroupDocs.Search для Java API Reference"
description: "Указывает статус поисковой сети."
type: docs
weight: 13
url: /ru/java/com.groupdocs.search.scaling/searchnetworkstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum SearchNetworkStatus extends Enum<SearchNetworkStatus>
```

Указывает статус поисковой сети.

## Fields

| Field | Описание |
| --- | --- |
|  | [Ready](#Ready) | Поисковая сеть свободна и готова к изменениям. |
|
|  | [Configuring](#Configuring) | Поисковая сеть выполняет операцию конфигурирования. |
|
|  | [Indexing](#Indexing) | Поисковая сеть выполняет операцию индексации. |
|
|  | [Optimizing](#Optimizing) | Поисковая сеть выполняет операцию оптимизации. |
|
|  | [Deleting](#Deleting) | Поисковая сеть выполняет операцию удаления. |
|
|  | [ChangingAttributes](#ChangingAttributes) | Поисковая сеть изменяет атрибуты. |
|
|  | [Synchronizing](#Synchronizing) | Поисковая сеть выполняет операцию синхронизации. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### Ready {#Ready}
```
public static final SearchNetworkStatus Ready
```


Поисковая сеть свободна и готова к изменениям.


### Configuring {#Configuring}
```
public static final SearchNetworkStatus Configuring
```


Поисковая сеть выполняет операцию конфигурирования.


### Indexing {#Indexing}
```
public static final SearchNetworkStatus Indexing
```


Поисковая сеть выполняет операцию индексации.


### Optimizing {#Optimizing}
```
public static final SearchNetworkStatus Optimizing
```


Поисковая сеть выполняет операцию оптимизации.


### Deleting {#Deleting}
```
public static final SearchNetworkStatus Deleting
```


Поисковая сеть выполняет операцию удаления.


### ChangingAttributes {#ChangingAttributes}
```
public static final SearchNetworkStatus ChangingAttributes
```


Поисковая сеть изменяет атрибуты.


### Synchronizing {#Synchronizing}
```
public static final SearchNetworkStatus Synchronizing
```


Поисковая сеть выполняет операцию синхронизации.


### values() {#values--}
```
public static SearchNetworkStatus[] values()
```




**Returns:**
com.groupdocs.search.scaling.SearchNetworkStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static SearchNetworkStatus valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[SearchNetworkStatus](../../com.groupdocs.search.scaling/searchnetworkstatus)
