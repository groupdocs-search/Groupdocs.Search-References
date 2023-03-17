---
title: Index
second_title: GroupDocs.Search для справочника API .NET
description: Представляет основной класс для индексации документов и поиска по ним.
type: docs
weight: 680
url: /ru/net/groupdocs.search/index/
---
## Index class

Представляет основной класс для индексации документов и поиска по ним.

```csharp
public class Index : IDisposable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Index](index#constructor)() | Инициализирует новый экземпляр[`Index`](../index) класс в памяти. |
| [Index](index#constructor_1)(IndexSettings) | Инициализирует новый экземпляр[`Index`](../index) класс в памяти с определенными настройками индекса. |
| [Index](index#constructor_2)(string) | Инициализирует новый экземпляр[`Index`](../index) class. Создает новый или открывает существующий индекс на диске. |
| [Index](index#constructor_3)(string, bool) | Инициализирует новый экземпляр[`Index`](../index) class. Загружает существующий индекс с диска, если*overwriteIfExists* является`ЛОЖЬ`; в противном случае создает новый индекс на диске. |
| [Index](index#constructor_4)(string, IndexSettings) | Инициализирует новый экземпляр[`Index`](../index) class. Создает новый индекс с определенными настройками или открывает существующий индекс на диске. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Инициализирует новый экземпляр[`Index`](../index) class. Загружает существующий индекс с диска, если*overwriteIfExists* является`ЛОЖЬ` ; в противном случае создает новый индекс на диске с определенными настройками индекса. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Получает хранилище словарей. |
| [Events](../../groupdocs.search/index/events) { get; } | Получает концентратор событий для подписки на события. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Получает основную информацию об индексе. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Получает настройки индекса. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Получает объект репозитория индексов, если индекс содержится в нем. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Выполняет операцию индексирования. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Выполняет операцию индексирования. Добавляет документы из файловой системы, потока или структуры. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Выполняет операцию индексирования. Добавляет извлеченные данные в индекс. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Выполняет операцию индексирования. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Применяет указанный пакет изменений атрибутов к проиндексированным документам без переиндексации во время операции обновления. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Удаляет проиндексированные файлы или папки из индекса. Затем обновляет индекс без удаленных путей. Обратите внимание, что отдельный документ не может быть удален из индекса, если он был добавлен в индекс как часть папки. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Удаляет проиндексированные документы из потоков или структур. Затем обновляет индекс без удаленных документов. |
| [Dispose](../../groupdocs.search/index/dispose)() | Освобождает все ресурсы, используемые[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Получает все атрибуты, связанные с указанным индексированным документом. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Генерирует текст в формате HTML для проиндексированного документа и передает его через выходной адаптер. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Генерирует текст в формате HTML для проиндексированного документа и передает его через выходной адаптер. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Получает массив вложенных элементов указанного документа (для документов-контейнеров, таких как ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Получает массив всех проиндексированных документов. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Получает массив проиндексированных путей - документов или папок. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Получает отчеты об операциях индексирования. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Получает отчеты о поисковых операциях. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Генерирует текст в формате HTML с выделенными найденными терминами. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Генерирует текст в формате HTML с выделенными найденными терминами. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Объединяет указанный индекс с текущим индексом. Обратите внимание, что другой индекс не будет изменен. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Объединяет индексы из указанного репозитория индексов в текущий индекс. Обратите внимание, что индексы в репозитории не будут изменены. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Передает указанный объект уведомления в индекс для выполнения уведомления. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Минимизирует количество сегментов индекса, объединяя их друг с другом. Эта операция повышает производительность поиска. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Минимизирует количество сегментов индекса, объединяя их друг с другом. Эта операция повышает производительность поиска. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Поиск в индексе. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Поиск в индексе. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Выполняет обратный поиск изображения в индексе. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Поиск в индексе. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Поиск в индексе. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Продолжает поиск фрагмента, начатый методом Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Продолжает поиск фрагмента, начатый методом Search. |
| [Update](../../groupdocs.search/index/update#update)() | Переиндексирует документы, которые были изменены или удалены с момента последнего обновления. Добавляет новые файлы, добавленные в проиндексированные папки. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Переиндексирует документы, которые были изменены или удалены с момента последнего обновления. Добавляет новые файлы, добавленные в проиндексированные папки. |

### Примечания

**Узнать больше**

* [Создание индекса](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Индексация](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Идет поиск](https://docs.groupdocs.com/display/searchnet/Searching)

### Примеры

Пример демонстрирует типичное использование класса.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

SearchResult result = index.Search(query); // Поиск по индексу
```

### Смотрите также

* пространство имен [GroupDocs.Search](../../groupdocs.search)
* сборка [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
