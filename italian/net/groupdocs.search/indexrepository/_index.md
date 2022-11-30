---
title: IndexRepository
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta un contenitore per combinare più indici ed eseguire operazioni comuni su di essi.
type: docs
weight: 660
url: /it/net/groupdocs.search/indexrepository/
---
## IndexRepository class

Rappresenta un contenitore per combinare più indici ed eseguire operazioni comuni su di essi.

```csharp
public class IndexRepository : IDisposable
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [IndexRepository](indexrepository)() | Inizializza una nuova istanza di[`IndexRepository`](../indexrepository) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Ottiene l'hub eventi per la sottoscrizione agli eventi. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Ottiene gli indici contenuti in this[`IndexRepository`](../indexrepository) . |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Aggiunge un indice al repository dell'indice. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Apre e aggiunge un indice al repository dell'indice. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Crea un nuovo indice in memoria. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Crea un nuovo indice in memoria. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Crea un nuovo indice su disco. La cartella dell'indice verrà pulita prima della creazione dell'indice. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Crea un nuovo indice su disco. La cartella dell'indice verrà pulita prima della creazione dell'indice. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Rilascia tutte le risorse utilizzate da[`IndexRepository`](../indexrepository) . |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Cerca in tutti gli indici del repository. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Cerca in tutti gli indici del repository. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Cerca in tutti gli indici del repository. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Cerca in tutti gli indici del repository. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Aggiorna tutti gli indici nel repository. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Aggiorna tutti gli indici nel repository. |

### Osservazioni

**Scopri di più**

* [Archivio indice di ricerca](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Caricamento di un indice esistente
repository.AddToRepository(indexFolder2); // Caricamento di un altro indice esistente

SearchResult result = repository.Search(query); // Ricerca negli indici del repository
```

### Guarda anche

* spazio dei nomi [GroupDocs.Search](../../groupdocs.search)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->