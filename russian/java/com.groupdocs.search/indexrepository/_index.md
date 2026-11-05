---
title: "IndexRepository"
second_title: "GroupDocs.Search для Java API Reference"
description: "Представляет контейнер для объединения нескольких индексов и выполнения общих операций над ними."
type: docs
weight: 18
url: /ru/java/com.groupdocs.search/indexrepository/
---
**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.io.Closeable
```
public class IndexRepository implements Closeable
```

Представляет контейнер для объединения нескольких индексов и выполнения общих операций над ними.


**Learn more**

* [Search index repository](../https://docs.groupdocs.com/display/searchjava/Search+index+repository)


Пример демонстрирует типичное использование класса.

````
 ```

String indexFolder1 = "c:\\MyIndex\\";
String indexFolder2 = "c:\\MyIndex\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
repository.addToRepository(indexFolder1); // Загрузка существующего индекса
repository.addToRepository(indexFolder2); // Загрузка другого существующего индекса
SearchResult result = repository.search(query); // Поиск в индексах репозитория
 
```
 
````


## Конструкторы

| Конструктор | Описание |
| --- | --- |
|  | [IndexRepository()](#IndexRepository--) | Инициализирует новый экземпляр |
IndexRepository
класс.
|
## Методы

| Метод | Описание |
| --- | --- |
|  | [getEvents()](#getEvents--) | Получает центр событий для подписки на события. |
|
|  | [getIndexes()](#getIndexes--) | Получает индексы, содержащиеся в этом |
IndexRepository
.
|
|  | [close()](#close--) | Освобождает все ресурсы, используемые |
IndexRepository
.
|
|  | [create()](#create--) | Создает новый индекс в памяти. |
|
|  | [create(IndexSettings settings)](#create-com.groupdocs.search.IndexSettings-) | Создает новый индекс в памяти. |
|
|  | [create(String indexFolder)](#create-java.lang.String-) | Создает новый индекс на диске. |
|
|  | [create(String indexFolder, IndexSettings settings)](#create-java.lang.String-com.groupdocs.search.IndexSettings-) | Создает новый индекс на диске. |
|
|  | [addToRepository(Index index)](#addToRepository-com.groupdocs.search.Index-) | Добавляет индекс в репозиторий индексов. |
|
|  | [addToRepository(String indexFolder)](#addToRepository-java.lang.String-) | Открывает и добавляет индекс в репозиторий индексов. |
|
|  | [update()](#update--) | Обновляет все индексы в репозитории. |
|
|  | [update(UpdateOptions options)](#update-com.groupdocs.search.options.UpdateOptions-) | Обновляет все индексы в репозитории. |
|
|  | [search(String query)](#search-java.lang.String-) | Ищет во всех индексах репозитория. |
|
|  | [search(String query, SearchOptions options)](#search-java.lang.String-com.groupdocs.search.options.SearchOptions-) | Ищет во всех индексах репозитория. |
|
|  | [search(SearchQuery query)](#search-com.groupdocs.search.SearchQuery-) | Ищет во всех индексах репозитория. |
|
|  | [search(SearchQuery query, SearchOptions options)](#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-) | Ищет во всех индексах репозитория. |
|
### IndexRepository() {#IndexRepository--}
```
public IndexRepository()
```


Инициализирует новый экземпляр
IndexRepository
класс.


### getEvents() {#getEvents--}
```
public final EventHub getEvents()
```


Получает центр событий для подписки на события.


**Returns:**
[EventHub](../../com.groupdocs.search.events/eventhub) - The event hub for subscribing to events.

### getIndexes() {#getIndexes--}
```
public final Index[] getIndexes()
```


Получает индексы, содержащиеся в этом
IndexRepository
.


**Returns:**
com.groupdocs.search.Index[] - Индексы.

### close() {#close--}
```
public final void close()
```


Освобождает все ресурсы, используемые
IndexRepository
.


### create() {#create--}
```
public final Index create()
```


Создает новый индекс в памяти.


**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

Пример демонстрирует, как создать индекс в памяти через репозиторий индексов.

````
 ```

IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create();
 
```
 
````


### create(IndexSettings settings) {#create-com.groupdocs.search.IndexSettings-}
```
public final Index create(IndexSettings settings)
```


Создает новый индекс в памяти.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Настройки индекса. |

Пример демонстрирует, как создать индекс в памяти через репозиторий индексов.

````
 ```

IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Отключение использования стоп-слов при индексации
Index index = indexRepository.create(settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder) {#create-java.lang.String-}
```
public final Index create(String indexFolder)
```


Создает новый индекс на диске.
Папка индекса будет очищена перед созданием индекса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Папка индекса. |

Пример демонстрирует, как создать индекс на диске через репозиторий индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
Index index = indexRepository.create(indexFolder);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### create(String indexFolder, IndexSettings settings) {#create-java.lang.String-com.groupdocs.search.IndexSettings-}
```
public final Index create(String indexFolder, IndexSettings settings)
```


Создает новый индекс на диске.
Папка индекса будет очищена перед созданием индекса.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Папка индекса. |
|
|  | settings | [IndexSettings](../../com.groupdocs.search/indexsettings) | Настройки индекса. |

Пример демонстрирует, как создать индекс на диске через репозиторий индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
IndexSettings settings = new IndexSettings();
settings.setUseStopWords(false); // Отключение использования стоп-слов при индексации
Index index = indexRepository.create(indexFolder, settings);
 
```
 
````

|

**Returns:**
[Index](../../com.groupdocs.search/index) - The created index.

### addToRepository(Index index) {#addToRepository-com.groupdocs.search.Index-}
```
public final void addToRepository(Index index)
```


Добавляет индекс в репозиторий индексов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | index | [Index](../../com.groupdocs.search/index) | Индекс для добавления. |

Пример демонстрирует, как добавить индекс в репозиторий индексов.

````
 ```

Index index = new Index();
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(index);
 
```
 
````

|

### addToRepository(String indexFolder) {#addToRepository-java.lang.String-}
```
public final void addToRepository(String indexFolder)
```


Открывает и добавляет индекс в репозиторий индексов.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | indexFolder | java.lang.String | Папка индекса. |

Пример демонстрирует, как добавить индекс в репозиторий индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
IndexRepository indexRepository = new IndexRepository();
indexRepository.addToRepository(indexFolder);
 
```
 
````

|

### update() {#update--}
```
public final void update()
```


Обновляет все индексы в репозитории.

Пример демонстрирует, как обновлять индексы в репозитории.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Создание индекса
index.add(documentsFolder); // Индексация документов
// Удалите документы из папки документов или измените их, или добавьте новые документы в папку
repository.update();
 
```
 
````



### update(UpdateOptions options) {#update-com.groupdocs.search.options.UpdateOptions-}
```
public final void update(UpdateOptions options)
```


Обновляет все индексы в репозитории.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | options | [UpdateOptions](../../com.groupdocs.search.options/updateoptions) | Параметры обновления. |

Пример демонстрирует, как обновлять индексы в репозитории.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Создание индекса
index.add(documentsFolder); // Индексация документов
// Удалите документы из папки документов или измените их, или добавьте новые документы в папку
UpdateOptions options = new UpdateOptions();
options.setThreads(2); // Установка количества потоков индексации
repository.update(options);
 
```
 
````

|

### search(String query) {#search-java.lang.String-}
```
public final SearchResult search(String query)
```


Ищет во всех индексах репозитория.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | java.lang.String | Запрос поиска. |

Пример демонстрирует, как выполнять поиск в репозитории индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Создание индекса
index.add(documentsFolder); // Индексация документов
SearchResult result = repository.search(query); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(String query, SearchOptions options) {#search-java.lang.String-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(String query, SearchOptions options)
```


Ищет во всех индексах репозитория.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | java.lang.String | Запрос поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |

Пример демонстрирует, как выполнять поиск в репозитории индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
String query = "Einstein";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Создание индекса
index.add(documentsFolder); // Индексация документов
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Установка флага поиска с учётом регистра
SearchResult result = repository.search(query, options); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query) {#search-com.groupdocs.search.SearchQuery-}
```
public final SearchResult search(SearchQuery query)
```


Ищет во всех индексах репозитория.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос поиска. |

Пример демонстрирует, как выполнять поиск в репозитории индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Создание индекса
index.add(documentsFolder); // Индексация документов
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Создание поискового запроса в виде объекта
SearchResult result = repository.search(query); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

### search(SearchQuery query, SearchOptions options) {#search-com.groupdocs.search.SearchQuery-com.groupdocs.search.options.SearchOptions-}
```
public final SearchResult search(SearchQuery query, SearchOptions options)
```


Ищет во всех индексах репозитория.


**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
|  | query | [SearchQuery](../../com.groupdocs.search/searchquery) | Запрос поиска. |
|
|  | options | [SearchOptions](../../com.groupdocs.search.options/searchoptions) | Параметры поиска. |

Пример демонстрирует, как выполнять поиск в репозитории индексов.

````
 ```

String indexFolder = "c:\\MyIndex\\";
String documentsFolder = "c:\\MyDocuments\\";
IndexRepository repository = new IndexRepository();
Index index = repository.create(indexFolder); // Создание индекса
index.add(documentsFolder); // Индексация документов
SearchOptions options = new SearchOptions();
options.setUseCaseSensitiveSearch(true); // Установка флага поиска с учётом регистра
SearchQuery query = SearchQuery.createWordQuery("Einstein"); // Создание поискового запроса в виде объекта
SearchResult result = repository.search(query, options); // Поиск
 
```
 
````

|

**Returns:**
[SearchResult](../../com.groupdocs.search.results/searchresult) - The search result.

