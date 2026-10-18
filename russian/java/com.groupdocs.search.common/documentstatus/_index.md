---
title: "DocumentStatus"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет статус обработки документа."
type: docs
weight: 40
url: /ru/java/com.groupdocs.search.common/documentstatus/
---
**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum DocumentStatus extends Enum<DocumentStatus>
```

Представляет статус обработки документа.

## Fields

| Field | Описание |
| --- | --- |
|  | [SuccessfullyProcessed](#SuccessfullyProcessed) | Документ успешно проиндексирован. |
|
|  | [Skipped](#Skipped) | Документ пропущен. |
|
|  | [ProcessedWithError](#ProcessedWithError) | Произошла ошибка при индексации документа. |
|
## Методы

| Метод | Описание |
| --- | --- |
| [values()](#values--) |  |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
### SuccessfullyProcessed {#SuccessfullyProcessed}
```
public static final DocumentStatus SuccessfullyProcessed
```


Документ успешно проиндексирован.


### Skipped {#Skipped}
```
public static final DocumentStatus Skipped
```


Документ пропущен.


### ProcessedWithError {#ProcessedWithError}
```
public static final DocumentStatus ProcessedWithError
```


Произошла ошибка при индексации документа.


### values() {#values--}
```
public static DocumentStatus[] values()
```




**Returns:**
com.groupdocs.search.common.DocumentStatus[]
### valueOf(String name) {#valueOf-java.lang.String-}
```
public static DocumentStatus valueOf(String name)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| имя | java.lang.String |  |

**Returns:**
[DocumentStatus](../../com.groupdocs.search.common/documentstatus)
