---
title: Search
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Recherche dans lindex.
type: docs
weight: 220
url: /fr/net/groupdocs.search/index/search/
---
## Search(string) {#search_3}

Recherche dans l'index.

```csharp
public SearchResult Search(string query)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| query | String | La requête de recherche. |

### Return_Value

Le résultat de la recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche simple.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

SearchResult result = index.Search(query); // Recherche
```

L'exemple suivant montre comment effectuer une recherche Regex.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

string query = "^[0-9]{3,}"; // Le signe caret au début de la requête de recherche indique à l'index qu'il s'agit d'une requête Regex
SearchResult result = index.Search(query); // Recherche
```

L'exemple suivant montre comment effectuer une recherche à facettes.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

string query = "content:Newton"; // Le mot avant les deux-points dans la requête signifie le nom du champ de document à rechercher
SearchResult result = index.Search(query); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_4}

Recherche dans l'index.

```csharp
public SearchResult Search(string query, SearchOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| query | String | La requête de recherche. |
| options | SearchOptions | Les possibilités de recherche. |

### Return_Value

Le résultat de la recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche floue.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

SearchOptions options = new SearchOptions();
options.FuzzySearch.Enabled = true; // Activation de la recherche floue
options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1); // Définition du nombre de différences possibles pour chaque mot

// Les guillemets doubles au début et à la fin indiquent à l'index qu'il s'agit d'une requête de recherche d'expression
string query = "\"The Pursuit of Happiness\"";
SearchResult result = index.Search(query, options); // Recherche
```

L'exemple suivant montre comment effectuer une recherche de synonymes.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

SearchOptions options = new SearchOptions();
options.UseSynonymSearch = true; // Activer la recherche de synonymes

string query = "cry";
SearchResult result = index.Search(query, options); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search_1}

Recherche dans l'index.

```csharp
public SearchResult Search(SearchQuery query)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| query | SearchQuery | La requête de recherche. |

### Return_Value

Le résultat de la recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche à l'aide d'une requête sous forme d'objet.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

// Création de la sous-requête 1
SearchQuery subquery1 = SearchQuery.CreateWordQuery("accommodation");
subquery1.SearchOptions = new SearchOptions(); // Définition des options de recherche uniquement pour la sous-requête 1
subquery1.SearchOptions.FuzzySearch.Enabled = true; // Activation de la recherche floue
subquery1.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3); // Définition du nombre maximum de différences

// Création de la sous-requête 2
SearchQuery subquery2 = SearchQuery.CreateNumericRangeQuery(1, 1000000);

// Création de la sous-requête 3
SearchQuery subquery3 = SearchQuery.CreateRegexQuery(@"(.)\1");

// Combinaison de sous-requêtes en une seule requête
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

SearchResult result = index.Search(query); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_2}

Recherche dans l'index.

```csharp
public SearchResult Search(SearchQuery query, SearchOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| query | SearchQuery | La requête de recherche. |
| options | SearchOptions | Les possibilités de recherche. |

### Return_Value

Le résultat de la recherche.

### Exemples

L'exemple suivant montre comment effectuer une recherche à l'aide d'une requête sous forme d'objet.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Création d'un index dans le dossier spécifié
index.Add(documentsFolder); // Indexation des documents du dossier spécifié

// Création d'une sous-requête de recherche par plage de dates
SearchQuery subquery1 = SearchQuery.CreateDateRangeQuery(new DateTime(2011, 6, 17), new DateTime(2013, 1, 1));

// Création d'une sous-requête de caractère générique avec un nombre de mots manqués de 0 à 2
SearchQuery subquery2 = SearchQuery.CreateWildcardQuery(0, 2);

// Création d'une sous-requête de mot simple
SearchQuery subquery3 = SearchQuery.CreateWordQuery("birth");
subquery3.SearchOptions = new SearchOptions(); // Définition des options de recherche uniquement pour la sous-requête 3
subquery3.SearchOptions.FuzzySearch.Enabled = true;
subquery3.SearchOptions.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(1);

// Combinaison de sous-requêtes en une seule requête
SearchQuery query = SearchQuery.CreatePhraseSearchQuery(subquery1, subquery2, subquery3);

// Création d'un objet d'options de recherche avec une capacité accrue d'occurrences trouvées
SearchOptions options = new SearchOptions(); // Options de recherche globales
options.MaxOccurrenceCountPerTerm = 1000000;
options.MaxTotalOccurrenceCount = 10000000;

SearchResult result = index.Search(query, options); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(SearchImage, ImageSearchOptions) {#search}

Effectue une recherche d'image inversée dans l'index.

```csharp
public ImageSearchResult Search(SearchImage image, ImageSearchOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| image | SearchImage | L'image à rechercher. |
| options | ImageSearchOptions | Les options de recherche d'images. |

### Return_Value

Le résultat d'une recherche d'image inversée.

### Voir également

* class [ImageSearchResult](../../../groupdocs.search.results/imagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
