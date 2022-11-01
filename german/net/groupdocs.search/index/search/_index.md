---
title: Search
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Sucht im Index.
type: docs
weight: 220
url: /de/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Sucht im Index.

```csharp
public SearchResult Search(string query)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| query | String | Die Suchanfrage. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel zeigt, wie eine einfache Suche durchgeführt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

SearchResult result = index.Search(query); // Suchen
```

Das folgende Beispiel zeigt, wie eine Regex-Suche durchgeführt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

string query = "^[0-9]{3,}"; // Das Caret-Symbol am Anfang der Suchanfrage teilt dem Index mit, dass es sich um eine Regex-Abfrage handelt
SearchResult result = index.Search(query); // Suchen
```

Das folgende Beispiel zeigt, wie eine facettierte Suche durchgeführt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

string query = "content:Newton"; // Das Wort vor dem Doppelpunkt in der Abfrage bedeutet den Namen des zu durchsuchenden Dokumentfelds
SearchResult result = index.Search(query); // Suchen
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Sucht im Index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| query | String | Die Suchanfrage. |
| options | SearchOptions | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel zeigt, wie eine Fuzzy-Suche durchgeführt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Fuzzy-Suche aktivieren
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Festlegen der Anzahl möglicher Unterschiede für jedes Wort

// Doppelte Anführungszeichen am Anfang und am Ende teilen dem Index mit, dass es sich um eine Phrasensuchabfrage handelt
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Suchen
```

Das folgende Beispiel zeigt, wie man eine Synonymsuche durchführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Aktivierung der Synonymsuche

string query = "cry";
SearchResult result = index.Search(query, options); // Suchen
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Sucht im Index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| query | SearchQuery | Die Suchanfrage. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel zeigt, wie eine Suche mit einer Abfrage in Objektform durchgeführt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

// Unterabfrage 1 erstellen
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Suchoptionen nur für Unterabfrage 1 setzen
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Fuzzy-Suche aktivieren
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Festlegen der maximalen Anzahl von Unterschieden

// Unterabfrage 2 erstellen
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Unterabfrage 3 erstellen
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Kombinieren von Unterabfragen zu einer Abfrage
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Suchen
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Sucht im Index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| query | SearchQuery | Die Suchanfrage. |
| options | SearchOptions | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Beispiele

Das folgende Beispiel zeigt, wie eine Suche mit einer Abfrage in Objektform durchgeführt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

// Unterabfrage der Datumsbereichssuche erstellen
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Erstellen einer Unterabfrage des Platzhalters mit der Anzahl der fehlenden Wörter von 0 bis 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Unterabfrage eines einfachen Wortes erstellen
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Suchoptionen nur für Unterabfrage 3 setzen
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Kombinieren von Unterabfragen zu einer Abfrage
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Suchoptionsobjekt mit erhöhter Kapazität gefundener Vorkommen erstellen
SearchOptions options = new SearchOptions(); // Allgemeine Suchoptionen
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Suchen
```

### Siehe auch

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Führt eine umgekehrte Bildsuche im Index durch.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| image | SearchImage | Das zu durchsuchende Bild. |
| options | ImageSearchOptions | Die Bildsuchoptionen. |

### Rückgabewert

Das Ergebnis einer umgekehrten Bildsuche.

### Siehe auch

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
