---
title: "Sök"
second_title: "GroupDocs.Search för .NET API-referens"
description: "Söker i indexet."
type: docs
weight: 260
url: /sv/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Söker i indexet.

```csharp
public SearchResult Search(string query)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fråga | String | Sökfrågan. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför en enkel sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Följande exempel visar hur man utför en Regex-sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Följande exempel visar hur man utför en facetterad sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Söker i indexet.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fråga | String | Sökfrågan. |
| options | SearchOptions | Sökalternativen. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför en fuzzy-sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Dubbla citationstecken i början och slutet talar om för indexet att det är en fras-sökfråga.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Följande exempel visar hur man utför en synonym-sökning.

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

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Söker i indexet.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fråga | SearchQuery | Sökfrågan. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför en sökning med en fråga i objektform.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Skapar delfråga 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Skapar delfråga 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Skapar delfråga 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Kombinerar delfrågor till en fråga.
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Söker i indexet.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fråga | SearchQuery | Sökfrågan. |
| options | SearchOptions | Sökalternativen. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför en sökning med en fråga i objektform.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Skapar delfråga för datumintervallsökning.
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Skapar delfråga för jokertecken med antal saknade ord från 0 till 2.
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Skapar delfråga för enkelt ord.
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombinerar delfrågor till en fråga.
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Skapar sökalternativobjekt med ökad kapacitet för hittade förekomster.
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Utför en omvänd bildsökning i indexet.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bild | SearchImage | Bilden att söka efter. |
| options | ImageSearchOptions | Bildssökalternativen. |

### Returvärde

Resultatet av en omvänd bildsökning.

### Se även

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
