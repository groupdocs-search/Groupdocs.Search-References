---
title: "Index"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет основной класс для индексации документов и поиска по ним."
type: docs
weight: 17
url: /ru/java/com.groupdocs.search/index/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class Index implements Closeable
```

Представляет основной класс для индексации документов и поиска по ним.


**Learn more**

* [Creating an index](../https://docs.groupdocs.com/display/searchjava/Creating+an+index)
* [Indexing](../https://docs.groupdocs.com/display/searchjava/Indexing)
* [Searching](../https://docs.groupdocs.com/display/searchjava/Searching)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchResult result = index.search(query); // Поиск в индексе
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [Index()](#Index--) | Инициализирует новый экземпляр класса  Index  в памяти. |
|
|  | [Index(IndexSettings settings)](#Index-com.groupdocs.search.IndexSettings-) | Инициализирует новый экземпляр класса  Index  в памяти с конкретными настройками индекса. |
|
|  | [Index(String indexFolder)](#Index-java.lang.String-) | Инициализирует новый экземпляр класса  Index  . |
|
|  | [Index(String indexFolder, IndexSettings settings)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-) | Инициализирует новый экземпляр |
Index
класс.
|
|  | [Index(String indexFolder, boolean overwriteIfExists)](#Index-java.lang.String-boolean-) | Инициализирует новый экземпляр |
Index
класс.
|
|  | [Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)](#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-) | Инициализирует новый экземпляр |
Index
класс.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEvents()](#getEvents--) | Получает центр событий для подписки на события. |
|
|  | [getIndexInfo()](#getIndexInfo--) | Получает базовую информацию об индексе. |
|
|  | [getRepository()](#getRepository--) | Получает объект репозитория индекса, если индекс содержится в нём. |
|
|  | [getIndexSettings()](#getIndexSettings--) | Получает настройки индекса. |
|
|  | [getDictionaries()](#getDictionaries--) | Получает репозиторий словаря. |
|
|  | [close()](#close--) | Освобождает все ресурсы, используемые |
Index
.
|
|  | [add(String path)](#add-java.lang.String-) | Выполняет операцию индексации. |
|
|  | [add(String path, IndexingOptions options)](#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-) | Выполняет операцию индексации. |
|
|  | [add(String[] paths)](#add-java.lang.String---) | Выполняет операцию индексации. |
|
|  | [add(String[] paths, IndexingOptions options)](#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-) | Выполняет операцию индексации. |
|
|  | [add(Document[] documents, IndexingOptions options)](#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-) | Выполняет операцию индексации. |
|
|  | [add(ExtractedData[] data, IndexingOptions options)](#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-) | Выполняет операцию индексации. |
|
|  | [update()](#update--) | Переиндексирует документы, которые были изменены или удалены с момента последнего обновления. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Переиндексирует документы, которые были изменены или удалены с момента последнего обновления. |
|
|  | [getIndexingReports()](#getIndexingReports--) | Получает отчёты о операциях индексации. |
|
|  | [getSearchReports()](#getSearchReports--) | Получает отчёты о поисковых операциях. |
|
|  | [search(String query)](#search-java.lang.String-) | Выполняет поиск в индексе. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Выполняет поиск в индексе. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Выполняет поиск в индексе. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Выполняет поиск в индексе. |
|
|  | [search(SearchImage image, ImageSearchOptions options)](#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-) | Выполняет обратный поиск изображений в индексе. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-) | Продолжает поиск фрагментов, начатый методом Search. |
|
|  | [searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)](#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-) | Продолжает поиск фрагментов, начатый методом Search. |
|
|  | [optimize()](#optimize--) | Минимизирует количество сегментов индекса, объединяя их друг с другом. |
|
|  | [optimize(MergeOptions options)](#optimize-com.groupdocs.search.options.MergeOptions-) | Минимизирует количество сегментов индекса, объединяя их друг с другом. |
|
|  | [merge(Index index, MergeOptions options)](#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-) | Объединяет указанный индекс с текущим индексом. |
|
|  | [merge(IndexRepository repository, MergeOptions options)](#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-) | Объединяет индексы из указанного репозитория индексов с текущим индексом. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-) | Генерирует текст в формате HTML с выделенными найденными терминами. |
|
|  | [highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)](#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-) | Генерирует текст в формате HTML с выделенными найденными терминами. |
|
|  | [getIndexedDocuments()](#getIndexedDocuments--) | Получает массив всех проиндексированных документов. |
|
|  | [getIndexedDocumentItems(DocumentInfo documentInfo)](#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-) | Получает массив элементов документа. |
|
|  | [GetIndexedDocument(String documentKey)](#GetIndexedDocument-java.lang.String-) | Получает проиндексированный документ по ключу документа. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-) | Генерирует текст проиндексированного документа и передаёт его через выходной адаптер. |
|
|  | [getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)](#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-) | Генерирует текст в формате HTML для проиндексированного документа и передаёт его через выходной адаптер. |
|
|  | [getIndexedPaths()](#getIndexedPaths--) | Получает массив проиндексированных путей — документов или папок. |
|
|  | [delete(String[] paths, UpdateOptions options)](#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-) | Удаляет проиндексированные файлы или папки из индекса. |
|
|  | [delete(UpdateOptions options, String[] documentKeys)](#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---) | Удаляет документы, проиндексированные из потоков или структур. |
|
|  | [notifyIndex(Notification notification)](#notifyIndex-com.groupdocs.search.Notification-) | Передаёт указанный объект уведомления индексу для выполнения уведомления. |
|
|  | [changeAttributes(AttributeChangeBatch batch)](#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-) | Применяет указанную партию изменений атрибутов к проиндексированным документам без переиндексации во время операции обновления. |
|
|  | [getAttributes(String path)](#getAttributes-java.lang.String-) | Получает все атрибуты, связанные с указанным проиндексированным документом. |
|
|  | [loadIntoMemoryCompletely(String indexFolder)](#loadIntoMemoryCompletely-java.lang.String-) | Загружает весь индекс в память. |
|
|  | [loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)](#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-) | Загружает весь индекс в память. |
|
### Index() {#Index--}
```
public Index()
```


Инициализирует новый экземпляр класса  Index  в памяти.


Пример демонстрирует, как создать индекс в памяти без сохранения файлов на диск.

````
 ```

