---
title: "DeleteResult"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет результат операции удаления проиндексированных файлов или папок из индекса."
type: docs
weight: 10
url: /ru/java/com.groupdocs.search.results/deleteresult/
---
**Inheritance:**
java.lang.Object
```
public class DeleteResult
```

Представляет результат операции удаления проиндексированных файлов или папок из индекса.


**Learn more**

* [Delete indexed paths](../https://docs.groupdocs.com/display/searchjava/Delete+indexed+paths)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getItemResults()](#getItemResults--) | Возвращает результаты удаления каждого пути. |
|
|  | [getTotalCount()](#getTotalCount--) | Возвращает общее количество путей для удаления. |
|
|  | [getSuccessCount()](#getSuccessCount--) | Возвращает количество успешно удалённых путей. |
|
|  | [getFailedCount()](#getFailedCount--) | Возвращает количество путей, не удалённых из‑за ошибок. |
|
|  | [getErrors()](#getErrors--) | Возвращает описания ошибок удаления. |
|
### getItemResults() {#getItemResults--}
```
public final PathDeleteResult[] getItemResults()
```


Возвращает результаты удаления каждого пути.


**Returns:**
com.groupdocs.search.results.PathDeleteResult[] - Результаты удаления каждого пути.

### getTotalCount() {#getTotalCount--}
```
public final int getTotalCount()
```


Возвращает общее количество путей для удаления.


**Returns:**
int - Общее количество путей для удаления.

### getSuccessCount() {#getSuccessCount--}
```
public final int getSuccessCount()
```


Возвращает количество успешно удалённых путей.


**Returns:**
int - Количество успешно удалённых путей.

### getFailedCount() {#getFailedCount--}
```
public final int getFailedCount()
```


Возвращает количество путей, не удалённых из‑за ошибок.


**Returns:**
int - Количество путей, не удалённых из-за ошибок.

### getErrors() {#getErrors--}
```
public final String[] getErrors()
```


Возвращает описания ошибок удаления.


**Returns:**
java.lang.String[] - Описания ошибок удаления.

