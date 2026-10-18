---
title: "CreateOrQuery"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales."
type: docs
weight: 60
url: /fr/net/groupdocs.search/searchquery/createorquery/
---
## CreateOrQuery(SearchQuery, SearchQuery) {#createorquery}

Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales.

```csharp
public static SearchQuery CreateOrQuery(SearchQuery leftQuery, SearchQuery rightQuery)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| leftQuery | SearchQuery | La requête enfant gauche. |
| rightQuery | SearchQuery | La requête enfant droite. |

### Valeur de retour

Une requête OR combinée.

### Voir aussi

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## CreateOrQuery(params SearchQuery[]) {#createorquery_1}

Crée une requête combinée qui trouvera tous les documents qui seront trouvés au moins pour l'une des requêtes originales.

```csharp
public static SearchQuery CreateOrQuery(params SearchQuery[] queries)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| requêtes | SearchQuery[] | Les requêtes enfants. |

### Valeur de retour

Une requête OR combinée.

### Voir aussi

* class [SearchQuery](../../searchquery)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
