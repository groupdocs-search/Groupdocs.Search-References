---
title: "BaseOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options de base pour les opérations d'index."
type: docs
weight: 760
url: /fr/net/groupdocs.search.options/baseoptions/
---
## BaseOptions class

Fournit des options de base pour les opérations d'index.

```csharp
public abstract class BaseOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [BaseOptions](baseoptions)() | Initialise une nouvelle instance de la classe [`BaseOptions`](../baseoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Obtient ou définit une valeur indiquant s'il faut détecter automatiquement l'encodage ou non. La valeur par défaut est `false`. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Obtient ou définit l'encodage utilisé pour extraire le texte des documents texte. La valeur par défaut est `null`, ce qui signifie que l'encodage par défaut UTF-8 est utilisé. Si AutoDetectEncoding est `true`, alors cette valeur est utilisée comme encodage par défaut. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Obtient les options d'indexation d'image pour la recherche d'image inversée. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Obtient les options d'indexation des champs de métadonnées. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Obtient les options de traitement OCR et d'indexation du texte reconnu. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Obtient ou définit une valeur indiquant si le processus doit utiliser SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS pour accéder aux fichiers et répertoires. La valeur par défaut est `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Obtient ou définit une valeur indiquant si le mode brut est utilisé pour l'extraction de texte lorsque cela est possible. La valeur par défaut est `false`. Le mode brut peut augmenter considérablement la vitesse d'indexation, mais le mode normal améliore le formatage du texte extrait. |

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
