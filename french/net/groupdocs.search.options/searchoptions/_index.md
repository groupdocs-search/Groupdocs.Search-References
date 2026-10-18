---
title: "SearchOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour l'opération de recherche."
type: docs
weight: 1100
url: /fr/net/groupdocs.search.options/searchoptions/
---
## SearchOptions class

Fournit des options pour l'opération de recherche.

```csharp
public class SearchOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SearchOptions](searchoptions)() | Initialise une nouvelle instance de la classe [`SearchOptions`](../searchoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [Cancellation](../../groupdocs.search.options/searchoptions/cancellation) { get; set; } | Obtient ou définit l'objet d'annulation de l'opération. La valeur par défaut est `null`. |
| [DateFormats](../../groupdocs.search.options/searchoptions/dateformats) { get; } | Obtient la collection de formats de date pour la recherche de plage de dates. Les formats de date par défaut sont 'dd.MM.yyyy', 'MM/dd/yyyy' et 'yyyy-MM-dd'. |
| [FuzzySearch](../../groupdocs.search.options/searchoptions/fuzzysearch) { get; } | Obtient les options de recherche floue. |
| [IsChunkSearch](../../groupdocs.search.options/searchoptions/ischunksearch) { get; set; } | Obtient ou définit le drapeau de recherche par morceaux. La valeur par défaut est `false`. |
| [KeyboardLayoutCorrector](../../groupdocs.search.options/searchoptions/keyboardlayoutcorrector) { get; } | Obtient les options du correcteur de disposition du clavier. |
| [MaxOccurrenceCountPerTerm](../../groupdocs.search.options/searchoptions/maxoccurrencecountperterm) { get; set; } | Obtient ou définit le nombre maximal d'occurrences de chaque terme dans une requête de recherche. La valeur par défaut est `2000000000`. |
| [MaxTotalOccurrenceCount](../../groupdocs.search.options/searchoptions/maxtotaloccurrencecount) { get; set; } | Obtient ou définit le nombre total maximal d'occurrences de tous les termes dans une requête de recherche. La valeur par défaut est `2000000000`. |
| [RetrieveAttributes](../../groupdocs.search.options/searchoptions/retrieveattributes) { get; set; } | Obtient ou définit le drapeau de récupération des attributs associés aux documents trouvés. La valeur par défaut est `false`. |
| [SearchDocumentFilter](../../groupdocs.search.options/searchoptions/searchdocumentfilter) { get; set; } | Obtient ou définit le filtre de document de recherche. [`SearchDocumentFilter`](./searchdocumentfilter) fonctionne selon la logique d'inclusion. Utilisez la classe [`SearchDocumentFilter`](../searchdocumentfilter) pour créer des instances de filtre de document de recherche. La valeur par défaut est `null`, ce qui signifie que tous les documents trouvés seront retournés. |
| [SpellingCorrector](../../groupdocs.search.options/searchoptions/spellingcorrector) { get; } | Obtient les options du correcteur orthographique. |
| [UseCaseSensitiveSearch](../../groupdocs.search.options/searchoptions/usecasesensitivesearch) { get; set; } | Obtient ou définit le drapeau de recherche sensible à la casse. La valeur par défaut est `false`. |
| [UseHomophoneSearch](../../groupdocs.search.options/searchoptions/usehomophonesearch) { get; set; } | Obtient ou définit le drapeau d'utilisation des homophones dans la recherche. La valeur par défaut est `false`. |
| [UseSynonymSearch](../../groupdocs.search.options/searchoptions/usesynonymsearch) { get; set; } | Obtient ou définit le drapeau d'utilisation des synonymes dans la recherche. La valeur par défaut est `false`. |
| [UseWordFormsSearch](../../groupdocs.search.options/searchoptions/usewordformssearch) { get; set; } | Obtient ou définit le drapeau d'utilisation de différentes formes de mots dans la recherche. La valeur par défaut est `false`. |

### Remarques

**Learn more**

* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
