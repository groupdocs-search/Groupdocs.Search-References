---
title: HighlightOptions
second_title: GroupDocs.Search efter .NET API Reference
description: Ger alternativ för att markera hittade termer.
type: docs
weight: 830
url: /sv/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Ger alternativ för att markera hittade termer.

```csharp
public class HighlightOptions : TextOptions
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Initierar en ny instans av[`HighlightOptions`](../highlightoptions) class. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Hämtar eller ställer in de ytterligare dokumentfälten som användes för indexering. Standardvärdet är`null` . Observera att detta värde endast används om dokumenttexten inte sparades i indexet. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Hämtar eller ställer in annulleringsobjektet. Standardvärdet är`null` . |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Hämtar eller ställer in den anpassade textextraheraren som användes för indexering. Standardvärdet är`null` . Observera att detta värde endast används om dokumenttexten inte sparades i indexet. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Hämtar eller ställer in ett värde som indikerar om Head-taggen genereras i utdata-HTML. Standardvärdet är`Sann` . |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Hämtar eller ställer in en färg som används för att markera händelser. Standardvärdet är #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/textoptions/imageindexingoptions) { get; } | Hämtar bildindexeringsalternativen för omvänd bildsökning. |
| [MetadataIndexingOptions](../../groupdocs.search.options/textoptions/metadataindexingoptions) { get; } | Hämtar alternativen för att indexera metadatafält. |
| [OcrIndexingOptions](../../groupdocs.search.options/textoptions/ocrindexingoptions) { get; } | Får alternativen för OCR-bearbetning och indexering av igenkänd text. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Hämtar eller ställer in det maximala antalet ord i ett textfragment efter markerat ord. Värdet måste ligga i intervallet från 0 till 10000. Standardvärdet är`7` . |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Hämtar eller ställer in det maximala antalet ord i ett textfragment före det markerade ordet. Värdet måste ligga i intervallet från 0 till 10000. Standardvärdet är`7` . |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Hämtar eller ställer in det maximala antalet ord i ett textfragment. Värdet måste ligga i intervallet från 0 till 10000. Standardvärdet är`21` . |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Hämtar eller ställer in ett värde som anger om inline-stilar används för att markera förekomster. Standardvärdet är`Sann` . |

### Anmärkningar

**Läs mer**

* [Markera sökresultat](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Se även

* class [TextOptions](../textoptions)
* namnutrymme [GroupDocs.Search.Options](../../groupdocs.search.options)
* hopsättning [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->