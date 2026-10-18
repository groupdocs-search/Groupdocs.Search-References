---
title: "IndexRepository"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un conteneur permettant de combiner plusieurs index et d'exécuter des opérations communes sur ceux-ci."
type: docs
weight: 710
url: /fr/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Représente un conteneur permettant de combiner plusieurs index et d'exécuter des opérations communes sur ceux-ci.

```csharp
public class IndexRepository : IDisposable
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [IndexRepository](indexrepository)() | Initialise une nouvelle instance de la classe [`IndexRepository`](../indexrepository). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Obtient le hub d'événements pour s'abonner aux événements. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Obtient les index contenus dans ce [`IndexRepository`](../indexrepository). |

## Méthodes

| Nom | Description |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Ajoute un index au référentiel d'index. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Ouvre et ajoute un index au référentiel d'index. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Crée un nouvel index en mémoire. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Crée un nouvel index en mémoire. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Crée un nouvel index sur disque. Le dossier d'index sera nettoyé avant la création de l'index. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Crée un nouvel index sur disque. Le dossier d'index sera nettoyé avant la création de l'index. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Libère toutes les ressources utilisées par le [`IndexRepository`](../indexrepository). |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Recherche dans tous les index du référentiel. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Recherche dans tous les index du référentiel. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Recherche dans tous les index du référentiel. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Recherche dans tous les index du référentiel. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Met à jour tous les index du référentiel. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Met à jour tous les index du référentiel. |

### Remarques

**Learn more**

* [Search index repository](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Loading an existing index
repository.AddToRepository(indexFolder2); // Loading another existing index

SearchResult result = repository.Search(query); // Searching in indexes of the repository
```

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
