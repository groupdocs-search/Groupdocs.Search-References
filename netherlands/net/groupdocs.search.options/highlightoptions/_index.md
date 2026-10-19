---
title: "MarkeerOpties"
second_title: "GroupDocs.Search voor .NET API-referentie"
description: "Biedt opties voor het markeren van gevonden termen."
type: docs
weight: 910
url: /nl/net/groupdocs.search.options/highlightoptions/
---
## HighlightOptions class

Biedt opties voor het markeren van gevonden termen.

```csharp
public class HighlightOptions : TextOptions
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [HighlightOptions](highlightoptions)() | Initialiseert een nieuwe instantie van de [`HighlightOptions`](../highlightoptions) klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Haalt op of stelt de extra documentvelden in die werden gebruikt voor indexering. De standaardwaarde is `null`. Merk op dat deze waarde alleen wordt gebruikt als documenttekst niet in de index is opgeslagen. |
| [AutoDetectEncoding](../../groupdocs.search.options/baseoptions/autodetectencoding) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de codering automatisch moet worden gedetecteerd of niet. De standaardwaarde is `false`. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Haalt op of stelt het annuleringsobject in. De standaardwaarde is `null`. |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Haalt op of stelt de aangepaste tekst-extractor in die werd gebruikt voor indexering. De standaardwaarde is `null`. Merk op dat deze waarde alleen wordt gebruikt als documenttekst niet in de index is opgeslagen. |
| [Encoding](../../groupdocs.search.options/baseoptions/encoding) { get; set; } | Haalt op of stelt de codering in die wordt gebruikt om tekst uit tekstdocumenten te extraheren. De standaardwaarde is `null`, wat betekent dat de standaardcodering UTF-8 wordt gebruikt. Als AutoDetectEncoding `true` is, wordt deze waarde als de standaardcodering gebruikt. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de Head-tag wordt gegenereerd in de output-HTML. De standaardwaarde is `true`. |
| [HighlightColor](../../groupdocs.search.options/highlightoptions/highlightcolor) { get; set; } | Haalt op of stelt een kleur in die wordt gebruikt om voorkomens te markeren. De standaardwaarde is #FFD800. |
| [ImageIndexingOptions](../../groupdocs.search.options/baseoptions/imageindexingoptions) { get; } | Haalt de opties voor afbeeldingsindexering op voor omgekeerd zoeken naar afbeeldingen. |
| [MetadataIndexingOptions](../../groupdocs.search.options/baseoptions/metadataindexingoptions) { get; } | Haalt de opties voor het indexeren van metagegevensvelden op. |
| [OcrIndexingOptions](../../groupdocs.search.options/baseoptions/ocrindexingoptions) { get; } | Haalt de opties voor OCR-verwerking en het indexeren van herkende tekst op. |
| [TermHighlightEndTag](../../groupdocs.search.options/highlightoptions/termhighlightendtag) { get; set; } | Haalt op of stelt de eindtag in voor de markering van het gevonden woord. Deze tag wordt alleen gebruikt bij markering in platte tekst. De standaardwaarde is een lege tekenreeks. |
| [TermHighlightStartTag](../../groupdocs.search.options/highlightoptions/termhighlightstarttag) { get; set; } | Haalt op of stelt de starttag in voor de markering van het gevonden woord. Deze tag wordt alleen gebruikt bij markering in platte tekst. De standaardwaarde is een lege tekenreeks. |
| [TermsAfter](../../groupdocs.search.options/highlightoptions/termsafter) { get; set; } | Haalt op of stelt het maximale aantal woorden in een tekstfragment na het gemarkeerde woord in. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is `7`. |
| [TermsBefore](../../groupdocs.search.options/highlightoptions/termsbefore) { get; set; } | Haalt op of stelt het maximale aantal woorden in een tekstfragment vóór het gemarkeerde woord in. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is `7`. |
| [TermsTotal](../../groupdocs.search.options/highlightoptions/termstotal) { get; set; } | Haalt op of stelt het maximale aantal woorden in een tekstfragment in. De waarde moet liggen tussen 0 en 10000. De standaardwaarde is `21`. |
| [UseBackupPrivilege](../../groupdocs.search.options/baseoptions/usebackupprivilege) { get; set; } | Haalt op of stelt een waarde in die aangeeft of het proces de SeBackupPrivilege en FILE_FLAG_BACKUP_SEMANTICS moet gebruiken om toegang te krijgen tot bestanden en mappen. De standaardwaarde is `false`. |
| [UseInlineStyles](../../groupdocs.search.options/highlightoptions/useinlinestyles) { get; set; } | Haalt op of stelt een waarde in die aangeeft of inline stijlen worden gebruikt om voorkomens te markeren. De standaardwaarde is `true`. |
| [UseRawTextExtraction](../../groupdocs.search.options/baseoptions/userawtextextraction) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de ruwe modus wordt gebruikt voor tekstextractie indien mogelijk. De standaardwaarde is `false`. De ruwe modus kan de indexeringssnelheid aanzienlijk verhogen, maar de normale modus verbetert de opmaak van de geëxtraheerde tekst. |

### Opmerkingen

**Learn more**

* [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Zie ook

* class [TextOptions](../textoptions)
* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
