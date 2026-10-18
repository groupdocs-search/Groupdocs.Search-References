---
title: "ImageSearchOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour l'opération de recherche d'images inversée."
type: docs
weight: 960
url: /fr/net/groupdocs.search.options/imagesearchoptions/
---
## ImageSearchOptions class

Fournit des options pour l'opération de recherche d'images inversée.

```csharp
public class ImageSearchOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [ImageSearchOptions](imagesearchoptions)() | Initialise une nouvelle instance de la classe [`ImageSearchOptions`](../imagesearchoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [HashDifferences](../../groupdocs.search.options/imagesearchoptions/hashdifferences) { get; set; } | Obtient ou définit le nombre maximal de bits non correspondants dans le hachage d'image. La valeur par défaut est `5`. |
| [MaxResultCount](../../groupdocs.search.options/imagesearchoptions/maxresultcount) { get; set; } | Obtient ou définit le nombre maximal d'images trouvées pour une requête de recherche d'image inversée. La valeur par défaut est `1000`. |
| [SearchDocumentFilter](../../groupdocs.search.options/imagesearchoptions/searchdocumentfilter) { get; set; } | Obtient ou définit le filtre de document de recherche. [`SearchDocumentFilter`](./searchdocumentfilter) fonctionne selon la logique d'inclusion. Utilisez la classe [`SearchDocumentFilter`](../searchdocumentfilter) pour créer des instances de filtre de document de recherche. La valeur par défaut est `null`, ce qui signifie que tous les documents trouvés seront retournés. |

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
