---
title: "Suche"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Durchsucht den Index."
type: docs
weight: 260
url: /de/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Durchsucht den Index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | String | Die Suchabfrage. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel demonstriert, wie man eine einfache Suche durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

Das folgende Beispiel demonstriert, wie man eine Regex-Suche durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

Das folgende Beispiel demonstriert, wie man eine facettierte Suche durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Durchsucht den Index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | String | Die Suchabfrage. |
| Optionen | Suchoptionen | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel demonstriert, wie man eine unscharfe Suche durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Anführungszeichen am Anfang und Ende teilen dem Index mit, dass es sich um eine Phrase‑Suchanfrage handelt.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

Das folgende Beispiel demonstriert, wie man eine Synonymsuche durchführt.

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

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Durchsucht den Index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | SearchQuery | Die Suchabfrage. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel demonstriert, wie man eine Suche mit einer Abfrage in Objektform durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Erstellen von Unterabfrage 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Erstelle Unterabfrage 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Erstelle Unterabfrage 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Kombiniere Unterabfragen zu einer Abfrage.
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Durchsucht den Index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | SearchQuery | Die Suchabfrage. |
| Optionen | Suchoptionen | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel demonstriert, wie man eine Suche mit einer Abfrage in Objektform durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Erstelle Unterabfrage der Datumsbereichssuche.
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Erstelle Unterabfrage des Platzhalters mit einer Anzahl fehlender Wörter von 0 bis 2.
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Erstelle Unterabfrage eines einfachen Wortes.
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombiniere Unterabfragen zu einer Abfrage.
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Erstelle Suchoptionsobjekt mit erhöhter Kapazität gefundener Vorkommen.
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Führt eine umgekehrte Bildsuche im Index durch.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Bild | SearchImage | Das Bild, das durchsucht werden soll. |
| Optionen | ImageSearchOptions | Die Bildsuchoptionen. |

### Rückgabewert

Das Ergebnis einer umgekehrten Bildsuche.

### Siehe auch

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
