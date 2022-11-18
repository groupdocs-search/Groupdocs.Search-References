---
title: Search
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Ricerche nellindice.
type: docs
weight: 220
url: /it/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Ricerche nell'indice.

```csharp
public SearchResult Search(string query)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| query | String | La domanda di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio seguente mostra come eseguire una ricerca semplice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchResult result = index.Search(query); // Ricerca
```

L'esempio seguente mostra come eseguire la ricerca Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

string query = "^[0-9]{3,}"; // Il simbolo dell'accento circonflesso all'inizio della query di ricerca indica all'indice che si tratta di una query Regex
SearchResult result = index.Search(query); // Ricerca
```

L'esempio seguente mostra come eseguire la ricerca con facet.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

string query = "content:Newton"; // La parola prima dei due punti nella query indica il nome del campo del documento da cercare
SearchResult result = index.Search(query); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Ricerche nell'indice.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| query | String | La domanda di ricerca. |
| options | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio seguente mostra come eseguire la ricerca fuzzy.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Abilitazione della ricerca fuzzy
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Impostazione del numero di possibili differenze per ogni parola

// Le doppie virgolette all'inizio e alla fine indicano all'indice che si tratta di una query di ricerca per frase
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Ricerca
```

L'esempio seguente mostra come eseguire la ricerca di sinonimi.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Abilitazione della ricerca dei sinonimi

string query = "cry";
SearchResult result = index.Search(query, options); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Ricerche nell'indice.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La domanda di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio seguente mostra come eseguire la ricerca utilizzando la query in forma di oggetto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

// Creazione della sottoquery 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Impostazione delle opzioni di ricerca solo per la sottoquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Abilitazione della ricerca fuzzy
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Impostazione del numero massimo di differenze

// Creazione della sottoquery 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Creazione della sottoquery 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combina le sottoquery in un'unica query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Ricerche nell'indice.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La domanda di ricerca. |
| options | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio seguente mostra come eseguire la ricerca utilizzando la query in forma di oggetto.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

// Creazione di una sottoquery della ricerca per intervallo di date
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Creazione di una sottoquery di caratteri jolly con numero di parole mancanti da 0 a 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Creazione di una sottoquery di una parola semplice
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Impostazione delle opzioni di ricerca solo per la sottoquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combina le sottoquery in un'unica query
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Creazione di un oggetto delle opzioni di ricerca con una maggiore capacità di occorrenze trovate
SearchOptions options = new SearchOptions(); // Opzioni generali di ricerca
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Esegue una ricerca inversa delle immagini nell'indice.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| image | SearchImage | L'immagine da cercare. |
| options | ImageSearchOptions | Le opzioni di ricerca delle immagini. |

### Valore di ritorno

Il risultato di una ricerca di immagini inversa.

### Guarda anche

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
