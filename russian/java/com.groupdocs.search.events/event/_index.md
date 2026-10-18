---
title: "Event"
second_title: "GroupDocs.Search для Java API Reference"
description: "Этот класс предназначен для наследования при подписке на события."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.events/event/
---
**Inheritance:**
java.lang.Object
```
public abstract class Event<T>
```

Этот класс предназначен для наследования при подписке на события.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Event()](#Event--) | Инициализирует новый экземпляр класса  Event  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [add(T delegate)](#add-T-) | Добавляет слушателя для события. |
|
|  | [remove(T delegate)](#remove-T-) | Удаляет слушателя для события. |
|
|  | [isEmpty()](#isEmpty--) | Проверяет наличие хотя бы одного слушателя. |
|
### Event() {#Event--}
```
public Event()
```


Инициализирует новый экземпляр класса  Event  .


### add(T delegate) {#add-T-}
```
public final synchronized void add(T delegate)
```


Добавляет слушателя для события.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | delegate | T | Слушатель события для добавления. |
|

### remove(T delegate) {#remove-T-}
```
public final synchronized void remove(T delegate)
```


Удаляет слушателя для события.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | delegate | T | Слушатель события для удаления. |
|

### isEmpty() {#isEmpty--}
```
public synchronized boolean isEmpty()
```


Проверяет наличие хотя бы одного слушателя.


**Returns:**
boolean - Значение, указывающее, что хотя бы один слушатель добавлен для события.

