---
title: Search
second_title: GroupDocs.Search efter .NET API Reference
description: Söker i index.
type: docs
weight: 220
url: /sv/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Söker i index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| query | String | Sökfrågan. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man gör en enkel sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

SearchResult result = index.Search(query); // Söker
```

Följande exempel visar hur man utför Regex-sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

string query = "^[0-9]{3,}"; // Caret-symbolen i början av sökfrågan talar om för indexet att det är en Regex-fråga
SearchResult result = index.Search(query); // Söker
```

Följande exempel visar hur man utför facetterad sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

string query = "content:Newton"; // Ordet före kolon i frågan betyder dokumentfältsnamnet som ska sökas
SearchResult result = index.Search(query); // Söker
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Söker i index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| query | String | Sökfrågan. |
| options | SearchOptions | Sökalternativen. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför fuzzy sökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Aktiverar den otydliga sökningen
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Ställa in antalet möjliga skillnader för varje ord

// Dubbla citattecken i början och slutet talar om för indexet att det är en frassökning
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Söker
```

Följande exempel visar hur man utför synonymsökning.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Aktiverar synonymsökning

string query = "cry";
SearchResult result = index.Search(query, options); // Söker
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Söker i index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| query | SearchQuery | Sökfrågan. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför sökning med hjälp av fråga i objektform.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

// Skapa delfråga 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Ställa in sökalternativ endast för delfråga 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Aktiverar den otydliga sökningen
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Ställa in maximalt antal skillnader

// Skapa delfråga 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Skapa delfråga 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Kombinera delfrågor till en fråga
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Söker
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Söker i index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| query | SearchQuery | Sökfrågan. |
| options | SearchOptions | Sökalternativen. |

### Returvärde

Sökresultatet.

### Exempel

Följande exempel visar hur man utför sökning med hjälp av fråga i objektform.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Skapar index i den angivna mappen
index.Add(documentsFolder); // Indexering av dokument från den angivna mappen

// Skapar underfråga till datumintervallsökning
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Skapar underfråga av jokertecken med antalet missade ord från 0 till 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Skapar underfråga av enkelt ord
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Ställ in sökalternativ endast för delfråga 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombinera delfrågor till en fråga
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Skapar sökalternativsobjekt med ökad kapacitet för hittade förekomster
SearchOptions options = new SearchOptions(); // Övergripande sökalternativ
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Söker
```

### Se även

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Utför en omvänd bildsökning i indexet.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| image | SearchImage | Bilden att söka. |
| options | ImageSearchOptions | Alternativen för bildsökning. |

### Returvärde

Resultatet av en omvänd bildsökning.

### Se även

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namnutrymme [GroupDocs.Search](../../index)
* hopsättning [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