Index index = new Index();
 
```
 
````



### Index(IndexSettings settings) {#Index-com.groupdocs.search.IndexSettings-}
```
public Index(IndexSettings settings)
```


Инициализирует новый экземпляр класса  Index  в памяти с конкретными настройками индекса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Объект настроек индекса. |


Пример демонстрирует, как создать индекс в памяти без сохранения файлов на диск с определёнными настройками индекса.

````
 ```

IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(settings);
 
```
 
````

|

### Index(String indexFolder) {#Index-java.lang.String-}
```
public Index(String indexFolder)
```


Инициализирует новый экземпляр класса  Index . Создает новый или открывает существующий индекс на диске.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Путь к папке индекса. |


Пример демонстрирует, как создать индекс на диске или открыть существующий индекс.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public Index(String indexFolder, IndexSettings settings)
```


Инициализирует новый экземпляр
Index
класс.
Создает новый индекс с определенными настройками или открывает существующий индекс на диске.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Путь к папке индекса. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Объект настроек индекса. |

Пример демонстрирует, как создать индекс на диске с определенными настройками индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings);
 
```
 
````

|

### Index(String indexFolder, boolean overwriteIfExists) {#Index-java.lang.String-boolean-}
```
public Index(String indexFolder, boolean overwriteIfExists)
```


Инициализирует новый экземпляр
Index
класс.
Загружает существующий индекс с диска, если
overwriteIfExists
равно
false
;
в противном случае создает новый индекс на диске.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Путь к папке индекса. |
|
|  | overwriteIfExists | boolean | Флаг перезаписи папки индекса. |

Пример демонстрирует, как создать новый индекс в папке, которая уже содержит другой индекс.

````
 ```

String indexFolder = "c:\\MyIndex\\";
Index index = new Index(indexFolder, true);
 
```
 
````

|

### Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists) {#Index-java.lang.String-com.groupdocs.search.IndexSettings-boolean-}
```
public Index(String indexFolder, IndexSettings settings, boolean overwriteIfExists)
```


Инициализирует новый экземпляр
Index
класс.
Загружает существующий индекс с диска, если
overwriteIfExists
равно
false
;
в противном случае создает новый индекс на диске с определенными настройками индекса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Путь к папке индекса. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Объект настроек индекса. |
|
|  | overwriteIfExists | boolean | Флаг перезаписи папки индекса. |

Пример демонстрирует, как создать индекс на диске с определенными настройками индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexSettings settings = new IndexSettings();
settings.setIndexType(IndexType.CompactIndex);
Index index = new Index(indexFolder, settings, true);
 
```
 
