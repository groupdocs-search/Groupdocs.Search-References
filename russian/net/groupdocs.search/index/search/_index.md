---
title: Search
second_title: GroupDocs.Search для справочника API .NET
description: Поиск в индексе.
type: docs
weight: 220
url: /ru/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Поиск в индексе.

```csharp
public SearchResult Search(string query)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| query | String | Поисковый запрос. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере показано, как выполнить простой поиск.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

SearchResult result = index.Search(query); // Идет поиск
```

В следующем примере показано, как выполнять поиск Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

string query = "^[0-9]{3,}"; // Символ вставки в начале поискового запроса сообщает индексу, что это запрос Regex
SearchResult result = index.Search(query); // Идет поиск
```

В следующем примере показано, как выполнять многогранный поиск.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

string query = "content:Newton"; // Слово перед двоеточием в запросе означает имя поля документа для поиска
SearchResult result = index.Search(query); // Идет поиск
```

### Смотрите также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Поиск в индексе.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| query | String | Поисковый запрос. |
| options | SearchOptions | Параметры поиска. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере показано, как выполнять нечеткий поиск.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Включение нечеткого поиска
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Установка количества возможных отличий для каждого слова

// Двойные кавычки в начале и в конце сообщают индексу, что это поисковый запрос по фразе
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Идет поиск
```

В следующем примере показано, как выполнять поиск синонимов.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Включение поиска синонимов

string query = "cry";
SearchResult result = index.Search(query, options); // Идет поиск
```

### Смотрите также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Поиск в индексе.

```csharp
public SearchResult Search(SearchQuery query)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| query | SearchQuery | Поисковый запрос. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере показано, как выполнять поиск с использованием запроса в форме объекта.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

// Создание подзапроса 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Установка параметров поиска только для подзапроса 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Включение нечеткого поиска
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Установка максимального количества отличий

// Создание подзапроса 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Создание подзапроса 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Идет поиск
```

### Смотрите также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Поиск в индексе.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| query | SearchQuery | Поисковый запрос. |
| options | SearchOptions | Параметры поиска. |

### Возвращаемое значение

Результат поиска.

### Примеры

В следующем примере показано, как выполнять поиск с использованием запроса в форме объекта.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Создание индекса в указанной папке
index.Add(documentsFolder); // Индексация документов из указанной папки

// Создание подзапроса поиска диапазона дат
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Создание подзапроса подстановочного знака с количеством пропущенных слов от 0 до 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Создание подзапроса простого слова
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Установка параметров поиска только для подзапроса 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Объединение подзапросов в один запрос
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Создание объекта опций поиска с увеличенной емкостью найденных вхождений
SearchOptions options = new SearchOptions(); // Общие параметры поиска
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Идет поиск
```

### Смотрите также

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Выполняет обратный поиск изображения в индексе.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| image | SearchImage | Изображение для поиска. |
| options | ImageSearchOptions | Параметры поиска изображений. |

### Возвращаемое значение

Результат обратного поиска изображения.

### Смотрите также

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* пространство имен [GroupDocs.Search](../../index)
* сборка [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
