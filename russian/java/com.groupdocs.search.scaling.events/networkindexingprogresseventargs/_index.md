---
title: "NetworkIndexingProgressEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события изменения прогресса операции индексации."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search.scaling.events/networkindexingprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkIndexingProgressEventArgs extends EventArgs
```

Представляет аргументы события изменения прогресса операции индексации.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Получает индекс узла поисковой сети. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Получает индекс службы узла поисковой сети. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Получает количество обработанных документов. |
|
|  | [getTotalDocuments()](#getTotalDocuments--) | Получает общее количество документов для обработки. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Получает процент выполнения. |
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

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Получает количество обработанных документов.


**Returns:**
int - Количество обработанных документов.

### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Получает общее количество документов для обработки.


**Returns:**
int - Общее количество документов для обработки.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Получает процент выполнения.


**Returns:**
double - Процент выполнения.

