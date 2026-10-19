---
title: "Cerca"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Cerca nell'indice."
type: docs
weight: 260
url: /it/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Cerca nell'indice.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | String | La query di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

Il seguente esempio dimostra come eseguire una ricerca semplice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Il seguente esempio dimostra come eseguire una ricerca Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Il seguente esempio dimostra come eseguire una ricerca a faccette.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Cerca nell'indice.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | String | La query di ricerca. |
| opzioni | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

Il seguente esempio dimostra come eseguire una ricerca fuzzy.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Le virgolette doppie all'inizio e alla fine indicano all'indice che si tratta di una query di ricerca a frase
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Il seguente esempio dimostra come eseguire una ricerca di sinonimi.

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

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Cerca nell'indice.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La query di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

Il seguente esempio dimostra come eseguire una ricerca utilizzando una query in forma di oggetto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creazione della sottoquery 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Creazione della sottoquery 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Creazione della sottoquery 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combinazione di sottoquery in una singola query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Cerca nell'indice.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La query di ricerca. |
| opzioni | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

Il seguente esempio dimostra come eseguire una ricerca utilizzando una query in forma di oggetto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Creazione di sottoquery di ricerca per intervallo di date
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creazione di sottoquery di carattere jolly con numero di parole mancanti da 0 a 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creazione di sottoquery di parola semplice
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinazione di sottoquery in una singola query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creazione di oggetto opzioni di ricerca con capacità aumentata delle occorrenze trovate
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Vedi anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Esegue una ricerca inversa di immagini nell'indice.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| immagine | SearchImage | L'immagine da cercare. |
| opzioni | ImageSearchOptions | Le opzioni di ricerca dell'immagine. |

### Valore di ritorno

Il risultato di una ricerca inversa di immagini.

### Vedi anche

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
