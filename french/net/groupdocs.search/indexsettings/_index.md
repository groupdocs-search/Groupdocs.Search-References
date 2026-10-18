---
title: "IndexSettings"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente les paramètres d'index qui permettent de personnaliser les opérations d'indexation."
type: docs
weight: 720
url: /fr/net/groupdocs.search/indexsettings/
---
## IndexSettings class

Représente les paramètres d'index qui permettent de personnaliser les opérations d'indexation.

```csharp
public class IndexSettings
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [IndexSettings](indexsettings)() | Initialise une nouvelle instance de la classe [`IndexSettings`](../indexsettings). |

## Propriétés

| Nom | Description |
| --- | --- |
| [CustomExtractors](../../groupdocs.search/indexsettings/customextractors) { get; } | Obtient la collection d'extracteurs personnalisés. |
| [DocumentFilter](../../groupdocs.search/indexsettings/documentfilter) { get; set; } | Obtient ou définit un filtre de documents. Le [`DocumentFilter`](./documentfilter) fonctionne selon la logique d'inclusion. Utilisez la classe [`DocumentFilter`](../../groupdocs.search.options/documentfilter) pour créer des instances de filtre de documents. La valeur par défaut est `null`, ce qui signifie que tous les documents ajoutés sont indexés. |
| [IndexType](../../groupdocs.search/indexsettings/indextype) { get; set; } | Obtient ou définit le type d'index. La valeur par défaut est NormalIndex. |
| [InMemoryIndex](../../groupdocs.search/indexsettings/inmemoryindex) { get; } | Obtient une valeur indiquant si l'index est stocké en mémoire ou sur le disque. |
| [Logger](../../groupdocs.search/indexsettings/logger) { get; set; } | Obtient ou définit un journaliseur utilisé pour consigner les événements et les erreurs dans l'index. Notez que le journaliseur n'est pas sauvegardé et doit être créé et assigné chaque fois que l'index est créé ou chargé. |
| [MaxIndexingReportCount](../../groupdocs.search/indexsettings/maxindexingreportcount) { get; set; } | Obtient ou définit le nombre maximal de rapports d'indexation. La valeur par défaut est `5`. |
| [MaxSearchReportCount](../../groupdocs.search/indexsettings/maxsearchreportcount) { get; set; } | Obtient ou définit le nombre maximal de rapports de recherche. La valeur par défaut est `10`. |
| [SearchThreads](../../groupdocs.search/indexsettings/searchthreads) { get; set; } | Obtient ou définit le nombre de threads utilisés pour la recherche. La valeur par défaut est Default, ce qui signifie que la recherche sera effectuée en utilisant un nombre de threads égal au nombre de cœurs du processeur. |
| [TextStorageSettings](../../groupdocs.search/indexsettings/textstoragesettings) { get; set; } | Obtient ou définit les paramètres de stockage du texte. La valeur par défaut est `null`, ce qui signifie que les textes des documents ne sont pas stockés. |
| [UseCharacterReplacements](../../groupdocs.search/indexsettings/usecharacterreplacements) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser les remplacements de caractères ou non. La valeur par défaut est `false`. |
| [UseStopWords](../../groupdocs.search/indexsettings/usestopwords) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser les mots vides ou non. La valeur par défaut est `true`. |

### Remarques

**Learn more**

* [Search index settings](https://docs.groupdocs.com/display/searchnet/Search+index+settings)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex; // Setting the index type

Index index = new Index(indexFolder, settings); // Creating an index
```

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