````

|

### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Получает центр событий для подписки на события.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexInfo() {#getIndexInfo--}
```
public final IndexInfo getIndexInfo()
```


Получает базовую информацию об индексе.


**Returns:**
[IndexInfo](../../com.groupdocs.search.common/indexinfo) - The basic information on the index.

### getRepository() {#getRepository--}
```
public final IndexRepository getRepository()
```


Получает объект репозитория индекса, если индекс содержится в нём.


**Returns:**
[IndexRepository](../../com.groupdocs.search/indexrepository) - The index repository object.

### getIndexSettings() {#getIndexSettings--}
```
public final IndexSettings getIndexSettings()
```


Получает настройки индекса.


**Returns:**
[IndexSettings](../../com.groupdocs.search/indexsettings) - The index settings.

### getDictionaries() {#getDictionaries--}
```
public final DictionaryRepository getDictionaries()
```


Получает репозиторий словаря.


**Returns:**
[DictionaryRepository](../../com.groupdocs.search.dictionaries/dictionaryrepository) - The dictionary repository.

### close() {#close--}
```
public final void close()
```


Освобождает все ресурсы, используемые
Index
.


### add(String path) {#add-java.lang.String-}
```
public final void add(String path)
```


Выполняет операцию индексации.
Добавляет файл или папку по абсолютному или относительному пути.
Документы из всех подпапок будут проиндексированы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | путь | java.lang.String | Путь к файлу или папке, которые будут проиндексированы. |

Пример демонстрирует, как добавить документы в индекс.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(folderPath); // Индексация документов в указанной папке
index.add(filePath); // Индексация указанного документа
 
```
 
````

|

### add(String path, IndexingOptions options) {#add-java.lang.String-com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String path, IndexingOptions options)
```


Выполняет операцию индексации.
Добавляет файл или папку по абсолютному или относительному пути.
Документы из всех подпапок будут проиндексированы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | путь | java.lang.String | Путь к файлу или папке, которые будут проиндексированы. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры индексации. |

Пример демонстрирует, как добавить документы в индекс с определёнными параметрами индексации.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Установка количества потоков индексации
index.add(folderPath, options); // Индексация документов в указанной папке
index.add(filePath, options); // Индексация указанного документа
 
```
 
````

|

### add(String[] paths) {#add-java.lang.String---}
```
public final void add(String[] paths)
```


Выполняет операцию индексации.
Добавляет файлы или папки по абсолютному или относительному пути.
Документы из всех подпапок будут проиндексированы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пути | java.lang.String[] | Пути к файлам или папкам, которые необходимо проиндексировать. |

Пример демонстрирует, как добавить документы в индекс.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
String[] paths = new String[] { folderPath, filePath };
index.add(paths); // Индексация документов по указанным путям
 
```
 
````

|

### add(String[] paths, IndexingOptions options) {#add-java.lang.String---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(String[] paths, IndexingOptions options)
```


Выполняет операцию индексации.
Добавляет файлы или папки по абсолютному или относительному пути.
Документы из всех подпапок будут проиндексированы.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пути | java.lang.String[] | Пути к файлам или папкам, которые необходимо проиндексировать. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры индексации. |

Пример демонстрирует, как добавить документы в индекс с определёнными параметрами индексации.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String folderPath = "c:\\MyDocuments\\";
String filePath = "c:\\Documents\\MyFile.txt";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
IndexingOptions options = new IndexingOptions();
options.setThreads(2); // Установка количества потоков индексации
String[] paths = new String[] { folderPath, filePath };
index.add(paths, options); // Индексация документов по указанным путям
 
```
 
````

|

