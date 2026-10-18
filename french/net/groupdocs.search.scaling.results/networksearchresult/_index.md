---
title: "NetworkSearchResult"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un résultat de recherche correspondant à une requête de recherche."
type: docs
weight: 1530
url: /fr/net/groupdocs.search.scaling.results/networksearchresult/
---
## NetworkSearchResult class

Représente un résultat de recherche correspondant à une requête de recherche.

```csharp
public class NetworkSearchResult : IEnumerable<NetworkFoundDocument>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DocumentCount](../../groupdocs.search.scaling.results/networksearchresult/documentcount) { get; } | Obtient le nombre de documents trouvés. |
| [EndTime](../../groupdocs.search.scaling.results/networksearchresult/endtime) { get; } | Obtient l'heure de fin de la recherche. |
| [NextChunkSearchToken](../../groupdocs.search.scaling.results/networksearchresult/nextchunksearchtoken) { get; } | Obtient un jeton de recherche de fragment pour rechercher le fragment suivant. |
| [NodeIndex](../../groupdocs.search.scaling.results/networksearchresult/nodeindex) { get; } | Obtient l'index du nœud dont le résultat a été reçu. |
| [OccurrenceCount](../../groupdocs.search.scaling.results/networksearchresult/occurrencecount) { get; } | Obtient le nombre total d'occurrences trouvées. |
| [SearchDuration](../../groupdocs.search.scaling.results/networksearchresult/searchduration) { get; } | Obtient la durée de la recherche. |
| [StartTime](../../groupdocs.search.scaling.results/networksearchresult/starttime) { get; } | Obtient l'heure de début de la recherche. |
| [Truncated](../../groupdocs.search.scaling.results/networksearchresult/truncated) { get; } | Obtient une valeur indiquant que le résultat est tronqué. |
| [Warnings](../../groupdocs.search.scaling.results/networksearchresult/warnings) { get; } | Obtient un avertissement décrivant le résultat. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetEnumerator](../../groupdocs.search.scaling.results/networksearchresult/getenumerator)() | Renvoie un énumérateur qui parcourt la collection des documents trouvés. |
| [GetFoundDocument](../../groupdocs.search.scaling.results/networksearchresult/getfounddocument)(int) | Obtient le document trouvé par indice. |

### Voir aussi

* class [NetworkFoundDocument](../networkfounddocument)
* namespace [GroupDocs.Search.Scaling.Results](../../groupdocs.search.scaling.results)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
