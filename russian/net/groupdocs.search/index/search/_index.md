---
title: "Поиск"
second_title: "Справочник API GroupDocs.Search для .NET"
description: "Выполняет поиск в индексе."
type: docs
weight: 260
url: /ru/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Выполняет поиск в индексе.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| запрос | String | Поисковый запрос. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере демонстрируется, как выполнить простой поиск.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

В следующем примере демонстрируется, как выполнить поиск с использованием регулярных выражений.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

В следующем примере демонстрируется, как выполнить фасетный поиск.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### См. также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Выполняет поиск в индексе.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| запрос | String | Поисковый запрос. |
| опции | SearchOptions | Параметры поиска. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере демонстрируется, как выполнить нечёткий поиск.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Кавычки в начале и в конце указывают индексу, что это запрос фразового поиска.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

В следующем примере демонстрируется, как выполнить поиск синонимов.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Enabling the synonym search

string query = "cry";
SearchResult result = index.Search(query, options); // Searching
```

### См. также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Выполняет поиск в индексе.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| запрос | SearchQuery | Поисковый запрос. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере демонстрируется, как выполнить поиск, используя запрос в виде объекта.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Создание подзапроса 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Создание подзапроса 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Создание подзапроса 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### См. также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Выполняет поиск в индексе.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| запрос | SearchQuery | Поисковый запрос. |
| опции | SearchOptions | Параметры поиска. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере демонстрируется, как выполнить поиск, используя запрос в виде объекта.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Создание подзапроса поиска диапазона дат
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Создание подзапроса подстановки с количеством пропущенных слов от 0 до 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Создание подзапроса простого слова
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Создание объекта параметров поиска с увеличенной емкостью найденных вхождений
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### См. также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Выполняет обратный поиск изображений в индексе.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Описание |
| --- | --- | --- |
| изображение | SearchImage | Изображение для поиска. |
| опции | ImageSearchOptions | Параметры поиска изображения. |

### Возвращаемое значение

Результат обратного поиска изображения.

### См. также

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