### add(Document[] documents, IndexingOptions options) {#add-com.groupdocs.search.Document---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(Document[] documents, IndexingOptions options)
```


Выполняет операцию индексации.
Добавляет документы из файловой системы, потока или структуры.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documents | [Document\[\]](../../com.groupdocs.search/document) | Документы из файловой системы, потока или структуры. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры индексации. |
|

### add(ExtractedData[] data, IndexingOptions options) {#add-com.groupdocs.search.ExtractedData---com.groupdocs.search.options.IndexingOptions-}
```
public final void add(ExtractedData[] data, IndexingOptions options)
```


Выполняет операцию индексации.
Добавляет извлечённые данные в индекс.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | data | [ExtractedData\[\]](../../com.groupdocs.search/extracteddata) | Извлечённые данные. |
|
|  | options | [IndexingOptions](../../com.groupdocs.search.options/indexingoptions) | Параметры индексации. |
|

### update() {#update--}
```
public final void update()
```


Переиндексирует документы, которые были изменены или удалены с момента последнего обновления.
Добавляет новые файлы, которые были добавлены в проиндексированные папки.

Пример демонстрирует, как обновить индекс.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
// Удалите документы из папки документов или измените их, или добавьте новые документы в папку
index.update(); // Обновление индекса
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Переиндексирует документы, которые были изменены или удалены с момента последнего обновления.
Добавляет новые файлы, которые были добавлены в проиндексированные папки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Параметры обновления. |

Пример демонстрирует, как обновить индекс с определёнными параметрами обновления.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
// Удалите документы из папки документов или измените их, или добавьте новые документы в папку
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Установка количества потоков индексации
index.update(options); // Обновление индекса
 
```
 
````

|

### getIndexingReports() {#getIndexingReports--}
```
public final IndexingReport[] getIndexingReports()
```


Получает отчёты о операциях индексации.


**Returns:**
com.groupdocs.search.common.IndexingReport[] - Отчёты об индексации.

Пример демонстрирует, как получить отчёты об индексации.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
IndexingReport[] reports = index.getIndexingReports(); // Получение отчётов об индексации
 
```
 
````


### getSearchReports() {#getSearchReports--}
```
public final SearchReport[] getSearchReports()
```


Получает отчёты о поисковых операциях.


**Returns:**
com.groupdocs.search.common.SearchReport[] - Отчёты поиска.

Пример демонстрирует, как получить отчёты поиска.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query1 = "Einstein";
String query2 = "Newton";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchResult result1 = index.search(query1); // Поиск
SearchResult result2 = index.search(query2);
SearchResult result3 = index.search(query1 + " & " + query2);
SearchReport[] reports = index.getSearchReports(); // Получение отчётов поиска
 
```
 
````


### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Выполняет поиск в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | java.lang.String | Запрос поиска. |

Следующий пример демонстрирует, как выполнить простой поиск.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchResult result = index.search(query); // Поиск
 
```
 
````

Следующий пример демонстрирует, как выполнить поиск Regex.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
String query = "^[0-9]{3,}"; // Символ каретки в начале поискового запроса сообщает индексу, что это запрос Regex
SearchResult result = index.search(query); // Поиск
 
```
 
````

Следующий пример демонстрирует, как выполнить фасетный поиск.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
String query = "content:Newton"; // Слово перед двоеточием в запросе обозначает имя поля документа для поиска
SearchResult result = index.search(query); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Выполняет поиск в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | java.lang.String | Запрос поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |

Следующий пример демонстрирует, как выполнить нечёткий поиск.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.getFuzzySearch().setEnabled(true); // Включение нечёткого поиска
options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1)); // Установка количества возможных различий для каждого слова
// Кавычки в начале и в конце указывают индексу, что это запрос поиска фразы
String query = "\"The Pursuit of Happiness\"";
SearchResult result = index.search(query, options); // Поиск
 
