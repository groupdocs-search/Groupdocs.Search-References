---
title: "SearchFirst"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Avvia una ricerca con una query in forma di testo nell'indice di ricerca distribuito."
type: docs
weight: 50
url: /it/net/groupdocs.search.scaling/searcher/searchfirst/
---
## SearchFirst(string, SearchOptions) {#searchfirst_2}

Avvia una ricerca con una query in forma di testo nell'indice di ricerca distribuito.

```csharp
public NetworkSearchResult SearchFirst(string query, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | String | La query di ricerca. |
| opzioni | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Vedi anche

* class [NetworkSearchResult](../../../groupdocs.search.scaling.results/networksearchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## SearchFirst(SearchQuery, SearchOptions) {#searchfirst_1}

Avvia una ricerca con una query in forma di oggetto nell'indice di ricerca distribuito.

```csharp
public NetworkSearchResult SearchFirst(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery | La query di ricerca. |
| opzioni | SearchOptions | Le opzioni di ricerca. |

### Valore di ritorno

Il risultato della ricerca.

### Vedi anche

* class [NetworkSearchResult](../../../groupdocs.search.scaling.results/networksearchresult)
* class [SearchQuery](../../../groupdocs.search/searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## SearchFirst(SearchImage, ImageSearchOptions) {#searchfirst}

Avvia una ricerca inversa di immagini nell'indice di ricerca distribuito.

```csharp
public NetworkImageSearchResult SearchFirst(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| immagine | SearchImage | L'immagine da cercare. |
| opzioni | ImageSearchOptions | Le opzioni di ricerca dell'immagine. |

### Valore di ritorno

Il risultato della ricerca inversa di immagini.

### Vedi anche

* class [NetworkImageSearchResult](../../../groupdocs.search.scaling.results/networkimagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
