---
title: "Recherche"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Recherche dans l'index."
type: docs
weight: 260
url: /fr/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Recherche dans l'index.

```csharp
public SearchResult Search(string query)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | String | La requête de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche simple.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching
```

L'exemple suivant montre comment effectuer une recherche Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "^[0-9]{3,}"; // The caret symbol at the beginning of the search query tells the index that it is a Regex query
SearchResult result = index.Search(query); // Searching
```

L'exemple suivant montre comment effectuer une recherche à facettes.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

string query = "content:Newton"; // The word before the colon in the query means the document field name to search
SearchResult result = index.Search(query); // Searching
```

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Recherche dans l'index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | String | La requête de recherche. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche floue.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Enabling the fuzzy search
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Setting the number of possible differences for each word

// Les guillemets au début et à la fin indiquent à l'index qu'il s'agit d'une requête de recherche de phrase.
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Searching
```

L'exemple suivant montre comment effectuer une recherche de synonymes.

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

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Recherche dans l'index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | SearchQuery | La requête de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche en utilisant une requête sous forme d'objet.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Création de la sous-requête 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Setting search options only for subquery 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Enabling the fuzzy search
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Setting maximum number of differences

// Création de la sous-requête 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Création de la sous-requête 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combinaison des sous-requêtes en une seule requête
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Searching
```

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Recherche dans l'index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | SearchQuery | La requête de recherche. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Le résultat de recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche en utilisant une requête sous forme d'objet.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Création d'une sous-requête de recherche de plage de dates
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Création d'une sous-requête de caractère générique avec un nombre de mots manquants de 0 à 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Création d'une sous-requête de mot simple
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Setting search options only for subquery 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinaison des sous-requêtes en une seule requête
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Création d'un objet d'options de recherche avec une capacité accrue des occurrences trouvées
SearchOptions options = new SearchOptions(); // Overall search options
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Searching
```

### Voir aussi

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Effectue une recherche d'image inversée dans l'index.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| image | SearchImage | L'image à rechercher. |
| options | ImageSearchOptions | Les options de recherche d'image. |

### Valeur de retour

Le résultat d'une recherche d'image inversée.

### Voir aussi

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
