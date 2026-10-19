---
title: "SearchOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per l'operazione di ricerca."
type: docs
weight: 1100
url: /it/net/groupdocs.search.options/searchoptions/
---
## SearchOptions class

Fornisce opzioni per l'operazione di ricerca.

```csharp
public class SearchOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SearchOptions](searchoptions)() | Inizializza una nuova istanza della classe [`SearchOptions`](../searchoptions). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Cancellation](../../groupdocs.search.options/searchoptions/cancellation) { get; set; } | Ottiene o imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è `null`. |
| [DateFormats](../../groupdocs.search.options/searchoptions/dateformats) { get; } | Restituisce la raccolta di formati di data per la ricerca per intervallo di date. I formati di data predefiniti sono 'dd.MM.yyyy', 'MM/dd/yyyy' e 'yyyy-MM-dd'. |
| [FuzzySearch](../../groupdocs.search.options/searchoptions/fuzzysearch) { get; } | Restituisce le opzioni di ricerca fuzzy. |
| [IsChunkSearch](../../groupdocs.search.options/searchoptions/ischunksearch) { get; set; } | Ottiene o imposta il flag per la ricerca per blocchi. Il valore predefinito è `false`. |
| [KeyboardLayoutCorrector](../../groupdocs.search.options/searchoptions/keyboardlayoutcorrector) { get; } | Restituisce le opzioni del correttore di layout della tastiera. |
| [MaxOccurrenceCountPerTerm](../../groupdocs.search.options/searchoptions/maxoccurrencecountperterm) { get; set; } | Ottiene o imposta il numero massimo di occorrenze di ciascun termine in una query di ricerca. Il valore predefinito è `2000000000`. |
| [MaxTotalOccurrenceCount](../../groupdocs.search.options/searchoptions/maxtotaloccurrencecount) { get; set; } | Ottiene o imposta il numero totale massimo di occorrenze di tutti i termini in una query di ricerca. Il valore predefinito è `2000000000`. |
| [RetrieveAttributes](../../groupdocs.search.options/searchoptions/retrieveattributes) { get; set; } | Ottiene o imposta il flag per il recupero degli attributi associati ai documenti trovati. Il valore predefinito è `false`. |
| [SearchDocumentFilter](../../groupdocs.search.options/searchoptions/searchdocumentfilter) { get; set; } | Ottiene o imposta il filtro del documento di ricerca. [`SearchDocumentFilter`](./searchdocumentfilter) funziona sulla logica di inclusione. Usa la classe [`SearchDocumentFilter`](../searchdocumentfilter) per creare istanze del filtro del documento di ricerca. Il valore predefinito è `null`, il che significa che tutti i documenti trovati saranno restituiti. |
| [SpellingCorrector](../../groupdocs.search.options/searchoptions/spellingcorrector) { get; } | Restituisce le opzioni del correttore ortografico. |
| [UseCaseSensitiveSearch](../../groupdocs.search.options/searchoptions/usecasesensitivesearch) { get; set; } | Ottiene o imposta il flag per la ricerca sensibile al maiuscolo/minuscolo. Il valore predefinito è `false`. |
| [UseHomophoneSearch](../../groupdocs.search.options/searchoptions/usehomophonesearch) { get; set; } | Ottiene o imposta il flag per l'uso di omofoni nella ricerca. Il valore predefinito è `false`. |
| [UseSynonymSearch](../../groupdocs.search.options/searchoptions/usesynonymsearch) { get; set; } | Ottiene o imposta il flag per l'uso di sinonimi nella ricerca. Il valore predefinito è `false`. |
| [UseWordFormsSearch](../../groupdocs.search.options/searchoptions/usewordformssearch) { get; set; } | Ottiene o imposta il flag per l'uso di forme diverse delle parole nella ricerca. Il valore predefinito è `false`. |

### Osservazioni

**Learn more**

* [Search options](https://docs.groupdocs.com/display/searchnet/Search+options)

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
