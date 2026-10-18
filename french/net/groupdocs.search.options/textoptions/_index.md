---
title: "TextOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour récupérer le texte du document depuis un index."
type: docs
weight: 1180
url: /fr/net/groupdocs.search.options/textoptions/
---
## TextOptions class

Fournit des options pour récupérer le texte du document depuis un index.

```csharp
public class TextOptions : BaseOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [TextOptions](textoptions)() | Initialise une nouvelle instance de la classe [`TextOptions`](../textoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Obtient ou définit les champs de document supplémentaires qui ont été utilisés pour l'indexation. La valeur par défaut est `null`. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Obtient ou définit une valeur indiquant s'il faut détecter automatiquement l'encodage ou non. La valeur par défaut est `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Obtient ou définit l'objet d'annulation. La valeur par défaut est `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Obtient ou définit l'extracteur de texte personnalisé qui a été utilisé pour l'indexation. La valeur par défaut est `null`. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Obtient ou définit l'encodage utilisé pour extraire le texte des documents texte. La valeur par défaut est `null`, ce qui signifie que l'encodage par défaut UTF-8 est utilisé. Si AutoDetectEncoding est `true`, alors cette valeur est utilisée comme encodage par défaut. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Obtient ou définit une valeur indiquant si la balise Head est générée dans le HTML de sortie. La valeur par défaut est `true`. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Obtient les options d'indexation d'image pour la recherche d'image inversée. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Obtient les options d'indexation des champs de métadonnées. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Obtient les options de traitement OCR et d'indexation du texte reconnu. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Obtient ou définit une valeur indiquant si le processus doit utiliser SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS pour accéder aux fichiers et répertoires. La valeur par défaut est `false`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Obtient ou définit une valeur indiquant si le mode brut est utilisé pour l'extraction de texte lorsque cela est possible. La valeur par défaut est `false`. Le mode brut peut augmenter considérablement la vitesse d'indexation, mais le mode normal améliore le formatage du texte extrait. |

### Remarques

**Learn more**

* [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Voir aussi

* class [BaseOptions](../baseoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