```
 
````

Следующий пример демонстрирует, как выполнить поиск синонимов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.setUseSynonymSearch(true); // Включение поиска синонимов
String query = "cry";
SearchResult result = index.search(query, options); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Выполняет поиск в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос поиска. |

Следующий пример демонстрирует, как выполнить поиск, используя запрос в виде объекта.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
// Создание подзапроса 1
SearchQuery subquery1 = SearchQuery.createWordQuery("accommodation");
subquery1.setSearchOptions(new SearchOptions()); // Установка параметров поиска только для подзапроса 1
subquery1.getSearchOptions().getFuzzySearch().setEnabled(true); // Включение нечеткого поиска
subquery1.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3)); // Установка максимального количества различий
// Создание подзапроса 2
SearchQuery subquery2 = SearchQuery.createNumericRangeQuery(1, 1000000);
// Создание подзапроса 3
SearchQuery subquery3 = SearchQuery.createRegexQuery("(.)\\1");
// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
SearchResult result = index.search(query); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Выполняет поиск в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |

Следующий пример демонстрирует, как выполнить поиск, используя запрос в виде объекта.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
// Создание подзапроса поиска по диапазону дат
SearchQuery subquery1 = SearchQuery.createDateRangeQuery(new Date(2011, 6, 17), new Date(2013, 1, 1));
// Создание подзапроса с подстановкой, количество пропущенных слов от 0 до 2
SearchQuery subquery2 = SearchQuery.createWildcardQuery(0, 2);
// Создание подзапроса простого слова
SearchQuery subquery3 = SearchQuery.createWordQuery("birth");
subquery3.setSearchOptions(new SearchOptions()); // Установка параметров поиска только для подзапроса 3
subquery3.getSearchOptions().getFuzzySearch().setEnabled(true);
subquery3.getSearchOptions().getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(1));
// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.createPhraseSearchQuery(subquery1, subquery2, subquery3);
// Создание объекта параметров поиска с увеличенной ёмкостью найденных вхождений
SearchOptions options = new SearchOptions(); // Общие параметры поиска
options.setMaxOccurrenceCountPerTerm(1000000);
options.setMaxTotalOccurrenceCount(10000000);
SearchResult result = index.search(query, options); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchImage image, ImageSearchOptions options) {#search-com.groupdocs.search.common.SearchImage-com.groupdocs.search.options.ImageSearchOptions-}
```
public final ImageSearchResult search(SearchImage image, ImageSearchOptions options)
```


Выполняет обратный поиск изображений в индексе.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | image | [SearchImage](../../com.groupdocs.search.common/searchimage) | Изображение для поиска. |
|
|  | options | [ImageSearchOptions](../../com.groupdocs.search.options/imagesearchoptions) | Параметры поиска изображения. |
|

**Returns:**
[ImageSearchResult](../../com.groupdocs.search.results/imagesearchresult) - The result of a reverse image search.

### searchNext(ChunkSearchToken chunkSearchToken) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken)
```


Продолжает поиск фрагментов, начатый методом Search.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Токен поиска фрагмента. |

Пример демонстрирует, как выполнить поиск фрагментов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Включение поиска фрагментов
SearchResult result = index.search(query, options); // Запуск поиска фрагментов
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken()); // Продолжение поиска фрагментов
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation) {#searchNext-com.groupdocs.search.common.ChunkSearchToken-com.groupdocs.search.common.Cancellation-}
```
public final SearchResult searchNext(ChunkSearchToken chunkSearchToken, Cancellation cancellation)
```


Продолжает поиск фрагментов, начатый методом Search.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | chunkSearchToken | [ChunkSearchToken](../../com.groupdocs.search.common/chunksearchtoken) | Токен поиска фрагмента. |
|
|  | cancellation | [Cancellation](../../com.groupdocs.search.common/cancellation) | Объект отмены. |

Пример демонстрирует, как выполнить поиск, используя запрос в виде объекта.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder); // Индексация документов из указанной папки
Cancellation cancellation = new Cancellation(); // Этот объект отмены прерывает все продолжения поиска при отмене
SearchOptions options = new SearchOptions();
options.setChunkSearch(true); // Включение поиска фрагментов
options.setCancellation(cancellation);
SearchResult result = index.search(query, options); // Запуск поиска фрагментов
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
while (result.getNextChunkSearchToken() != null) {
result = index.searchNext(result.getNextChunkSearchToken(), cancellation); // Продолжение поиска фрагментов
System.out.println("Document count: " + result.getDocumentCount());
System.out.println("Occurrence count: " + result.getOccurrenceCount());
}
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### optimize() {#optimize--}
```
public final void optimize()
```


Минимизирует количество сегментов индекса, объединяя их друг с другом.
Эта операция повышает производительность поиска.

Пример демонстрирует, как объединять сегменты индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder1); // Индексация документов из указанной папки
index.add(documentsFolder2); // Каждый вызов AddToIndex создает как минимум один новый сегмент в индексе
index.add(documentsFolder3);
// Слияние сегментов индекса
index.optimize();
 
