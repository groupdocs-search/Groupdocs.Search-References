---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет аргументы события обновления прогресса операции индексации."
type: docs
weight: 18
url: /ru/java/com.groupdocs.search.events/operationprogresseventargs/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.search.events.EventArgs](../../com.groupdocs.search.events/eventargs), [com.groupdocs.search.events.BaseIndexEventArgs](../../com.groupdocs.search.events/baseindexeventargs)
```
public class OperationProgressEventArgs extends BaseIndexEventArgs
```

Представляет аргументы события обновления прогресса операции индексации.


**Learn more**

* [Search index events](../https://docs.groupdocs.com/display/searchjava/Search+index+events)

## Методы

| Метод | Описание |
| --- | --- |
|  | [getTotalDocuments()](#getTotalDocuments--) | Получает общее количество документов для обработки. |
|
|  | [getProcessedDocuments()](#getProcessedDocuments--) | Получает количество успешно обработанных документов. |
|
|  | [getSkippedDocuments()](#getSkippedDocuments--) | Получает количество пропущенных документов. |
|
|  | [getProgressPercentage()](#getProgressPercentage--) | Получает процент выполнения. |
|
|  | [getLastDocumentKey()](#getLastDocumentKey--) | Получает ключ последнего обработанного документа. |
|
|  | [getLastDocumentPath()](#getLastDocumentPath--) | Получает путь к последнему обработанному документу. |
|
|  | [getLastDocumentStatus()](#getLastDocumentStatus--) | Получает статус последнего обработанного документа. |
|
### getTotalDocuments() {#getTotalDocuments--}
```
public final int getTotalDocuments()
```


Получает общее количество документов для обработки.


**Returns:**
int - Общее количество документов для обработки.

### getProcessedDocuments() {#getProcessedDocuments--}
```
public final int getProcessedDocuments()
```


Получает количество успешно обработанных документов.


**Returns:**
int - Количество успешно обработанных документов.

### getSkippedDocuments() {#getSkippedDocuments--}
```
public final int getSkippedDocuments()
```


Получает количество пропущенных документов.


**Returns:**
int - Количество пропущенных документов.

### getProgressPercentage() {#getProgressPercentage--}
```
public final double getProgressPercentage()
```


Получает процент выполнения.


**Returns:**
double - Процент выполнения.

### getLastDocumentKey() {#getLastDocumentKey--}
```
public final String getLastDocumentKey()
```


Получает ключ последнего обработанного документа.


**Returns:**
java.lang.String - Ключ последнего обработанного документа.

### getLastDocumentPath() {#getLastDocumentPath--}
```
public final String getLastDocumentPath()
```


Получает путь к последнему обработанному документу.


**Returns:**
java.lang.String - Путь к последнему обработанному документу.

### getLastDocumentStatus() {#getLastDocumentStatus--}
```
public final DocumentStatus getLastDocumentStatus()
```


Получает статус последнего обработанного документа.


**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus) - The last processed document status.

