---
title: SearchOptions
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Fornisce opzioni per loperazione di ricerca.
type: docs
weight: 1040
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
| [SearchOptions](searchoptions)() | Inizializza una nuova istanza di[`SearchOptions`](../searchoptions) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Cancellation](../../groupdocs.search.options/searchoptions/cancellation) { get; set; } | Ottiene o imposta l'oggetto di annullamento dell'operazione. Il valore predefinito è`nullo` . |
| [DateFormats](../../groupdocs.search.options/searchoptions/dateformats) { get; } | Recupera la raccolta di formati di data per la ricerca per intervallo di date. I formati di data predefiniti sono 'gg.MM.aaaa', 'MM/gg/aaaa' e 'aaaa-MM-gg'. |
| [FuzzySearch](../../groupdocs.search.options/searchoptions/fuzzysearch) { get; } | Ottiene le opzioni di ricerca fuzzy. |
| [IsChunkSearch](../../groupdocs.search.options/searchoptions/ischunksearch) { get; set; } | Ottiene o imposta il flag di ricerca per blocchi. Il valore predefinito è`falso` . |
| [KeyboardLayoutCorrector](../../groupdocs.search.options/searchoptions/keyboardlayoutcorrector) { get; } | Ottiene le opzioni del correttore del layout di tastiera. |
| [MaxOccurrenceCountPerTerm](../../groupdocs.search.options/searchoptions/maxoccurrencecountperterm) { get; set; } | Ottiene o imposta il numero massimo di occorrenze di ciascun termine in una query di ricerca. Il valore predefinito è`100000` . |
| [MaxTotalOccurrenceCount](../../groupdocs.search.options/searchoptions/maxtotaloccurrencecount) { get; set; } | Ottiene o imposta il numero totale massimo di occorrenze di tutti i termini in una query di ricerca. Il valore predefinito è`500000` . |
| [SearchDocumentFilter](../../groupdocs.search.options/searchoptions/searchdocumentfilter) { get; set; } | Ottiene o imposta il filtro del documento di ricerca. [`SearchDocumentFilter`](./searchdocumentfilter) lavora sulla logica di inclusione. Usa[`SearchDocumentFilter`](../searchdocumentfilter) class per la creazione di un documento di ricerca istanze di filtro. Il valore predefinito è`nullo` , il che significa che verranno restituiti tutti i documenti trovati. |
| [SpellingCorrector](../../groupdocs.search.options/searchoptions/spellingcorrector) { get; } | Ottiene le opzioni del correttore ortografico. |
| [UseCaseSensitiveSearch](../../groupdocs.search.options/searchoptions/usecasesensitivesearch) { get; set; } | Ottiene o imposta il flag della ricerca con distinzione tra maiuscole e minuscole. Il valore predefinito è`falso` . |
| [UseHomophoneSearch](../../groupdocs.search.options/searchoptions/usehomophonesearch) { get; set; } | Ottiene o imposta il flag di utilizzo degli omofoni nella ricerca. Il valore predefinito è`falso` . |
| [UseSynonymSearch](../../groupdocs.search.options/searchoptions/usesynonymsearch) { get; set; } | Ottiene o imposta il flag di utilizzo dei sinonimi nella ricerca. Il valore predefinito è`falso` . |
| [UseWordFormsSearch](../../groupdocs.search.options/searchoptions/usewordformssearch) { get; set; } | Ottiene o imposta il flag di utilizzo di diverse forme di parole nella ricerca. Il valore predefinito è`falso` . |

### Osservazioni

**Saperne di più**

* [opzioni di ricerca](https://docs.groupdocs.com/display/searchnet/Search+options)

### Guarda anche

* spazio dei nomi [GroupDocs.Search.Options](../../groupdocs.search.options)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
