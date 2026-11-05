---
title: "Отмена"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет объект для запроса отмены операции."
type: docs
weight: 11
url: /ru/java/com.groupdocs.search.common/cancellation/
---
**Inheritance:**
java.lang.Object
```
public class Cancellation
```

Представляет объект для запроса отмены операции.


**Learn more**

* [Indexing options](../https://docs.groupdocs.com/display/searchjava/Indexing+options)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Cancellation()](#Cancellation--) | Инициализирует новый экземпляр |
Отмена
класс.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isCancelled()](#isCancelled--) | Получает значение, указывающее, что запрос на отмену был сделан. |
|
|  | [cancel()](#cancel--) | Отправляет запрос на отмену. |
|
|  | [cancelAfter(int milliseconds)](#cancelAfter-int-) | Отправляет запрос на отмену после истечения указанного количества миллисекунд. |
|
### Cancellation() {#Cancellation--}
```
public Cancellation()
```


Инициализирует новый экземпляр
Отмена
класс.


### isCancelled() {#isCancelled--}
```
public final boolean isCancelled()
```


Получает значение, указывающее, что запрос на отмену был сделан.


**Returns:**
boolean - Значение, указывающее, что запрос на отмену был сделан.

### cancel() {#cancel--}
```
public final void cancel()
```


Отправляет запрос на отмену.


### cancelAfter(int milliseconds) {#cancelAfter-int-}
```
public final void cancelAfter(int milliseconds)
```


Отправляет запрос на отмену после истечения указанного количества миллисекунд.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | миллисекунды | int | Количество миллисекунд, после которых операция будет отменена. |
|

