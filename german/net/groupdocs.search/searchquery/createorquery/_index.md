---
title: "CreateOrQuery"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden."
type: docs
weight: 60
url: /de/net/groupdocs.search/searchquery/createorquery/
---
## CreateOrQuery(SearchQuery, SearchQuery) {#createorquery}

Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden.

```csharp
public static SearchQuery CreateOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| leftQuery | SearchQuery | Die linke Kindabfrage. |
| rightQuery | SearchQuery | Die rechte Kindabfrage. |

### Rückgabewert

Eine kombinierte ODER-Abfrage.

### Siehe auch

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## CreateOrQuery(params SearchQuery[]) {#createorquery_1}

Erstellt eine kombinierte Abfrage, die alle Dokumente findet, die mindestens für eine der ursprünglichen Abfragen gefunden werden.

```csharp
public static SearchQuery CreateOrQuery(params SearchQuery[] queries)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| queries | SearchQuery[] | Die Kindabfragen. |

### Rückgabewert

Eine kombinierte ODER-Abfrage.

### Siehe auch

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