```
 
````



### optimize(MergeOptions options) {#optimize-com.groupdocs.search.options.MergeOptions-}
```
public final void optimize(MergeOptions options)
```


Минимизирует количество сегментов индекса, объединяя их друг с другом.
Эта операция повышает производительность поиска.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Параметры слияния. |

Пример демонстрирует, как объединять сегменты индекса с определёнными параметрами слияния.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.add(documentsFolder1); // Индексация документов из указанной папки
index.add(documentsFolder2); // Каждый вызов AddToIndex создает как минимум один новый сегмент в индексе
index.add(documentsFolder3);
MergeOptions options = new MergeOptions();
options.setAsync(true); // Асинхронная операция
options.setCancellation(new Cancellation()); // Создание объекта отмены
// Слияние сегментов индекса
index.optimize(options); // Этот метод вернётся до завершения операции
options.getCancellation().cancelAfter(10000); // Установка максимальной продолжительности операции в 10 секунд
 
```
 
````

|

### merge(Index index, MergeOptions options) {#merge-com.groupdocs.search.Index-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(Index index, MergeOptions options)
```


Объединяет указанный индекс с текущим индексом.
Обратите внимание, что другой индекс не будет изменён.


Если у другого индекса есть предыдущая версия, её необходимо обновить перед слиянием с
IndexUpdater
.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Индекс, в который будет выполнено слияние. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Параметры слияния. |

Пример демонстрирует, как объединить индекс с текущим индексом.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
Index index1 = new Index(indexFolder1); // Создание index1
index1.add(documentsFolder1); // Индексация документов
Index index2 = new Index(indexFolder2); // Создание index2
index2.add(documentsFolder2); // Индексация документов
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Создание объекта отмены
// Слияние index2 в index1. Обратите внимание, что файлы index2 не будут изменены.
index1.merge(index2, options);
 
```
 
````

|

### merge(IndexRepository repository, MergeOptions options) {#merge-com.groupdocs.search.IndexRepository-com.groupdocs.search.options.MergeOptions-}
```
public final void merge(IndexRepository repository, MergeOptions options)
```


Объединяет индексы из указанного репозитория индексов с текущим индексом.
Обратите внимание, что индексы в репозитории не будут изменены.


Если у других индексов есть предыдущая версия, их необходимо обновить перед слиянием с
IndexUpdater
.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | repository | [IndexRepository](../../com.groupdocs.search/indexrepository) | Репозиторий индексов, в который будет выполнено слияние. |
|
|  | options | [MergeOptions](../../com.groupdocs.search.options/mergeoptions) | Параметры слияния. |

В примере демонстрируется, как объединить репозиторий индексов с текущим индексом.

````
 ```

String indexFolder1 = "c:\\MyIndex1\\";
String indexFolder2 = "c:\\MyIndex2\\";
String indexFolder3 = "c:\\MyIndex3\\";
String documentsFolder1 = "c:\\MyDocuments1\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
String documentsFolder3 = "c:\\MyDocuments3\\";
Index index1 = new Index(indexFolder1); // Создание index1
index1.add(documentsFolder1); // Индексация документов
IndexRepository repository = new IndexRepository(); // Создание репозитория индексов
Index index2 = repository.create(indexFolder2); // Создание index2
index2.add(documentsFolder2); // Индексация документов
Index index3 = repository.create(indexFolder3); // Создание index3
index3.add(documentsFolder3); // Индексация документов
MergeOptions options = new MergeOptions();
options.setCancellation(new Cancellation()); // Создание объекта отмены
// Объединение всех индексов в репозитории индексов в index1. Обратите внимание, что index2 и index3 не будут изменены.
index1.merge(repository, options);
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-}
```
public final void highlight(FoundDocument document, Highlighter highlighter)
```


Генерирует текст в формате HTML с выделенными найденными терминами.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Найденный документ. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Подсветка результатов поиска. |

В примере демонстрируется, как подсвечивать вхождения в тексте, отформатированном в HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentFolder);
// Поиск слова 'eternity'
SearchResult result = index.search("eternity");
// Подсветка вхождений в тексте
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Получение первого найденного документа
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Создание адаптера вывода в файл
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Создание объекта подсветки
index.highlight(document, highlighter); // Генерация текста в формате HTML с выделенными вхождениями
}
 
```
 
````

|

### highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options) {#highlight-com.groupdocs.search.results.FoundDocument-com.groupdocs.search.highlighters.Highlighter-com.groupdocs.search.options.HighlightOptions-}
```
public final void highlight(FoundDocument document, Highlighter highlighter, HighlightOptions options)
```


