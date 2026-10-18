---
title: "IndexingOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour l'opération d'indexation."
type: docs
weight: 980
url: /fr/net/groupdocs.search.options/indexingoptions/
---
## IndexingOptions class

Fournit des options pour l'opération d'indexation.

```csharp
public class IndexingOptions : BaseOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [IndexingOptions](indexingoptions)() | Initialise une nouvelle instance de la classe [`IndexingOptions`](../indexingoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Obtient ou définit une valeur indiquant s'il faut détecter automatiquement l'encodage ou non. La valeur par défaut est `false`. |
| [Cancellation](../../groupdocs.search.options/indexingoptions/cancellation) { get; set; } | Obtient ou définit l'objet d'annulation de l'opération. La valeur par défaut est `null`. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Obtient ou définit l'encodage utilisé pour extraire le texte des documents texte. La valeur par défaut est `null`, ce qui signifie que l'encodage par défaut UTF-8 est utilisé. Si AutoDetectEncoding est `true`, alors cette valeur est utilisée comme encodage par défaut. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Obtient les options d'indexation d'image pour la recherche d'image inversée. |
| [IsAsync](../../groupdocs.search.options/indexingoptions/isasync) { get; set; } | Obtient ou définit le drapeau d'exécution asynchrone de l'opération. La valeur par défaut est `false`. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Obtient les options d'indexation des champs de métadonnées. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Obtient les options de traitement OCR et d'indexation du texte reconnu. |
| [SeparateProcessOptions](../../groupdocs.search.options/indexingoptions/separateprocessoptions) { get; } | Obtient les options d'extraction des données dans un processus séparé. |
| [Threads](../../groupdocs.search.options/indexingoptions/threads) { get; set; } | Obtient ou définit le nombre de threads utilisés pour l'indexation. Le paramètre doit être compris entre `1` et `4`. La valeur par défaut est `1`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Obtient ou définit une valeur indiquant si le processus doit utiliser SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS pour accéder aux fichiers et répertoires. La valeur par défaut est `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Obtient ou définit une valeur indiquant si le mode brut est utilisé pour l'extraction de texte lorsque cela est possible. La valeur par défaut est `false`. Le mode brut peut augmenter considérablement la vitesse d'indexation, mais le mode normal améliore le formatage du texte extrait. |

### Remarques

**Learn more**

* [Indexing options](https://docs.groupdocs.com/display/searchnet/Indexing+options)

### Voir aussi

* class [BaseOptions](../baseoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
