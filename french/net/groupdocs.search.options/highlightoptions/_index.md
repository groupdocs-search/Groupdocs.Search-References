---
title: "HighlightOptions"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des options pour mettre en évidence les termes trouvés."
type: docs
weight: 910
url: /fr/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Fournit des options pour mettre en évidence les termes trouvés.

```csharp
public class HighlightOptions : TextOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Initialise une nouvelle instance de la classe [`HighlightOptions`](../highlightoptions). |

## Propriétés

| Nom | Description |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Obtient ou définit les champs de document supplémentaires qui ont été utilisés pour l'indexation. La valeur par défaut est `null`. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Obtient ou définit une valeur indiquant s'il faut détecter automatiquement l'encodage ou non. La valeur par défaut est `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Obtient ou définit l'objet d'annulation. La valeur par défaut est `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Obtient ou définit l'extracteur de texte personnalisé qui a été utilisé pour l'indexation. La valeur par défaut est `null`. Notez que cette valeur n'est utilisée que si le texte du document n'a pas été enregistré dans l'index. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Obtient ou définit l'encodage utilisé pour extraire le texte des documents texte. La valeur par défaut est `null`, ce qui signifie que l'encodage par défaut UTF-8 est utilisé. Si AutoDetectEncoding est `true`, alors cette valeur est utilisée comme encodage par défaut. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Obtient ou définit une valeur indiquant si la balise Head est générée dans le HTML de sortie. La valeur par défaut est `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Obtient ou définit une couleur utilisée pour mettre en évidence les occurrences. La valeur par défaut est #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Obtient les options d'indexation d'image pour la recherche d'image inversée. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Obtient les options d'indexation des champs de métadonnées. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Obtient les options de traitement OCR et d'indexation du texte reconnu. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Obtient ou définit la balise de fin du surlignage du mot trouvé. Cette balise n'est utilisée que lors du surlignage en texte brut. La valeur par défaut est une chaîne vide. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Obtient ou définit la balise de début du surlignage du mot trouvé. Cette balise n'est utilisée que lors du surlignage en texte brut. La valeur par défaut est une chaîne vide. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Obtient ou définit le nombre maximal de mots dans un fragment de texte après le mot surligné. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Obtient ou définit le nombre maximal de mots dans un fragment de texte avant le mot surligné. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Obtient ou définit le nombre maximal de mots dans un fragment de texte. La valeur doit être comprise entre 0 et 10000. La valeur par défaut est `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Obtient ou définit une valeur indiquant si le processus doit utiliser SeBackupPrivilege et FILE_FLAG_BACKUP_SEMANTICS pour accéder aux fichiers et répertoires. La valeur par défaut est `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Obtient ou définit une valeur indiquant si des styles en ligne sont utilisés pour surligner les occurrences. La valeur par défaut est `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Obtient ou définit une valeur indiquant si le mode brut est utilisé pour l'extraction de texte lorsque cela est possible. La valeur par défaut est `false`. Le mode brut peut augmenter considérablement la vitesse d'indexation, mais le mode normal améliore le formatage du texte extrait. |

### Remarques

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Voir aussi

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
