---
title: Index
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta la classe principale per lindicizzazione dei documenti e la ricerca al loro interno.
type: docs
weight: 680
url: /it/net/groupdocs.search/index/
---
## Index class

Rappresenta la classe principale per l'indicizzazione dei documenti e la ricerca al loro interno.

```csharp
public class Index : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Index](index#constructor)() | Inizializza una nuova istanza di[`Index`](../index) classe in memoria. |
| [Index](index#constructor_1)(IndexSettings) | Inizializza una nuova istanza di[`Index`](../index) classe in memoria con particolari impostazioni di indice. |
| [Index](index#constructor_2)(string) | Inizializza una nuova istanza di[`Index`](../index) class. Crea un nuovo o apre un indice esistente su disco. |
| [Index](index#constructor_3)(string, bool) | Inizializza una nuova istanza di[`Index`](../index) class. Carica un indice esistente dal disco se*overwriteIfExists* È`falso`; crea un nuovo indice su disco altrimenti. |
| [Index](index#constructor_4)(string, IndexSettings) | Inizializza una nuova istanza di[`Index`](../index) class. Crea un nuovo indice con impostazioni particolari o apre un indice esistente su disco. |
| [Index](index#constructor_5)(string, IndexSettings, bool) | Inizializza una nuova istanza di[`Index`](../index) class. Carica un indice esistente dal disco se*overwriteIfExists* È`falso` ; crea un nuovo indice su disco con particolari impostazioni di indice altrimenti. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Dictionaries](../../groupdocs.search/index/dictionaries) { get; } | Ottiene il repository del dizionario. |
| [Events](../../groupdocs.search/index/events) { get; } | Ottiene l'hub eventi per la sottoscrizione agli eventi. |
| [IndexInfo](../../groupdocs.search/index/indexinfo) { get; } | Ottiene le informazioni di base sull'indice. |
| [IndexSettings](../../groupdocs.search/index/indexsettings) { get; } | Ottiene le impostazioni dell'indice. |
| [Repository](../../groupdocs.search/index/repository) { get; } | Ottiene l'oggetto repository indice se l'indice è contenuto in esso. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../groupdocs.search/index/add#add_2)(string) | Esegue un'operazione di indicizzazione. Aggiunge un file o una cartella in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [Add](../../groupdocs.search/index/add#add_4)(string[]) | Esegue un'operazione di indicizzazione. Aggiunge file o cartelle in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [Add](../../groupdocs.search/index/add#add)(Document[], IndexingOptions) | Esegue un'operazione di indicizzazione. Aggiunge documenti da file system, flusso o struttura. |
| [Add](../../groupdocs.search/index/add#add_1)(ExtractedData[], IndexingOptions) | Esegue l'operazione di indicizzazione. Aggiunge i dati estratti all'indice. |
| [Add](../../groupdocs.search/index/add#add_3)(string, IndexingOptions) | Esegue un'operazione di indicizzazione. Aggiunge un file o una cartella in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [Add](../../groupdocs.search/index/add#add_5)(string[], IndexingOptions) | Esegue un'operazione di indicizzazione. Aggiunge file o cartelle in base a un percorso assoluto o relativo. I documenti di tutte le sottocartelle verranno indicizzati. |
| [ChangeAttributes](../../groupdocs.search/index/changeattributes)(AttributeChangeBatch) | Applica il batch specificato di modifiche agli attributi ai documenti indicizzati senza reindicizzare durante l'operazione di aggiornamento. |
| [Delete](../../groupdocs.search/index/delete#delete_1)(string[], UpdateOptions) | Elimina i file o le cartelle indicizzati dall'indice. Quindi aggiorna l'indice senza percorsi eliminati. Nota che un singolo documento non può essere eliminato dall'indice se è stato aggiunto all'indice come parte di una cartella. |
| [Delete](../../groupdocs.search/index/delete#delete)(UpdateOptions, string[]) | Elimina i documenti indicizzati da flussi o strutture. Quindi aggiorna l'indice senza documenti eliminati. |
| [Dispose](../../groupdocs.search/index/dispose)() | Rilascia tutte le risorse utilizzate da[`Index`](../index) . |
| [GetAttributes](../../groupdocs.search/index/getattributes)(string) | Recupera tutti gli attributi associati al documento indicizzato specificato. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext)(DocumentInfo, OutputAdapter) | Genera testo in formato HTML per il documento indicizzato e lo trasferisce tramite l'adattatore di output. |
| [GetDocumentText](../../groupdocs.search/index/getdocumenttext#getdocumenttext_1)(DocumentInfo, OutputAdapter, TextOptions) | Genera testo in formato HTML per il documento indicizzato e lo trasferisce tramite l'adattatore di output. |
| [GetIndexedDocumentItems](../../groupdocs.search/index/getindexeddocumentitems)(DocumentInfo) | Ottiene un array di elementi nidificati del documento specificato (per documenti contenitore come ZIP, OST, PST). |
| [GetIndexedDocuments](../../groupdocs.search/index/getindexeddocuments)() | Ottiene un array di tutti i documenti indicizzati. |
| [GetIndexedPaths](../../groupdocs.search/index/getindexedpaths)() | Ottiene un array di percorsi indicizzati: documenti o cartelle. |
| [GetIndexingReports](../../groupdocs.search/index/getindexingreports)() | Ottiene i report sulle operazioni di indicizzazione. |
| [GetSearchReports](../../groupdocs.search/index/getsearchreports)() | Ottiene i report sulle operazioni di ricerca. |
| [Highlight](../../groupdocs.search/index/highlight#highlight)(FoundDocument, Highlighter) | Genera testo in formato HTML con i termini trovati evidenziati. |
| [Highlight](../../groupdocs.search/index/highlight#highlight_1)(FoundDocument, Highlighter, HighlightOptions) | Genera testo in formato HTML con i termini trovati evidenziati. |
| [Merge](../../groupdocs.search/index/merge#merge)(Index, MergeOptions) | Unisce l'indice specificato nell'indice corrente. Si noti che l'altro indice non verrà modificato. |
| [Merge](../../groupdocs.search/index/merge#merge_1)(IndexRepository, MergeOptions) | Unisce gli indici dal repository di indici specificato nell'indice corrente. Si noti che gli indici nel repository non verranno modificati. |
| [Notify](../../groupdocs.search/index/notify)(Notification) | Passa l'oggetto di notifica specificato all'indice per eseguire la notifica. |
| [Optimize](../../groupdocs.search/index/optimize#optimize)() | Riduce al minimo il numero di segmenti di indice unendoli uno con l'altro. Questa operazione migliora le prestazioni della ricerca. |
| [Optimize](../../groupdocs.search/index/optimize#optimize_1)(MergeOptions) | Riduce al minimo il numero di segmenti di indice unendoli uno con l'altro. Questa operazione migliora le prestazioni della ricerca. |
| [Search](../../groupdocs.search/index/search#search_1)(SearchQuery) | Ricerche nell'indice. |
| [Search](../../groupdocs.search/index/search#search_3)(string) | Ricerche nell'indice. |
| [Search](../../groupdocs.search/index/search#search)(SearchImage, ImageSearchOptions) | Esegue una ricerca inversa delle immagini nell'indice. |
| [Search](../../groupdocs.search/index/search#search_2)(SearchQuery, SearchOptions) | Ricerche nell'indice. |
| [Search](../../groupdocs.search/index/search#search_4)(string, SearchOptions) | Ricerche nell'indice. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext)(ChunkSearchToken) | Continua la ricerca in chunk avviata con il metodo Search. |
| [SearchNext](../../groupdocs.search/index/searchnext#searchnext_1)(ChunkSearchToken, Cancellation) | Continua la ricerca in chunk avviata con il metodo Search. |
| [Update](../../groupdocs.search/index/update#update)() | Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge nuovi file che sono stati aggiunti alle cartelle indicizzate. |
| [Update](../../groupdocs.search/index/update#update_1)(UpdateOptions) | Reindicizza i documenti che sono stati modificati o eliminati dall'ultimo aggiornamento. Aggiunge nuovi file che sono stati aggiunti alle cartelle indicizzate. |

### Osservazioni

**Saperne di più**

* [Creazione di un indice](https://docs.groupdocs.com/display/searchnet/Creating+an+index)
* [Indicizzazione](https://docs.groupdocs.com/display/searchnet/Indexing)
* [Ricerca](https://docs.groupdocs.com/display/searchnet/Searching)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

Index index = new Index(indexFolder); // Creazione dell'indice nella cartella specificata
index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchResult result = index.Search(query); // Ricerca nell'indice
```

### Guarda anche

* spazio dei nomi [GroupDocs.Search](../../groupdocs.search)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
