---
title: "CreateAndQuery"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale."
type: docs
weight: 10
url: /fr/net/groupdocs.search/searchquery/createandquery/
---
## CreateAndQuery(SearchQuery, SearchQuery) {#createandquery}

Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale.

```csharp
public static SearchQuery CreateAndQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| leftQuery | SearchQuery | La requête enfant gauche. |
| rightQuery | SearchQuery | La requête enfant droite. |

### Valeur de retour

Une requête AND combinée.

### Voir aussi

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## CreateAndQuery(params SearchQuery[]) {#createandquery_1}

Crée une requête combinée qui ne trouvera que les documents qui seront trouvés pour chaque requête originale.

```csharp
public static SearchQuery CreateAndQuery(params SearchQuery[] queries)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requêtes | SearchQuery[] | Les requêtes enfants. |

### Valeur de retour

Une requête AND combinée.

### Voir aussi

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
