---
title: "OcrIndexingOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour le traitement OCR et l'indexation du texte reconnu."
type: docs
weight: 1050
url: /fr/net/groupdocs.search.options/ocrindexingoptions/
---
## OcrIndexingOptions class

Fournit des options pour le traitement OCR et l'indexation du texte reconnu.

```csharp
public class OcrIndexingOptions
```

## Propriétés

| Nom | Description |
| --- | --- |
| [EnabledForContainerItemImages](../../groupdocs.search.options/ocrindexingoptions/enabledforcontaineritemimages) { get; set; } | Obtient ou définit une valeur indiquant s'il faut reconnaître le texte dans les images qui sont des éléments d'un conteneur (par exemple, des images dans une archive ZIP). La valeur par défaut est `false`. |
| [EnabledForEmbeddedImages](../../groupdocs.search.options/ocrindexingoptions/enabledforembeddedimages) { get; set; } | Obtient ou définit une valeur indiquant s'il faut reconnaître le texte dans les images intégrées (par exemple, des images dans un document DOCX). La valeur par défaut est `false`. |
| [EnabledForSeparateImages](../../groupdocs.search.options/ocrindexingoptions/enabledforseparateimages) { get; set; } | Obtient ou définit une valeur indiquant s'il faut reconnaître le texte dans des fichiers image séparés. La valeur par défaut est `false`. |
| [OcrConnector](../../groupdocs.search.options/ocrindexingoptions/ocrconnector) { get; set; } | Obtient ou définit un connecteur OCR utilisé pour le traitement OCR. La valeur par défaut est `null`, ce qui signifie qu'aucun OCR n'est utilisé. |

### Voir aussi

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
