---
title: "DocumentFilter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente la classe de base pour les filtres de documents. Contient des méthodes pour la création d'instances de filtres de documents."
type: docs
weight: 850
url: /fr/net/groupdocs.search.options/documentfilter/
---
## DocumentFilter class

Représente la classe de base pour les filtres de documents. Contient des méthodes pour la création d'instances de filtres de documents.

```csharp
public abstract class DocumentFilter
```

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateAnd](../../groupdocs.search.options/documentfilter/createand)(params DocumentFilter[]) | Crée une conjonction logique des filtres spécifiés. |
| static [CreateCreationTimeLowerBound](../../groupdocs.search.options/documentfilter/createcreationtimelowerbound)(DateTime) | Crée un filtre pour ignorer les documents dont la date de création est antérieure à la limite inférieure. |
| static [CreateCreationTimeRange](../../groupdocs.search.options/documentfilter/createcreationtimerange)(DateTime, DateTime) | Crée un filtre pour ignorer les documents dont la date de création est hors de la plage spécifiée. |
| static [CreateCreationTimeUpperBound](../../groupdocs.search.options/documentfilter/createcreationtimeupperbound)(DateTime) | Crée un filtre pour ignorer les documents dont la date de création est postérieure à la limite supérieure. |
| static [CreateFileExtension](../../groupdocs.search.options/documentfilter/createfileextension)(params string[]) | Crée un filtre pour ignorer les documents qui n'ont pas d'extension autorisée. |
| static [CreateFileLengthLowerBound](../../groupdocs.search.options/documentfilter/createfilelengthlowerbound)(long) | Crée un filtre pour ignorer les documents dont la longueur est inférieure à la limite inférieure. |
| static [CreateFileLengthRange](../../groupdocs.search.options/documentfilter/createfilelengthrange)(long, long) | Crée un filtre pour ignorer les documents hors de la plage de longueur spécifiée. |
| static [CreateFileLengthUpperBound](../../groupdocs.search.options/documentfilter/createfilelengthupperbound)(long) | Crée un filtre pour ignorer les documents dont la longueur est supérieure à la limite supérieure. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/documentfilter/createfilepathregularexpression#createfilepathregularexpression)(string) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document. |
| static [CreateFilePathRegularExpression](../../groupdocs.search.options/documentfilter/createfilepathregularexpression#createfilepathregularexpression_1)(string, RegexOptions) | Crée un filtre pour ignorer les documents qui ne correspondent pas à une expression régulière. L'expression régulière est appliquée au chemin complet d'un document. |
| static [CreateModificationTimeLowerBound](../../groupdocs.search.options/documentfilter/createmodificationtimelowerbound)(DateTime) | Crée un filtre pour ignorer les documents dont la date de modification est antérieure à la limite inférieure. |
| static [CreateModificationTimeRange](../../groupdocs.search.options/documentfilter/createmodificationtimerange)(DateTime, DateTime) | Crée un filtre pour ignorer les documents dont la date de modification est hors de la plage spécifiée. |
| static [CreateModificationTimeUpperBound](../../groupdocs.search.options/documentfilter/createmodificationtimeupperbound)(DateTime) | Crée un filtre pour ignorer les documents dont la date de modification est postérieure à la limite supérieure. |
| static [CreateNot](../../groupdocs.search.options/documentfilter/createnot)(DocumentFilter) | Crée un filtre qui possède une logique inverse par rapport au filtre interne spécifié. |
| static [CreateOr](../../groupdocs.search.options/documentfilter/createor)(params DocumentFilter[]) | Crée une disjonction logique des filtres spécifiés. |
| abstract [ToString](../../groupdocs.search.options/documentfilter/tostring)() | Renvoie la représentation sous forme de chaîne d'un filtre de document. |

### Remarques

**Learn more**

* [Document filtering during indexing](https://docs.groupdocs.com/display/searchnet/Document+filtering+during+indexing)

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
