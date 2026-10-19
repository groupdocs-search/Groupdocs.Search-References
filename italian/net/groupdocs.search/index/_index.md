---
title: "Index"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta la classe principale per indicizzare i documenti e cercarli."
type: docs
weight: 700
url: /it/net/groupdocs.search/index/
---
## Index class

Rappresenta la classe principale per indicizzare i documenti e cercarli.

```csharp
public class Index : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Index](index#constructor)() | Inizializza una nuova istanza della classe [`Index`](../index) in memoria. |
| [Index](index#constructor_1)(IndexSettings) | Inizializza una nuova istanza della classe [`Index`](../index) in memoria con impostazioni di indice specifiche. |
| [Index](index#constructor_2)(string) | Inizializza una nuova istanza della classe [`Index`](../index). Crea un nuovo indice o apre un indice esistente su disco. |
| [Index](index#constructor_3)(string, bool) | Inizializza una nuova istanza della classe [`Index`](../index). Carica un indice esistente da disco se *overwriteIfExists* è `false`; altrimenti crea un nuovo indice su disco. |
| [Index](index#constructor_4)(string, IndexSettings) | Inizializza una nuova istanza della classe [`Index`](../index). Crea un nuovo indice con impostazioni particolari o apre un indice esistente sul disco. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Inizializza una nuova istanza della classe [`Index`](../index). Carica un indice esistente dal disco se *overwriteIfExists* è `false`; altrimenti crea un nuovo indice sul disco con impostazioni specifiche dell'indice. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Ottiene il repository del dizionario. |
| [Events](../../groupdocs.search/index/events) { get; } | Ottiene il hub degli eventi per l'iscrizione agli eventi. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Ottiene le informazioni di base sull'indice. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Ottiene le impostazioni dell'indice. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Ottiene l'oggetto repository dell'indice se l'indice è contenuto in esso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely)(string) | Carica l'intero indice in memoria. Eventuali modifiche all'indice non vengono salvate automaticamente nella cartella originale. |
| static [LoadIntoMemoryCompletely](../../groupdocs.search/index/loadintomemorycompletely#loadintomemorycompletely_1)(string, IndexSettings) | Carica l'intero indice in memoria. Eventuali modifiche all'indice non vengono salvate automaticamente nella cartella originale. |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Esegue l'operazione di indicizzazione. Aggiunge un file o una cartella tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Esegue l'operazione di indicizzazione. Aggiunge file o cartelle tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Esegue l'operazione di indicizzazione. Aggiunge documenti dal file system, dallo stream o dalla struttura. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Esegue l'operazione di indicizzazione. Aggiunge i dati estratti all'indice. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Esegue l'operazione di indicizzazione. Aggiunge un file o una cartella tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Esegue l'operazione di indicizzazione. Aggiunge file o cartelle tramite un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzare durante l'operazione di aggiornamento. |
| [CheckSegments](../../groupdocs.search/index/checksegments)(bool) | Controlla l'indice per file di segmento danneggiati sul disco. Il metodo ripara la funzionalità dell'indice in presenza di segmenti danneggiati, se *fixIndexFunctionality* è true; altrimenti non ripara. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Elimina file o cartelle indicizzate dall'indice. Quindi aggiorna l'indice senza i percorsi eliminati. Nota che un documento individuale non può essere eliminato dall'indice se è stato aggiunto all'indice come parte di una cartella. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Elimina i documenti indicizzati da stream o strutture. Quindi aggiorna l'indice senza i documenti eliminati. |
| [Dispose](../../groupdocs.search/index/dispose)() | Rilascia tutte le risorse utilizzate da [`Index`](../index). |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Ottiene tutti gli attributi associati al documento indicizzato specificato. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genera testo formattato in HTML per il documento indicizzato e lo trasferisce attraverso l'adattatore di output. |
| [GetIndexedDocument](../../groupdocs.search/index/getindexeddocument)(string) | Ottiene un documento indicizzato tramite la chiave del documento. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Ottiene un array di elementi annidati del documento specificato (per documenti contenitori come ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Ottiene un array di tutti i documenti indicizzati. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Ottiene un array di percorsi indicizzati - documenti o cartelle. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Ottiene i report sulle operazioni di indicizzazione. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Ottiene i report sulle operazioni di ricerca. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genera testo formattato in HTML con i termini trovati evidenziati. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genera testo formattato in HTML con i termini trovati evidenziati. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Unisce l'indice specificato all'indice corrente. Nota che l'altro indice non verrà modificato. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Unisce gli indici dal repository di indice specificato all'indice corrente. Nota che gli indici nel repository non verranno modificati. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Passa l'oggetto di notifica specificato all'indice per eseguire la notifica. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Riduce il numero di segmenti dell'indice unendoli tra loro. Questa operazione migliora le prestazioni della ricerca. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Riduce il numero di segmenti dell'indice unendoli tra loro. Questa operazione migliora le prestazioni della ricerca. |
| [SaveTo](../../groupdocs.search/index/saveto)(string) | Salva l'indice in memoria su disco. Salva anche l'indice regolare in un'altra cartella. Non modifica le impostazioni di questo indice. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Cerca nell'indice. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Cerca nell'indice. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Esegue una ricerca inversa di immagini nell'indice. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Cerca nell'indice. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Cerca nell'indice. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Continua la ricerca a blocchi avviata con il metodo Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Continua la ricerca a blocchi avviata con il metodo Search. |
| [Update](../../groupdocs.search/index/update#update)() | Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge i nuovi file inseriti nelle cartelle indicizzate. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge i nuovi file inseriti nelle cartelle indicizzate. |

### Osservazioni

**Learn more**

* [Creating an index](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indexing](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Searching](https://docs.groupdocs.com/display/searchnet/Searching)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Searching in index
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
