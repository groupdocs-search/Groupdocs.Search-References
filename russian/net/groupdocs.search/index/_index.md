---
title: "Index"
second_title: "Справочник API GroupDocs.Search для .NET"
description: "Представляет основной класс для индексации документов и поиска по ним."
type: docs
weight: 700
url: /ru/net/groupdocs.search/index/
---
## Index class

Представляет основной класс для индексации документов и поиска по ним.

```csharp
public class Index : IDisposable
```

## Конструкторы

| Name | Описание |
| --- | --- |
| [Index](index#constructor)() | Инициализирует новый экземпляр класса [`Index`](../index) в памяти. |
| [Index](index#constructor_1)(IndexSettings) | Инициализирует новый экземпляр класса [`Index`](../index) в памяти с определёнными настройками индекса. |
| [Index](index#constructor_2)(string) | Инициализирует новый экземпляр класса [`Index`](../index). Создаёт новый или открывает существующий индекс на диске. |
| [Index](index#constructor_3)(string, bool) | Инициализирует новый экземпляр класса [`Index`](../index). Загружает существующий индекс с диска, если *overwriteIfExists* равно `false`; в противном случае создаёт новый индекс на диске. |
| [Index](index#constructor_4)(string, IndexSettings) | Инициализирует новый экземпляр класса [`Index`](../index). Создает новый индекс с определёнными настройками или открывает существующий индекс на диске. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Инициализирует новый экземпляр класса [`Index`](../index). Загружает существующий индекс с диска, если *overwriteIfExists* равно `false`; в противном случае создаёт новый индекс на диске с определёнными настройками индекса. |

## Properties

| Name | Описание |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Получает репозиторий словаря. |
| [Events](../../groupdocs.search/index/events) { get; } | Получает центр событий для подписки на события. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Получает базовую информацию об индексе. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Получает настройки индекса. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Получает объект репозитория индекса, если индекс содержится в нём. |

## Methods

| Name | Описание |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Загружает весь индекс в память. Любые изменения индекса не сохраняются автоматически в исходную папку. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Загружает весь индекс в память. Любые изменения индекса не сохраняются автоматически в исходную папку. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Выполняет операцию индексации. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Выполняет операцию индексации. Добавляет документы из файловой системы, потока или структуры. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Выполняет операцию индексации. Добавляет извлечённые данные в индекс. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Выполняет операцию индексации. Добавляет файл или папку по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Выполняет операцию индексации. Добавляет файлы или папки по абсолютному или относительному пути. Документы из всех подпапок будут проиндексированы. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Применяет указанную партию изменений атрибутов к проиндексированным документам без переиндексации во время операции обновления. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Проверяет индекс на наличие повреждённых файлов сегментов на диске. Метод исправляет функциональность индекса при наличии повреждённых сегментов, если *fixIndexFunctionality* равно true; иначе не исправляет. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Удаляет проиндексированные файлы или папки из индекса. Затем обновляет индекс без удалённых путей. Обратите внимание, что отдельный документ нельзя удалить из индекса, если он был добавлен в индекс как часть папки. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Удаляет документы, проиндексированные из потоков или структур. Затем обновляет индекс без удалённых документов. |
| [Dispose](../../groupdocs.search/index/dispose)() | Освобождает все ресурсы, используемые [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Получает все атрибуты, связанные с указанным проиндексированным документом. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Генерирует текст проиндексированного документа и передаёт его через адаптер вывода. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Генерирует текст в формате HTML для проиндексированного документа и передаёт его через адаптер вывода. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Получает проиндексированный документ по ключу документа. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Получает массив вложенных элементов указанного документа (для контейнерных документов, таких как ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Получает массив всех проиндексированных документов. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Получает массив проиндексированных путей — документов или папок. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Получает отчёты об операциях индексации. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Получает отчёты об операциях поиска. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Генерирует текст в формате HTML с выделенными найденными терминами. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Генерирует текст в формате HTML с выделенными найденными терминами. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Объединяет указанный индекс с текущим индексом. Обратите внимание, что другой индекс не будет изменён. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Объединяет индексы из указанного репозитория индексов с текущим индексом. Обратите внимание, что индексы в репозитории не будут изменены. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Передаёт указанный объект уведомления индексу для выполнения уведомления. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Уменьшает количество сегментов индекса, объединяя их друг с другом. Эта операция улучшает производительность поиска. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Уменьшает количество сегментов индекса, объединяя их друг с другом. Эта операция улучшает производительность поиска. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Сохраняет индекс в памяти на диск. Также сохраняет обычный индекс в другую папку. Не изменяет настройки этого индекса. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Выполняет поиск в индексе. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Выполняет поиск в индексе. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Выполняет обратный поиск изображений в индексе. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Выполняет поиск в индексе. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Выполняет поиск в индексе. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Продолжает поиск фрагментов, начатый методом Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Продолжает поиск фрагментов, начатый методом Search. |
| [Update](../../groupdocs.search/index/update#update)() | Переиндексирует документы, которые были изменены или удалены с момента последнего обновления. Добавляет новые файлы, которые были добавлены в проиндексированные папки. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Переиндексирует документы, которые были изменены или удалены с момента последнего обновления. Добавляет новые файлы, которые были добавлены в проиндексированные папки. |

### Примечания

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Примеры

Пример демонстрирует типичное использование класса.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### См. также

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
