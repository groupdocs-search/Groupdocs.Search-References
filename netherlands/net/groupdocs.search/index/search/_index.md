---
title: "Zoeken"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Zoekt in de index."
type: docs
weight: 260
url: /nl/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Zoekt in de index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| zoekopdracht | String | De zoekopdracht. |

### Retourwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld toont hoe een eenvoudige zoekopdracht uit te voeren.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Het volgende voorbeeld toont hoe een regex-zoekopdracht uit te voeren.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Het volgende voorbeeld toont hoe een gefacetteerde zoekopdracht uit te voeren.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Zoekt in de index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| zoekopdracht | String | De zoekopdracht. |
| opties | SearchOptions | De zoekopties. |

### Retourwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld toont hoe een fuzzy-zoekopdracht uit te voeren.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Dubbele aanhalingstekens aan het begin en einde geven aan de index aan dat het een frase-zoekopdracht is
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Het volgende voorbeeld toont hoe een synoniemzoekopdracht uit te voeren.

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

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Zoekt in de index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| zoekopdracht | SearchQuery | De zoekopdracht. |

### Retourwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld toont hoe een zoekopdracht uit te voeren met een query in objectvorm.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Subquery 1 maken
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Subquery 2 maken
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Subquery 3 maken
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Subqueries combineren tot één query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Zoekt in de index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| zoekopdracht | SearchQuery | De zoekopdracht. |
| opties | SearchOptions | De zoekopties. |

### Retourwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld toont hoe een zoekopdracht uit te voeren met een query in objectvorm.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Subquery maken voor datumreekszoekopdracht
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Subquery maken voor wildcard met een aantal gemiste woorden van 0 tot 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Subquery maken voor eenvoudig woord
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Subqueries combineren tot één query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Zoekopties‑object maken met verhoogde capaciteit voor gevonden voorkomen.
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Voert een omgekeerde afbeeldingzoekopdracht uit in de index.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| afbeelding | SearchImage | De afbeelding om te zoeken. |
| opties | ImageSearchOptions | De afbeeldingszoekopties. |

### Retourwaarde

Het resultaat van een omgekeerde afbeeldingszoekopdracht.

### Zie ook

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
