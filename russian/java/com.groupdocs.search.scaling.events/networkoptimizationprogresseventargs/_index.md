---
title: "NetworkOptimizationProgressEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события изменения прогресса операции оптимизации."
type: docs
weight: 15
url: /ru/java/com.groupdocs.search.scaling.events/networkoptimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs)
```
public class NetworkOptimizationProgressEventArgs extends EventArgs
```

Представляет аргументы события изменения прогресса операции оптимизации.

## Методы

| Метод | Описание |
| --- | --- |
|  | [getNodeIndex()](#getNodeIndex--) | Получает индекс узла поисковой сети. |
|
|  | [getServiceIndex()](#getServiceIndex--) | Получает индекс службы узла поисковой сети. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Получает количество обработанных сегментов. |
|
|  | [getTotalSegments()](#getTotalSegments--) | Получает общее количество сегментов для обработки. |
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

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Получает количество обработанных сегментов.


**Returns:**
int - Количество обработанных сегментов.

### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Получает общее количество сегментов для обработки.


**Returns:**
int - Общее количество сегментов для обработки.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Получает процент выполнения.


**Returns:**
double - Процент выполнения.