Генерирует текст в формате HTML с выделенными найденными терминами.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | document | [FoundDocument](../../com.groupdocs.search.results/founddocument) | Найденный документ. |
|
|  | highlighter | [Highlighter](../../com.groupdocs.search.highlighters/highlighter) | Подсветка результатов поиска. |
|
|  | options | [HighlightOptions](../../com.groupdocs.search.options/highlightoptions) | Параметры подсветки. |

В примере демонстрируется, как подсвечивать вхождения в тексте, отформатированном в HTML.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentFolder = "c:\\MyDocuments\\";
// Создание индекса
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentFolder);
// Поиск слова 'eternity'
SearchResult result = index.search("eternity");
// Подсветка вхождений в тексте
if (result.getDocumentCount() > 0) {
FoundDocument document = result.getFoundDocument(0); // Получение первого найденного документа
OutputAdapter outputAdapter = new FileOutputAdapter("c:\\Highlighted.html"); // Создание адаптера вывода в файл
Highlighter highlighter = new HtmlHighlighter(outputAdapter); // Создание объекта подсветки
HighlightOptions options = new HighlightOptions(); // Создание объекта параметров подсветки
options.setTermsBefore(5);
options.setTermsAfter(5);
options.setTermsTotal(15);
index.highlight(document, highlighter, options); // Генерация текста в формате HTML с выделенными вхождениями
}
 
```
 
````

|

### getIndexedDocuments() {#getIndexedDocuments--}
```
public final DocumentInfo[] getIndexedDocuments()
```


Получает массив всех проиндексированных документов.


**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Массив всех проиндексированных документов.

Пример демонстрирует, как получить список проиндексированных документов из индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Получение списка проиндексированных документов
DocumentInfo[] documents = index.getIndexedDocuments();
 
```
 
````


### getIndexedDocumentItems(DocumentInfo documentInfo) {#getIndexedDocumentItems-com.groupdocs.search.results.DocumentInfo-}
```
public final DocumentInfo[] getIndexedDocumentItems(DocumentInfo documentInfo)
```


Получает массив элементов документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Информация о документе. |

Пример демонстрирует, как получить список элементов проиндексированного документа из индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Получение списка проиндексированных документов
DocumentInfo[] documents = index.getIndexedDocuments();
for (int i = 0; i < documents.length; i++) {
DocumentInfo document = documents[i];
System.out.println(document.getFilePath());
DocumentInfo[] items = index.getIndexedDocumentItems(document); // Получение списка элементов документа
for (int j = 0; j < items.length; j++) {
DocumentInfo item = items[j];
System.out.println("\t" + item.getInnerPath());
}
}
 
```
 
````

|

**Returns:**
com.groupdocs.search.results.DocumentInfo[] - Массив элементов документа.

### GetIndexedDocument(String documentKey) {#GetIndexedDocument-java.lang.String-}
```
public DocumentInfo GetIndexedDocument(String documentKey)
```


Получает проиндексированный документ по ключу документа.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentKey | java.lang.String | Ключ документа. |
|

**Returns:**
[DocumentInfo](../../com.groupdocs.search.results/documentinfo) - The indexed document.

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```


Генерирует текст проиндексированного документа и передаёт его через выходной адаптер.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Информация о проиндексированном документе. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Адаптер вывода. |

Пример демонстрирует, как получить текст проиндексированного документа из индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов из указанной папки
index.add(documentsFolder);
// Получение списка проиндексированных документов
DocumentInfo[] documents = index.getIndexedDocuments();
// Получение текста документа
if (documents.length > 0) {
FileOutputAdapter outputAdapter = new FileOutputAdapter("C:\\Text.html");
index.getDocumentText(documents[0], outputAdapter);
}
 
