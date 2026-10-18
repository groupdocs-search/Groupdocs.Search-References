---
title: "SearchFirst"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Démarre une recherche avec une requête sous forme de texte dans l'index de recherche distribué."
type: docs
weight: 50
url: /fr/net/groupdocs.search.scaling/searcher/searchfirst/
---
## SearchFirst(string, SearchOptions) {#searchfirst_2}

Démarre une recherche avec une requête sous forme de texte dans l'index de recherche distribué.

```csharp
public NetworkSearchResult SearchFirst(string query, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | String | La requête de recherche. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Le résultat de recherche.

### Voir aussi

* class [NetworkSearchResult](../../../groupdocs.search.scaling.results/networksearchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## SearchFirst(SearchQuery, SearchOptions) {#searchfirst_1}

Démarre une recherche avec une requête sous forme d'objet dans l'index de recherche distribué.

```csharp
public NetworkSearchResult SearchFirst(SearchQuery query, SearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requête | SearchQuery | La requête de recherche. |
| options | SearchOptions | Les options de recherche. |

### Valeur de retour

Le résultat de recherche.

### Voir aussi

* class [NetworkSearchResult](../../../groupdocs.search.scaling.results/networksearchresult)
* class [SearchQuery](../../../groupdocs.search/searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## SearchFirst(SearchImage, ImageSearchOptions) {#searchfirst}

Démarre une recherche d'image inversée dans l'index de recherche distribué.

```csharp
public NetworkImageSearchResult SearchFirst(SearchImage image, ImageSearchOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| image | SearchImage | L'image à rechercher. |
| options | ImageSearchOptions | Les options de recherche d'image. |

### Valeur de retour

Le résultat de recherche d'image inversée.

### Voir aussi

* class [NetworkImageSearchResult](../../../groupdocs.search.scaling.results/networkimagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
