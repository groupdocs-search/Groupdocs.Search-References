---
title: "SearchDocumentFilter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Contient des méthodes pour créer des filtres de recherche de documents."
type: docs
weight: 1090
url: /fr/net/groupdocs.search.options/searchdocumentfilter/
---
## SearchDocumentFilter class

Contient des méthodes pour créer des filtres de recherche de documents.

```csharp
public static class SearchDocumentFilter
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/searchdocumentfilter/createand)(params ISearchDocumentFilter[]) | Crée une conjonction logique des filtres spécifiés. |
| static [CreateAttribute](../../groupdocs.search.options/searchdocumentfilter/createattribute)(params string[]) | Crée un filtre pour ignorer les documents qui n'ont aucune valeur dans la liste spécifiée d'attributs autorisés. |
| static [CreateFileExtension](../../groupdocs.search.options/searchdocumentfilter/createfileextension)(params string[]) | Crée un filtre pour ignorer les documents qui ne figurent pas dans la liste spécifiée des extensions possibles. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/searchdocumentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document. |
| static [CreateNot](../../groupdocs.search.options/searchdocumentfilter/createnot)(ISearchDocumentFilter) | Crée un filtre qui possède une logique inverse par rapport au filtre interne spécifié. |
| static [CreateOr](../../groupdocs.search.options/searchdocumentfilter/createor)(params ISearchDocumentFilter[]) | Crée une disjonction logique des filtres spécifiés. |

### Remarques

**Learn more**

* [Document filtering in search result](https://docs.groupdocs.com/display/searchnet/Document+filtering+in+search+result)
* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
