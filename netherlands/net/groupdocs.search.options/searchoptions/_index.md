---
title: SearchOptions
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Biedt opties voor zoeken.
type: docs
weight: 1040
url: /nl/net/groupdocs.search.options/searchoptions/
---
## SearchOptions class

Biedt opties voor zoeken.

```csharp
public class SearchOptions
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [SearchOptions](searchoptions)() | Initialiseert een nieuw exemplaar van het[`SearchOptions`](../searchoptions) klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Cancellation](../../groupdocs.search.options/searchoptions/cancellation) { get; set; } | Hiermee wordt het object voor het annuleren van de bewerking opgehaald of ingesteld. De standaardwaarde is`nul` . |
| [DateFormats](../../groupdocs.search.options/searchoptions/dateformats) { get; } | Haalt de verzameling datumnotaties op voor zoeken in datumbereiken. De standaard datumnotaties zijn 'dd.MM.jjjj', 'MM/dd/jjjj' en 'jjjj-MM-dd'. |
| [FuzzySearch](../../groupdocs.search.options/searchoptions/fuzzysearch) { get; } | Krijgt de vage zoekopties. |
| [IsChunkSearch](../../groupdocs.search.options/searchoptions/ischunksearch) { get; set; } | Haalt de zoekvlag op of stelt deze in op segmenten. De standaardwaarde is`vals` . |
| [KeyboardLayoutCorrector](../../groupdocs.search.options/searchoptions/keyboardlayoutcorrector) { get; } | Krijgt de opties voor de corrector van de toetsenbordindeling. |
| [MaxOccurrenceCountPerTerm](../../groupdocs.search.options/searchoptions/maxoccurrencecountperterm) { get; set; } | Hiermee wordt het maximale aantal keren dat elke term in een zoekopdracht voorkomt, opgehaald of ingesteld. De standaardwaarde is`100000` . |
| [MaxTotalOccurrenceCount](../../groupdocs.search.options/searchoptions/maxtotaloccurrencecount) { get; set; } | Hiermee wordt het maximale totale aantal keren dat alle termen in een zoekopdracht voorkomen, opgehaald of ingesteld. De standaardwaarde is`500000` . |
| [SearchDocumentFilter](../../groupdocs.search.options/searchoptions/searchdocumentfilter) { get; set; } | Haalt of stelt het zoekdocumentfilter in. [`SearchDocumentFilter`](./searchdocumentfilter) werkt op de integratielogica. Gebruik[`SearchDocumentFilter`](../searchdocumentfilter) klasse voor het maken van een zoekdocument filterinstanties. De standaardwaarde is`nul` , wat betekent dat alle gevonden documenten worden geretourneerd. |
| [SpellingCorrector](../../groupdocs.search.options/searchoptions/spellingcorrector) { get; } | Krijgt de opties voor spellingcorrector. |
| [UseCaseSensitiveSearch](../../groupdocs.search.options/searchoptions/usecasesensitivesearch) { get; set; } | Hiermee wordt de vlag van hoofdlettergevoelig zoeken opgehaald of ingesteld. De standaardwaarde is`vals` . |
| [UseHomophoneSearch](../../groupdocs.search.options/searchoptions/usehomophonesearch) { get; set; } | Haalt of stelt de vlag van gebruik homofonen in zoeken in. De standaardwaarde is`vals` . |
| [UseSynonymSearch](../../groupdocs.search.options/searchoptions/usesynonymsearch) { get; set; } | Haalt of stelt de vlag van gebruikssynoniemen in zoeken in. De standaardwaarde is`vals` . |
| [UseWordFormsSearch](../../groupdocs.search.options/searchoptions/usewordformssearch) { get; set; } | Haalt of stelt de vlag in van het gebruik van verschillende woordvormen in zoekopdrachten. De standaardwaarde is`vals` . |

### Opmerkingen

**Kom meer te weten**

* [zoek opties](https://docs.groupdocs.com/display/searchnet/Search+options)

### Zie ook

* naamruimte [GroupDocs.Search.Options](../../groupdocs.search.options)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->