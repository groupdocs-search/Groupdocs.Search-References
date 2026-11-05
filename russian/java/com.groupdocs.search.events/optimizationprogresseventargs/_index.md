---
title: "OptimizationProgressEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события обновления прогресса операции индексации."
type: docs
weight: 19
url: /ru/java/com.groupdocs.search.events/optimizationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OptimizationProgressEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события обновления прогресса операции индексации.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getTotalSegments()](#getTotalSegments--) | Получает общее количество сегментов для обработки. |
|
|  | [getProcessedSegments()](#getProcessedSegments--) | Получает количество обработанных сегментов. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Получает процент выполнения. |
|
### getTotalSegments() {#getTotalSegments--}
```
public final int getTotalSegments()
```


Получает общее количество сегментов для обработки.


**Returns:**
int - Общее количество сегментов для обработки.

### getProcessedSegments() {#getProcessedSegments--}
```
public final int getProcessedSegments()
```


Получает количество обработанных сегментов.


**Returns:**
int - Количество обработанных сегментов.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Получает процент выполнения.


**Returns:**
double - Процент выполнения.

