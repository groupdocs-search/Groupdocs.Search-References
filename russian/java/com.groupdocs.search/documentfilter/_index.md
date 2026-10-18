---
title: "DocumentFilter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет базовый класс для фильтров документов."
type: docs
weight: 14
url: /ru/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Представляет базовый класс для фильтров документов. Содержит методы для создания экземпляров фильтров документов.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [toString()](#toString--) | Возвращает строковое представление фильтра документа. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Создаёт фильтр для пропуска документов с датой создания ранее нижней границы. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Создаёт фильтр для пропуска документов с датой создания позже верхней границы. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Создаёт фильтр для пропуска документов с датой создания вне указанного диапазона. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Создаёт фильтр для пропуска документов с датой изменения ранее нижней границы. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Создаёт фильтр для пропуска документов с датой изменения позже верхней границы. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Создаёт фильтр для пропуска документов с датой изменения вне указанного диапазона. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Создаёт фильтр для пропуска документов с длиной меньше нижней границы. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Создаёт фильтр для пропуска документов с длиной больше верхней границы. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Создаёт фильтр для пропуска документов вне указанного диапазона длины документов. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Создаёт фильтр для пропуска документов, не имеющих допустимое расширение. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Создаёт фильтр с обратной логикой относительно указанного внутреннего фильтра. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Создаёт логическую конъюнкцию указанных фильтров. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Создаёт логическую дизъюнкцию указанных фильтров. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Возвращает строковое представление фильтра документа.


**Returns:**
java.lang.String — строковое представление фильтра документа.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Создаёт фильтр для пропуска документов с датой создания ранее нижней границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Нижняя граница времени создания документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Создаёт фильтр для пропуска документов с датой создания позже верхней границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | upperBound | java.util.Date | Верхняя граница времени создания документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Создаёт фильтр для пропуска документов с датой создания вне указанного диапазона.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Нижняя граница времени создания документа. |
|
|  | upperBound | java.util.Date | Верхняя граница времени создания документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Создаёт фильтр для пропуска документов с датой изменения ранее нижней границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Нижняя граница времени изменения документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Создаёт фильтр для пропуска документов с датой изменения позже верхней границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | upperBound | java.util.Date | Верхняя граница времени изменения документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Создаёт фильтр для пропуска документов с датой изменения вне указанного диапазона.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Нижняя граница времени изменения документа. |
|
|  | upperBound | java.util.Date | Верхняя граница времени изменения документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. Регулярное выражение применяется к полному пути документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pattern | java.lang.String | Шаблон регулярного выражения. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. Регулярное выражение применяется к полному пути документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pattern | java.lang.String | Шаблон регулярного выражения. |
|
|  | options | int | Параметры регулярного выражения. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Создаёт фильтр для пропуска документов с длиной меньше нижней границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lowerBound | long | Нижняя граница длины документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Создаёт фильтр для пропуска документов с длиной больше верхней границы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | upperBound | long | Верхняя граница длины документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Создаёт фильтр для пропуска документов вне указанного диапазона длины документов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | lowerBound | long | Нижняя граница длины документа. |
|
|  | upperBound | long | Верхняя граница длины документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Создаёт фильтр для пропуска документов, не имеющих допустимое расширение.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Список допустимых расширений. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Создаёт фильтр с обратной логикой относительно указанного внутреннего фильтра.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Внутренний фильтр документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Создаёт логическую конъюнкцию указанных фильтров.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Фильтры документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Создаёт логическую дизъюнкцию указанных фильтров.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Фильтры документа. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

