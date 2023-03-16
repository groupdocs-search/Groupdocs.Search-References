---
title: ExtractionOptions
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Biedt opties voor het extraheren van gegevens uit documenten.
type: docs
weight: 820
url: /nl/net/groupdocs.search.options/extractionoptions/
---
## ExtractionOptions class

Biedt opties voor het extraheren van gegevens uit documenten.

```csharp
public class ExtractionOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [ExtractionOptions](extractionoptions)() | Initialiseert een nieuw exemplaar van het[`ExtractionOptions`](../extractionoptions) klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CustomExtractor](../../groupdocs.search.options/extractionoptions/customextractor) { get; set; } | Haalt de aangepaste tekstextractor op of stelt deze in. De standaardwaarde is`nul` . |
| [Encoding](../../groupdocs.search.options/extractionoptions/encoding) { get; set; } | Hiermee wordt de codering opgehaald of ingesteld die wordt gebruikt om uit tekstdocumenten te extraheren. |
| [ImageIndexingOptions](../../groupdocs.search.options/extractionoptions/imageindexingoptions) { get; } | Krijgt de opties voor het indexeren van afbeeldingen voor omgekeerd zoeken naar afbeeldingen. |
| [MetadataIndexingOptions](../../groupdocs.search.options/extractionoptions/metadataindexingoptions) { get; } | Krijgt de opties voor het indexeren van metadatavelden. |
| [OcrIndexingOptions](../../groupdocs.search.options/extractionoptions/ocrindexingoptions) { get; } | Krijgt de opties voor OCR-verwerking en indexering van herkende tekst. |
| [UseRawTextExtraction](../../groupdocs.search.options/extractionoptions/userawtextextraction) { get; set; } | Hiermee wordt een waarde opgehaald of ingesteld die aangeeft of de onbewerkte modus wordt gebruikt voor tekstextractie, indien mogelijk. De standaardwaarde is`WAAR` . De onbewerkte modus kan de indexeringssnelheid aanzienlijk verhogen, maar de normale modus verbetert de opmaak van de geëxtraheerde tekst. |

### Zie ook

* naamruimte [GroupDocs.Search.Options](../../groupdocs.search.options)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->