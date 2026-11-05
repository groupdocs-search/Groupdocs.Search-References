---
title: "Searcher"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет сервис, управляющий поисковыми запросами к шардам поисковой сети."
type: docs
weight: 12
url: /ru/java/com.groupdocs.search.scaling/searcher/
---
**Inheritance:**
java.lang.Object
```
public abstract class Searcher
```

Представляет сервис, управляющий поисковыми запросами к шардам поисковой сети.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Searcher()](#Searcher--) |  |
## Методы

| Метод | Описание |
| --- | --- |
|  | [searchFirst(String query, SearchOptions options)](#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Запускает поиск с запросом в текстовой форме в распределённом поисковом индексе. |
|
|  | [searchFirst(SearchQuery query, SearchOptions options)](#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Запускает поиск в распределённом поисковом индексе. |
|
|  | [searchFirst(SearchImage image, ImageSearchOptions options)](#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Выполняет обратный поиск по изображению в распределённом поисковом индексе. |
|
|  | [searchNext(NetworkSearchToken networkSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-) | Продолжает поиск в распределённом поисковом индексе. |
|
|  | [searchNext(NetworkImageSearchToken networkImageSearchToken)](#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-) | Продолжает обратный поиск по изображению в распределённом поисковом индексе. |
|
|  | [highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Генерирует текст в формате HTML с выделенными найденными терминами. |
|
|  | [getIndexedDocuments(int shardIndex)](#getIndexedDocuments-int-) | Получает массив всех проиндексированных документов. |
|
|  | [getIndexedDocumentItems(NetworkDocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-) | Получает массив вложенных элементов указанного документа (для контейнерных документов, таких как ZIP, OST, PST). |
|
|  | [getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Генерирует текст проиндексированного документа и передаёт его через выходной адаптер. |
|
### Searcher() {#Searcher--}
```
public Searcher()
```


### searchFirst(String query, SearchOptions options) {#searchFirst-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(String query, SearchOptions options)
```


Запускает поиск с запросом в текстовой форме в распределённом поисковом индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | java.lang.String | Запрос поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchQuery query, SearchOptions options) {#searchFirst-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public abstract NetworkSearchResult searchFirst(SearchQuery query, SearchOptions options)
```


Запускает поиск в распределённом поисковом индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchFirst(SearchImage image, ImageSearchOptions options) {#searchFirst-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public abstract NetworkImageSearchResult searchFirst(SearchImage image, ImageSearchOptions options)
```


Выполняет обратный поиск по изображению в распределённом поисковом индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Изображение для поиска. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Параметры поиска изображения. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### searchNext(NetworkSearchToken networkSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkSearchToken-}
```
public abstract NetworkSearchResult searchNext(NetworkSearchToken networkSearchToken)
```


Продолжает поиск в распределённом поисковом индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | networkSearchToken | [NetworkSearchToken](../../com.groupdocs.search.scaling.results/networksearchtoken) | Токен поиска в сети. |
|

**Returns:**
[NetworkSearchResult](../../com.groupdocs.search.scaling.results/networksearchresult) - The search result.

### searchNext(NetworkImageSearchToken networkImageSearchToken) {#searchNext-com.groupdocs.search.scaling.results.NetworkImageSearchToken-}
```
public abstract NetworkImageSearchResult searchNext(NetworkImageSearchToken networkImageSearchToken)
```


Продолжает обратный поиск по изображению в распределённом поисковом индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | networkImageSearchToken | [NetworkImageSearchToken](../../com.groupdocs.search.scaling.results/networkimagesearchtoken) | Токен поиска изображений в сети. |
|

**Returns:**
[NetworkImageSearchResult](../../com.groupdocs.search.scaling.results/networkimagesearchresult) - The reverse image search result.

### highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.scaling.results.NetworkFoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public abstract void highlight(NetworkFoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Генерирует текст в формате HTML с выделенными найденными терминами.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | [NetworkFoundDocument](../../com.groupdocs.search.scaling.results/networkfounddocument) | Найденный документ. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Подсветка результатов поиска. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Параметры подсветки. |
|

### getIndexedDocuments(int shardIndex) {#getIndexedDocuments-int-}
```
public abstract NetworkDocumentInfo[] getIndexedDocuments(int shardIndex)
```


Получает массив всех проиндексированных документов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | shardIndex | int | Индекс шарда. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - массив всех проиндексированных документов.

### getIndexedDocumentItems(NetworkDocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.scaling.results.NetworkDocumentInfo-}
```
public abstract NetworkDocumentInfo[] getIndexedDocumentItems(NetworkDocumentInfo documentInfo)
```


Получает массив вложенных элементов указанного документа (для контейнерных документов, таких как ZIP, OST, PST).


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Информация о документе. |
|

**Returns:**
com.groupdocs.search.scaling.results.NetworkDocumentInfo[] - массив элементов документа.

### getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.scaling.results.NetworkDocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public abstract void getDocumentText(NetworkDocumentInfo documentInfo, OutputAdapter adapter)
```


Генерирует текст проиндексированного документа и передаёт его через выходной адаптер.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [NetworkDocumentInfo](../../com.groupdocs.search.scaling.results/networkdocumentinfo) | Информация о проиндексированном документе. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Адаптер вывода. |
|

