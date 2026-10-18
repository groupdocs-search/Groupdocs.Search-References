---
title: "MetadataIndexingOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour l'indexation des champs de métadonnées."
type: docs
weight: 1020
url: /fr/net/groupdocs.search.options/metadataindexingoptions/
---
## MetadataIndexingOptions class

Fournit des options pour l'indexation des champs de métadonnées.

```csharp
public class MetadataIndexingOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [DefaultFieldName](../../groupdocs.search.options/metadataindexingoptions/defaultfieldname) { get; set; } | Obtient ou définit le nom de champ par défaut utilisé pour indexer les noms de champs vides. La valeur par défaut est `\"unknown\"`. |
| [IndexingEmptyNames](../../groupdocs.search.options/metadataindexingoptions/indexingemptynames) { get; set; } | Obtient ou définit une valeur indiquant s'il faut indexer les noms de champs vides ou non. La valeur par défaut est `true`. |
| [IndexingEmptyValues](../../groupdocs.search.options/metadataindexingoptions/indexingemptyvalues) { get; set; } | Obtient ou définit une valeur indiquant s'il faut indexer les valeurs de champs vides ou non. La valeur par défaut est `true`. |
| [MaxBytesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxbytestoindexfield) { get; set; } | Obtient ou définit le nombre maximal de valeurs dans un tableau de type byte pour indexer le champ. La valeur par défaut est `int.MaxValue`. |
| [MaxDoublesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxdoublestoindexfield) { get; set; } | Obtient ou définit le nombre maximal de valeurs dans un tableau de type double pour indexer le champ. La valeur par défaut est `int.MaxValue`. |
| [MaxIntsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxintstoindexfield) { get; set; } | Obtient ou définit le nombre maximal de valeurs dans un tableau de type int pour indexer le champ. La valeur par défaut est `int.MaxValue`. |
| [MaxLongsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxlongstoindexfield) { get; set; } | Obtient ou définit le nombre maximal de valeurs dans un tableau de type long pour indexer le champ. La valeur par défaut est `int.MaxValue`. |
| [SeparatorBetweenValues](../../groupdocs.search.options/metadataindexingoptions/separatorbetweenvalues) { get; set; } | Obtient ou définit le séparateur entre les valeurs dans un champ de type tableau. La valeur par défaut est le caractère espace. |
| [SeparatorInCompoundName](../../groupdocs.search.options/metadataindexingoptions/separatorincompoundname) { get; set; } | Obtient ou définit le séparateur dans le nom composé d'un champ. La valeur par défaut est `"."`. |

### Remarques

**Learn more**

* [Indexing options](https://docs.groupdocs.com/display/searchnet/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
