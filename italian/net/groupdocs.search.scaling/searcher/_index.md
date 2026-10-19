---
title: "Ricercatore"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un servizio che gestisce le query di ricerca verso i frammenti della rete di ricerca."
type: docs
weight: 1570
url: /it/net/groupdocs.search.scaling/searcher/
---
## Searcher class

Rappresenta un servizio che gestisce le query di ricerca verso i frammenti della rete di ricerca.

```csharp
public sealed class Searcher
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetDocumentText](../../groupdocs.search.scaling/searcher/getdocumenttext)(NetworkDocumentInfo, OutputAdapter) | Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output. |
| [GetIndexedDocumentItems](../../groupdocs.search.scaling/searcher/getindexeddocumentitems)(NetworkDocumentInfo) | Ottiene un array di elementi annidati del documento specificato (per documenti contenitori come ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search.scaling/searcher/getindexeddocuments)(int) | Ottiene un array di tutti i documenti indicizzati. |
| [Highlight](../../groupdocs.search.scaling/searcher/highlight)(NetworkFoundDocument, Highlighter, HighlightOptions) | Genera testo formattato in HTML con i termini trovati evidenziati. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst)(SearchImage, ImageSearchOptions) | Avvia una ricerca inversa di immagini nell'indice di ricerca distribuito. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst_1)(SearchQuery, SearchOptions) | Avvia una ricerca con una query in forma di oggetto nell'indice di ricerca distribuito. |
| [SearchFirst](../../groupdocs.search.scaling/searcher/searchfirst#searchfirst_2)(string, SearchOptions) | Avvia una ricerca con una query in forma di testo nell'indice di ricerca distribuito. |
| [SearchNext](../../groupdocs.search.scaling/searcher/searchnext#searchnext)(NetworkImageSearchToken) | Continua una ricerca inversa di immagini nell'indice di ricerca distribuito. |
| [SearchNext](../../groupdocs.search.scaling/searcher/searchnext#searchnext_1)(NetworkSearchToken) | Continua una ricerca nell'indice di ricerca distribuito. |

### Vedi anche

* namespace [GroupDocs.Search.Scaling](../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
