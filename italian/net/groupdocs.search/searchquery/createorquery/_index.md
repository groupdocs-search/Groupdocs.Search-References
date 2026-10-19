---
title: "CreateOrQuery"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Crea una query combinata che troverà tutti i documenti che saranno trovati almeno per una delle query originali."
type: docs
weight: 60
url: /it/net/groupdocs.search/searchquery/createorquery/
---
## CreateOrQuery(SearchQuery, SearchQuery) {#createorquery}

Crea una query combinata che troverà tutti i documenti che saranno trovati almeno per una delle query originali.

```csharp
public static SearchQuery CreateOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| leftQuery | SearchQuery | La query figlio sinistro. |
| rightQuery | SearchQuery | La query figlio destro. |

### Valore di ritorno

Una query OR combinata.

### Vedi anche

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## CreateOrQuery(params SearchQuery[]) {#createorquery_1}

Crea una query combinata che troverà tutti i documenti che saranno trovati almeno per una delle query originali.

```csharp
public static SearchQuery CreateOrQuery(params SearchQuery[] queries)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| query | SearchQuery[] | Le query figlio. |

### Valore di ritorno

Una query OR combinata.

### Vedi anche

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
