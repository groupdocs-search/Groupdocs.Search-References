---
title: "CreateAndQuery"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden."
type: docs
weight: 10
url: /de/net/groupdocs.search/searchquery/createandquery/
---
## CreateAndQuery(SearchQuery, SearchQuery) {#createandquery}

Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden.

```csharp
public static SearchQuery CreateAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| leftQuery | SearchQuery | Die linke Kindabfrage. |
| rightQuery | SearchQuery | Die rechte Kindabfrage. |

### Rückgabewert

Eine kombinierte AND-Abfrage.

### Siehe auch

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## CreateAndQuery(params SearchQuery[]) {#createandquery_1}

Erstellt eine kombinierte Abfrage, die nur Dokumente findet, die für jede ursprüngliche Abfrage gefunden werden.

```csharp
public static SearchQuery CreateAndQuery(params SearchQuery[] queries)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| queries | SearchQuery[] | Die Kindabfragen. |

### Rückgabewert

Eine kombinierte AND-Abfrage.

### Siehe auch

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
