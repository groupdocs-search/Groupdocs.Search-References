---
title: "CreateAndQuery"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale."
type: docs
weight: 10
url: /it/net/groupdocs.search/searchquery/createandquery/
---
## CreateAndQuery(SearchQuery, SearchQuery) {#createandquery}

Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale.

```csharp
public static SearchQuery CreateAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| leftQuery | SearchQuery | La query figlio sinistro. |
| rightQuery | SearchQuery | La query figlio destro. |

### Valore di ritorno

Una query AND combinata.

### Vedi anche

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## CreateAndQuery(params SearchQuery[]) {#createandquery_1}

Crea una query combinata che troverà solo i documenti che verranno trovati per ciascuna query originale.

```csharp
public static SearchQuery CreateAndQuery(params SearchQuery[] queries)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery[] | Le query figlio. |

### Valore di ritorno

Una query AND combinata.

### Vedi anche

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
