---
title: "MergeOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для операции слияния."
type: docs
weight: 28
url: /ru/java/com.groupdocs.search.options/mergeoptions/
---
**Inheritance:**
java.lang.Object
```
public class MergeOptions
```

Предоставляет параметры для операции слияния.


**Learn more**

* [Merge indexes](../https://docs.groupdocs.com/display/searchjava/Merge+indexes)
* [Optimize index](../https://docs.groupdocs.com/display/searchjava/Optimize+index)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [MergeOptions()](#MergeOptions--) | Инициализирует новый экземпляр класса MergeOptions. |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [isAsync()](#isAsync--) | Получает флаг асинхронного выполнения операции. |
|
|  | [setAsync(boolean value)](#setAsync-boolean-) | Устанавливает флаг асинхронного выполнения операции. |
|
|  | [getCancellation()](#getCancellation--) | Получает объект отмены операции. |
|
|  | [setCancellation(Cancellation value)](#setCancellation-com.groupdocs.search.common.Cancellation-) | Устанавливает объект отмены операции. |
|
### MergeOptions() {#MergeOptions--}
```
public MergeOptions()
```


Инициализирует новый экземпляр класса MergeOptions.


### isAsync() {#isAsync--}
```
public final boolean isAsync()
```


Получает флаг асинхронного выполнения операции. Значение по умолчанию — false.


**Returns:**
boolean — флаг асинхронного выполнения операции.

### setAsync(boolean value) {#setAsync-boolean-}
```
public final void setAsync(boolean value)
```


Устанавливает флаг асинхронного выполнения операции. Значение по умолчанию — false.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | boolean | Флаг асинхронного выполнения операции. |
|

### getCancellation() {#getCancellation--}
```
public final Cancellation getCancellation()
```


Получает объект отмены операции. Значение по умолчанию — null.


**Returns:**
[Cancellation](../../com.groupdocs.search.common/cancellation) - The operation cancellation object.

### setCancellation(Cancellation value) {#setCancellation-com.groupdocs.search.common.Cancellation-}
```
public final void setCancellation(Cancellation value)
```


Устанавливает объект отмены операции. Значение по умолчанию — null.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [Cancellation](../../com.groupdocs.search.common/cancellation) | Объект отмены операции. |
|

