---
title: "HighlightOptions"
second_title: "GroupDocs.Search för .NET API-referens"
description: "Tillhandahåller alternativ för att markera hittade termer."
type: docs
weight: 910
url: /sv/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Tillhandahåller alternativ för att markera hittade termer.

```csharp
public class HighlightOptions : TextOptions
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Initierar en ny instans av klassen [`HighlightOptions`](../highlightoptions). |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Hämtar eller anger de ytterligare dokumentfälten som användes för indexering. Standardvärdet är `null`. Observera att detta värde endast används om dokumenttexten inte sparades i indexet. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Hämtar eller anger ett värde som indikerar om kodning ska upptäckas automatiskt eller inte. Standardvärdet är `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Hämtar eller anger avbokningsobjektet. Standardvärdet är `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Hämtar eller anger den anpassade textextrahören som användes för indexering. Standardvärdet är `null`. Observera att detta värde endast används om dokumenttexten inte sparades i indexet. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Hämtar eller anger den kodning som används för att extrahera text från textdokument. Standardvärdet är `null`, vilket betyder att standardkodningen UTF-8 används. Om AutoDetectEncoding är `true` används detta värde som standardkodning. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Hämtar eller anger ett värde som indikerar om Head-taggen genereras i den utgående HTML:en. Standardvärdet är `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Hämtar eller anger en färg som används för att markera förekomster. Standardvärdet är #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Hämtar bildindexeringsalternativen för omvänd bildsökning. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Hämtar alternativen för indexering av metadatafält. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Hämtar alternativen för OCR-behandling och indexering av igenkänd text. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Hämtar eller anger sluttaggen för markeringen av det hittade ordet. Denna tagg används endast vid markering i vanlig text. Standardvärdet är en tom sträng. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Hämtar eller anger starttaggen för markeringen av det hittade ordet. Denna tagg används endast vid markering i vanlig text. Standardvärdet är en tom sträng. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Hämtar eller anger det maximala antalet ord i ett textfragment efter det markerade ordet. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Hämtar eller anger det maximala antalet ord i ett textfragment före det markerade ordet. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Hämtar eller anger det maximala antalet ord i ett textfragment. Värdet måste ligga i intervallet 0 till 10000. Standardvärdet är `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Hämtar eller anger ett värde som indikerar om processen ska använda SeBackupPrivilege och FILE_FLAG_BACKUP_SEMANTICS för att komma åt filer och kataloger. Standardvärdet är `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Hämtar eller anger ett värde som indikerar om inline‑stilar används för att markera förekomster. Standardvärdet är `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Hämtar eller anger ett värde som indikerar om råläge används för textutvinning om möjligt. Standardvärdet är `false`. Råläge kan avsevärt öka indexeringshastigheten, men normalt läge förbättrar formateringen av den extraherade texten. |

### Anmärkningar

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Se även

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