```
 
````

|

### getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options) {#getDocumentText-com.groupdocs.search.results.DocumentInfo-com.groupdocs.search.common.OutputAdapter-com.groupdocs.search.options.TextOptions-}
```
public final void getDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```


Генерирует текст в формате HTML для проиндексированного документа и передаёт его через выходной адаптер.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | documentInfo | [DocumentInfo](../../com.groupdocs.search.results/documentinfo) | Информация о проиндексированном документе. |
|
|  | adapter | [OutputAdapter](../../com.groupdocs.search.common/outputadapter) | Адаптер вывода. |
|
|  | options | [TextOptions](../../com.groupdocs.search.options/textoptions) | Параметры получения текста. |
|

### getIndexedPaths() {#getIndexedPaths--}
```
public final String[] getIndexedPaths()
```


Получает массив проиндексированных путей — документов или папок.


**Returns:**
java.lang.String[] - Массив проиндексированных путей.

### delete(String[] paths, UpdateOptions options) {#delete-java.lang.String---com.groupdocs.search.options.UpdateOptions-}
```
public final DeleteResult delete(String[] paths, UpdateOptions options)
```


Удаляет проиндексированные файлы или папки из индекса. Затем обновляет индекс без удалённых путей.
Обратите внимание, что отдельный документ нельзя удалить из индекса, если он был добавлен в индекс как часть папки.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | пути | java.lang.String[] | Пути к файлам или папкам для удаления. |
|
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Параметры обновления. |

Пример демонстрирует, как удалить проиндексированные пути из индекса.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder1 = "c:\\MyDocuments\\";
String documentsFolder2 = "c:\\MyDocuments2\\";
// Создание индекса в указанной папке
Index index = new Index(indexFolder);
// Индексация документов из указанных папок
index.add(documentsFolder1);
index.add(documentsFolder2);
// Получение проиндексированных путей из индекса
String[] indexedPaths1 = index.getIndexedPaths();
// Вывод проиндексированных путей в консоль
System.out.println("Проиндексированные пути:");
for (String path : indexedPaths1) {
System.out.println("\t" + path);
}
// Удаление пути из индекса
DeleteResult deleteResult = index.delete(new String[] { documentsFolder1 }, new UpdateOptions());
// Получение проиндексированных путей после удаления
String[] indexedPaths2 = index.getIndexedPaths();
System.out.println("\nУдалённые пути: " + deleteResult.getSuccessCount());
System.out.println("\nИндексированные пути:");
for (String path : indexedPaths2) {
System.out.println("\t" + path);
}
 
```
 
````

|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting files or folders from the index.

### delete(UpdateOptions options, String[] documentKeys) {#delete-com.groupdocs.search.options.UpdateOptions-java.lang.String---}
```
public final DeleteResult delete(UpdateOptions options, String[] documentKeys)
```


Удаляет документы, проиндексированные из потоков или структур. Затем обновляет индекс без удалённых документов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Параметры обновления. |
|
|  | documentKeys | java.lang.String[] | Ключи документов, добавленных из потоков или структур. |
|

**Returns:**
[DeleteResult](../../com.groupdocs.search.results/deleteresult) - An object describing the result of deleting documents from the index.

### notifyIndex(Notification notification) {#notifyIndex-com.groupdocs.search.Notification-}
```
public final boolean notifyIndex(Notification notification)
```


Передаёт указанный объект уведомления индексу для выполнения уведомления.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | notification | [Notification](../../com.groupdocs.search/notification) | Объект уведомления. |
|

**Returns:**
boolean - Возвращает  true  если уведомление было успешно выполнено; в противном случае  false .

### changeAttributes(AttributeChangeBatch batch) {#changeAttributes-com.groupdocs.search.common.AttributeChangeBatch-}
```
public final void changeAttributes(AttributeChangeBatch batch)
```


Применяет указанную партию изменений атрибутов к проиндексированным документам без переиндексации во время операции обновления.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | batch | [AttributeChangeBatch](../../com.groupdocs.search.common/attributechangebatch) | Пакет изменений атрибутов. |
|

### getAttributes(String path) {#getAttributes-java.lang.String-}
```
public final String[] getAttributes(String path)
```


Получает все атрибуты, связанные с указанным проиндексированным документом.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | путь | java.lang.String | Путь к документу. |
|

**Returns:**
java.lang.String[] - Атрибуты, связанные с документом.

### loadIntoMemoryCompletely(String indexFolder) {#loadIntoMemoryCompletely-java.lang.String-}
```
public static Index loadIntoMemoryCompletely(String indexFolder)
```


Загружает весь индекс в память.
Любые изменения индекса не сохраняются автоматически в оригинальную папку.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Путь к папке индекса. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

### loadIntoMemoryCompletely(String indexFolder, IndexSettings settings) {#loadIntoMemoryCompletely-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public static Index loadIntoMemoryCompletely(String indexFolder, IndexSettings settings)
```


Загружает весь индекс в память.
Любые изменения индекса не сохраняются автоматически в оригинальную папку.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Путь к папке индекса. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Объект настроек индекса. |
|

**Returns:**
[Index](../../com.groupdocs.search/index) - The loaded in-memory index.

