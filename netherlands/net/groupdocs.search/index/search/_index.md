---
title: Search
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Zoekopdrachten in index.
type: docs
weight: 220
url: /nl/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Zoekopdrachten in index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| query | String | De zoekvraag. |

### Winstwaarde

Het zoekresultaat.

### Voorbeelden

In het volgende voorbeeld ziet u hoe u eenvoudig kunt zoeken.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

SearchResult result = index.Search(query); // Zoeken
```

Het volgende voorbeeld laat zien hoe u een Regex-zoekopdracht uitvoert.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

string query = "^[0-9]{3,}"; // Het caret-symbool aan het begin van de zoekopdracht vertelt de index dat het een Regex-query is
SearchResult result = index.Search(query); // Zoeken
```

Het volgende voorbeeld demonstreert hoe u gefacetteerde zoekopdrachten kunt uitvoeren.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

string query = "content:Newton"; // Het woord voor de dubbele punt in de zoekopdracht betekent de naam van het documentveld waarin moet worden gezocht
SearchResult result = index.Search(query); // Zoeken
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Zoekopdrachten in index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| query | String | De zoekvraag. |
| options | SearchOptions | De zoekmogelijkheden. |

### Winstwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u fuzzy search uitvoert.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // De fuzzy search inschakelen
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Het aantal mogelijke verschillen voor elk woord instellen

// Dubbele aanhalingstekens aan het begin en einde vertellen de index dat het een zoekopdracht op woordgroep is
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Zoeken
```

Het volgende voorbeeld laat zien hoe u op synoniemen kunt zoeken.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Het zoeken naar synoniemen inschakelen

string query = "cry";
SearchResult result = index.Search(query, options); // Zoeken
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Zoekopdrachten in index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| query | SearchQuery | De zoekvraag. |

### Winstwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een zoekopdracht kunt uitvoeren met behulp van een query in objectvorm.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

// Subquery maken 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Zoekopties alleen instellen voor subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // De fuzzy search inschakelen
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Maximaal aantal verschillen instellen

// Subquery maken 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Subquery maken 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Subquery's combineren tot één query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Zoeken
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Zoekopdrachten in index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| query | SearchQuery | De zoekvraag. |
| options | SearchOptions | De zoekmogelijkheden. |

### Winstwaarde

Het zoekresultaat.

### Voorbeelden

Het volgende voorbeeld laat zien hoe u een zoekopdracht kunt uitvoeren met behulp van een query in objectvorm.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

// Subquery maken van zoeken in datumbereik
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Subquery van wildcard maken met aantal gemiste woorden van 0 tot 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Subquery maken van een eenvoudig woord
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Zoekopties alleen instellen voor subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Subquery's combineren tot één query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Een object met zoekopties maken met een grotere capaciteit van gevonden voorvallen
SearchOptions options = new SearchOptions(); // Algemene zoekopties
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Zoeken
```

### Zie ook

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Voert een reverse image search uit in de index.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| image | SearchImage | De afbeelding om te zoeken. |
| options | ImageSearchOptions | De zoekopties voor afbeeldingen. |

### Winstwaarde

Het resultaat van een reverse image search.

### Zie ook

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
