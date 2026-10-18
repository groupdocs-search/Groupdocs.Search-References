---
title: "ImageSearchOptions"
second_title: "GroupDocs.Search для Java API Reference"
description: "Предоставляет параметры для операции обратного поиска изображений."
type: docs
weight: 24
url: /ru/java/com.groupdocs.search.options/imagesearchoptions/
---
**Inheritance:**
java.lang.Object
```
public class ImageSearchOptions
```

Предоставляет параметры для операции обратного поиска изображений.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [ImageSearchOptions()](#ImageSearchOptions--) | Инициализирует новый экземпляр класса  ImageSearchOptions  . |
|
|  | [ImageSearchOptions(Object data)](#ImageSearchOptions-java.lang.Object-) | Инициализирует новый экземпляр класса  ImageSearchOptions  . |
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getHashDifferences()](#getHashDifferences--) | Получает максимальное количество несовпадающих битов в хэше изображения. |
|
|  | [setHashDifferences(int value)](#setHashDifferences-int-) | Устанавливает максимальное количество несовпадающих битов в хэше изображения. |
|
|  | [getMaxResultCount()](#getMaxResultCount--) | Получает максимальное количество найденных изображений для запроса обратного поиска изображения. |
|
|  | [setMaxResultCount(int value)](#setMaxResultCount-int-) | Устанавливает максимальное количество найденных изображений для запроса обратного поиска изображения. |
|
|  | [getSearchDocumentFilter()](#getSearchDocumentFilter--) | Получает фильтр поискового документа. |
|
|  | [setSearchDocumentFilter(ISearchDocumentFilter value)](#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-) | Получает или устанавливает фильтр поискового документа. |
|
| [getCore()](#getCore--) |  |
### ImageSearchOptions() {#ImageSearchOptions--}
```
public ImageSearchOptions()
```


Инициализирует новый экземпляр класса  ImageSearchOptions  .


### ImageSearchOptions(Object data) {#ImageSearchOptions-java.lang.Object-}
```
public ImageSearchOptions(Object data)
```


Инициализирует новый экземпляр класса  ImageSearchOptions  .


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | данные | java.lang.Object | Сериализованные данные. |
|

### getHashDifferences() {#getHashDifferences--}
```
public int getHashDifferences()
```


Получает максимальное количество несовпадающих битов в хэше изображения. Значение по умолчанию равно  5 .


**Returns:**
int - Максимальное количество несовпадающих битов в хэше изображения.

### setHashDifferences(int value) {#setHashDifferences-int-}
```
public void setHashDifferences(int value)
```


Устанавливает максимальное количество несовпадающих битов в хэше изображения. Значение по умолчанию — 5.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество несовпадающих битов в хэше изображения. |
|

### getMaxResultCount() {#getMaxResultCount--}
```
public int getMaxResultCount()
```


Получает максимальное количество найденных изображений для запроса обратного поиска изображения. Значение по умолчанию — 1000.


**Returns:**
int - Максимальное количество найденных изображений для запроса обратного поиска изображения.

### setMaxResultCount(int value) {#setMaxResultCount-int-}
```
public void setMaxResultCount(int value)
```


Устанавливает максимальное количество найденных изображений для запроса обратного поиска изображения. Значение по умолчанию — 1000.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | значение | int | Максимальное количество найденных изображений для запроса обратного поиска изображения. |
|

### getSearchDocumentFilter() {#getSearchDocumentFilter--}
```
public ISearchDocumentFilter getSearchDocumentFilter()
```


Получает фильтр документов поиска. SearchDocumentFilter работает по логике включения. Используйте класс GroupDocs.Search.Options.SearchDocumentFilter для создания экземпляров фильтра документов поиска. Значение по умолчанию — null, что означает, что будут возвращены все найденные документы.


**Returns:**
[ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) - The search document filter.

### setSearchDocumentFilter(ISearchDocumentFilter value) {#setSearchDocumentFilter-com.groupdocs.search.options.ISearchDocumentFilter-}
```
public void setSearchDocumentFilter(ISearchDocumentFilter value)
```


Получает или задает фильтр документов поиска. SearchDocumentFilter работает по логике включения. Используйте класс GroupDocs.Search.Options.SearchDocumentFilter для создания экземпляров фильтра документов поиска. Значение по умолчанию — null, что означает, что будут возвращены все найденные документы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | value | [ISearchDocumentFilter](../../com.groupdocs.search.options/isearchdocumentfilter) | Фильтр документов поиска. |
|

### getCore() {#getCore--}
```
public Object getCore()
```




**Returns:**
java.lang.Object
