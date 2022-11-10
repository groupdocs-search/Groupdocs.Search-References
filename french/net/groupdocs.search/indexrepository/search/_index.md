---
title: Search
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Recherche dans tous les index du référentiel.
type: docs
weight: 70
url: /fr/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Recherche dans tous les index du référentiel.

```csharp
public SearchResult Search(string query)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| query | String | La requête de recherche. |

### Return_Value

Le résultat de la recherche.

### Exemples

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Création de l'index
index.Add(documentsFolder); // Indexation des documents

SearchResult result = repository.Search(query); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* espace de noms [GroupDocs.Search](../../indexrepository)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Recherche dans tous les index du référentiel.

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

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Création de l'index
index.Add(documentsFolder); // Indexation des documents

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Définition du drapeau de recherche sensible à la casse

SearchResult result = repository.Search(query, options); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* espace de noms [GroupDocs.Search](../../indexrepository)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Recherche dans tous les index du référentiel.

```csharp
public SearchResult Search(SearchQuery query)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| query | SearchQuery | La requête de recherche. |

### Return_Value

Le résultat de la recherche.

### Exemples

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Création de l'index
index.Add(documentsFolder); // Indexation des documents

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Création d'une requête de recherche sous forme d'objet

SearchResult result = repository.Search(query); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* espace de noms [GroupDocs.Search](../../indexrepository)
* Assemblée [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Recherche dans tous les index du référentiel.

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

L'exemple montre comment effectuer une recherche dans le référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Création de l'index
index.Add(documentsFolder); // Indexation des documents

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Définition du drapeau de recherche sensible à la casse

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Création d'une requête de recherche sous forme d'objet

SearchResult result = repository.Search(query, options); // Recherche
```

### Voir également

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* espace de noms [GroupDocs.Search](../../indexrepository)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
