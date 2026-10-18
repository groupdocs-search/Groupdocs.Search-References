---
title: "SearchFirst"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Startet eine Suche mit einer Abfrage in Textform im verteilten Suchindex."
type: docs
weight: 50
url: /de/net/groupdocs.search.scaling/searcher/searchfirst/
---
## SearchFirst(string, SearchOptions) {#searchfirst_2}

Startet eine Suche mit einer Abfrage in Textform im verteilten Suchindex.

```csharp
public NetworkSearchResult SearchFirst(string query, SearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | String | Die Suchabfrage. |
| Optionen | Suchoptionen | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Siehe auch

* class [NetworkSearchResult](../../../groupdocs.search.scaling.results/networksearchresult)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## SearchFirst(SearchQuery, SearchOptions) {#searchfirst_1}

Startet eine Suche mit einer Abfrage in Objektform im verteilten Suchindex.

```csharp
public NetworkSearchResult SearchFirst(SearchQuery query, SearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Abfrage | SearchQuery | Die Suchabfrage. |
| Optionen | Suchoptionen | Die Suchoptionen. |

### Rückgabewert

Das Suchergebnis.

### Siehe auch

* class [NetworkSearchResult](../../../groupdocs.search.scaling.results/networksearchresult)
* class [SearchQuery](../../../groupdocs.search/searchquery)
* class [SearchOptions](../../../groupdocs.search.options/searchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## SearchFirst(SearchImage, ImageSearchOptions) {#searchfirst}

Startet eine umgekehrte Bildsuche im verteilten Suchindex.

```csharp
public NetworkImageSearchResult SearchFirst(SearchImage image, ImageSearchOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Bild | SearchImage | Das Bild, das durchsucht werden soll. |
| Optionen | ImageSearchOptions | Die Bildsuchoptionen. |

### Rückgabewert

Das Ergebnis der umgekehrten Bildsuche.

### Siehe auch

* class [NetworkImageSearchResult](../../../groupdocs.search.scaling.results/networkimagesearchresult)
* class [SearchImage](../../../groupdocs.search.common/searchimage)
* class [ImageSearchOptions](../../../groupdocs.search.options/imagesearchoptions)
* class [Searcher](../../searcher)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
