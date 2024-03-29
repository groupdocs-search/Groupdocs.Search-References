---
title: TextOptions
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Biedt opties voor het ophalen van documenttekst uit een index.
type: docs
weight: 1100
url: /nl/net/groupdocs.search.options/textoptions/
---
## TextOptions class

Biedt opties voor het ophalen van documenttekst uit een index.

```csharp
public class TextOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [TextOptions](textoptions)() | Initialiseert een nieuw exemplaar van het[`TextOptions`](../textoptions) klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.options/textoptions/additionalfields) { get; set; } | Haalt de aanvullende documentvelden op of stelt deze in die werden gebruikt voor indexering. De standaardwaarde is`nul`. Merk op dat deze waarde alleen wordt gebruikt als de documenttekst niet in de index is opgeslagen. |
| [Cancellation](../../groupdocs.search.options/textoptions/cancellation) { get; set; } | Haalt het annuleringsobject op of stelt het in. De standaardwaarde is`nul` . |
| [CustomExtractor](../../groupdocs.search.options/textoptions/customextractor) { get; set; } | Haalt de aangepaste tekstextractor op of stelt deze in die werd gebruikt voor indexering. De standaardwaarde is`nul`. Merk op dat deze waarde alleen wordt gebruikt als de documenttekst niet in de index is opgeslagen. |
| [GenerateHead](../../groupdocs.search.options/textoptions/generatehead) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de Head-tag wordt gegenereerd in de HTML-uitvoer. De standaardwaarde is`WAAR` . |
| [ImageIndexingOptions](../../groupdocs.search.options/textoptions/imageindexingoptions) { get; } | Krijgt de opties voor het indexeren van afbeeldingen voor omgekeerd zoeken naar afbeeldingen. |
| [MetadataIndexingOptions](../../groupdocs.search.options/textoptions/metadataindexingoptions) { get; } | Krijgt de opties voor het indexeren van metadatavelden. |
| [OcrIndexingOptions](../../groupdocs.search.options/textoptions/ocrindexingoptions) { get; } | Krijgt de opties voor OCR-verwerking en indexering van herkende tekst. |

### Opmerkingen

**Kom meer te weten**

* [Geïndexeerde documenten ophalen](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* [Zoekresultaten markeren](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Zie ook

* naamruimte [GroupDocs.Search.Options](../../groupdocs.search.options)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
