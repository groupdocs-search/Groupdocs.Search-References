---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search для Java API Reference"
description: "Содержит методы для создания фильтров поисковых документов."
type: docs
weight: 24
url: /ru/java/com.groupdocs.search/searchdocumentfilter/
---
**Inheritance:**
java.lang.Object
```
public class SearchDocumentFilter
```

Содержит методы для создания фильтров поисковых документов.


**Learn more**

* [Document filtering in search result](../https://docs.groupdocs.com/display/searchjava/Document+filtering+in+search+result)
* [Search options](../https://docs.groupdocs.com/display/searchjava/Search+options)

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [SearchDocumentFilter()](#SearchDocumentFilter--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Создаёт фильтр для пропуска документов, которые не находятся в указанном списке возможных расширений. |
|
|  | [createNot(ISearchDocumentFilter innerFilter)](#createNot-com.groupdocs.search.options.ISearchDocumentFilter-) | Создаёт фильтр с обратной логикой относительно указанного внутреннего фильтра. |
|
|  | [createAnd(ISearchDocumentFilter[] filters)](#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-) | Создаёт логическую конъюнкцию указанных фильтров. |
|
|  | [createOr(ISearchDocumentFilter[] filters)](#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-) | Создаёт логическую дизъюнкцию указанных фильтров. |
|
|  | [createAttribute(String[] attributes)](#createAttribute-java.lang.String...-) | Создаёт фильтр для пропуска документов, которые не имеют ни одного значения из указанного списка допустимых атрибутов. |
|
### SearchDocumentFilter() {#SearchDocumentFilter--}
```
public SearchDocumentFilter()
```


### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern)
```


Создаёт фильтр для пропуска документов, которые не соответствуют регулярному выражению. Регулярное выражение применяется к полному пути документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | pattern | java.lang.String | Шаблон регулярного выражения. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static ISearchDocumentFilter createFilePathRegularExpression(String pattern, int options)
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
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by file name.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static ISearchDocumentFilter createFileExtension(String[] extensions)
```


Создаёт фильтр для пропуска документов, которые не находятся в указанном списке возможных расширений.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Список возможных расширений. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document extension.

### createNot(ISearchDocumentFilter innerFilter) {#createNot-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public static ISearchDocumentFilter createNot(ISearchDocumentFilter innerFilter)
```


Создаёт фильтр с обратной логикой относительно указанного внутреннего фильтра.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | innerFilter | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Внутренний фильтр поискового документа. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - An inverted search document filter.

### createAnd(ISearchDocumentFilter[] filters) {#createAnd-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createAnd(ISearchDocumentFilter[] filters)
```


Создаёт логическую конъюнкцию указанных фильтров.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Фильтры поискового документа. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of conjunction of the specified filters.

### createOr(ISearchDocumentFilter[] filters) {#createOr-com.groupdocs.search.options.ISearchDocumentFilter...-}
```
public static ISearchDocumentFilter createOr(ISearchDocumentFilter[] filters)
```


Создаёт логическую дизъюнкцию указанных фильтров.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | filters | [ISearchDocumentFilter\[\]](../../com.groupdocs.search.options/isearchdocumentfilter) | Фильтры поискового документа. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter that represents result of disjunction of the specified filters.

### createAttribute(String[] attributes) {#createAttribute-java.lang.String...-}
```
public static ISearchDocumentFilter createAttribute(String[] attributes)
```


Создаёт фильтр для пропуска документов, которые не имеют ни одного значения из указанного списка допустимых атрибутов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | атрибуты | java.lang.String[] | Список допустимых атрибутов. |
|

**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - A search document filter by document attribute.

