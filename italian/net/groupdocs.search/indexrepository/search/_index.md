---
title: Search
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Cerca in tutti gli indici del repository.
type: docs
weight: 70
url: /it/net/groupdocs.search/indexrepository/search/
---
## Search(string) {#search_2}

Cerca in tutti gli indici del repository.

```csharp
public SearchResult Search(string query)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| query | String | La domanda di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio mostra come eseguire la ricerca nel repository dell'indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creazione indice
index.Add(documentsFolder); // Indicizzazione dei documenti

SearchResult result = repository.Search(query); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [IndexRepository](../../indexrepository)
* spazio dei nomi [GroupDocs.Search](../../indexrepository)
* assemblea [GroupDocs.Search](../../../)

---

## Search(string, SearchOptions) {#search_3}

Cerca in tutti gli indici del repository.

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

L'esempio mostra come eseguire la ricerca nel repository dell'indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creazione indice
index.Add(documentsFolder); // Indicizzazione dei documenti

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Impostazione del flag di ricerca con distinzione tra maiuscole e minuscole

SearchResult result = repository.Search(query, options); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* spazio dei nomi [GroupDocs.Search](../../indexrepository)
* assemblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery) {#search}

Cerca in tutti gli indici del repository.

```csharp
public SearchResult Search(SearchQuery query)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La domanda di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Esempi

L'esempio mostra come eseguire la ricerca nel repository dell'indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creazione indice
index.Add(documentsFolder); // Indicizzazione dei documenti

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creazione di una query di ricerca in forma di oggetto

SearchResult result = repository.Search(query); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [IndexRepository](../../indexrepository)
* spazio dei nomi [GroupDocs.Search](../../indexrepository)
* assemblea [GroupDocs.Search](../../../)

---

## Search(SearchQuery, SearchOptions) {#search_1}

Cerca in tutti gli indici del repository.

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

L'esempio mostra come eseguire la ricerca nel repository dell'indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();
Index index = repository.Create(indexFolder); // Creazione indice
index.Add(documentsFolder); // Indicizzazione dei documenti

SearchOptions options = new SearchOptions();
options.UseCaseSensitiveSearch = true; // Impostazione del flag di ricerca con distinzione tra maiuscole e minuscole

SearchQuery query = SearchQuery.CreateWordQuery("Einstein"); // Creazione di una query di ricerca in forma di oggetto

SearchResult result = repository.Search(query, options); // Ricerca
```

### Guarda anche

* class [SearchResult](../../../groupdocs.search.results/searchresult)
* class [SearchQuery](../../searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [IndexRepository](../../indexrepository)
* spazio dei nomi [GroupDocs.Search](../../indexrepository)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
