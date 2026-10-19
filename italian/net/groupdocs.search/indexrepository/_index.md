---
title: "IndexRepository"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un contenitore per combinare più indici ed eseguire operazioni comuni su di essi."
type: docs
weight: 710
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
| [IndexRepository](indexrepository)() | Inizializza una nuova istanza della classe [`IndexRepository`](../indexrepository). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Events](../../groupdocs.search/indexrepository/events) { get; } | Ottiene il hub degli eventi per l'iscrizione agli eventi. |
| [Indexes](../../groupdocs.search/indexrepository/indexes) { get; } | Ottiene gli indici contenuti in questo [`IndexRepository`](../indexrepository). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository)(Index) | Aggiunge un indice al repository degli indici. |
| [AddToRepository](../../groupdocs.search/indexrepository/addtorepository#addtorepository_1)(string) | Apre e aggiunge un indice al repository degli indici. |
| [Create](../../groupdocs.search/indexrepository/create#create)() | Crea un nuovo indice in memoria. |
| [Create](../../groupdocs.search/indexrepository/create#create_1)(IndexSettings) | Crea un nuovo indice in memoria. |
| [Create](../../groupdocs.search/indexrepository/create#create_2)(string) | Crea un nuovo indice su disco. La cartella dell'indice verrà pulita prima della creazione dell'indice. |
| [Create](../../groupdocs.search/indexrepository/create#create_3)(string, IndexSettings) | Crea un nuovo indice su disco. La cartella dell'indice verrà pulita prima della creazione dell'indice. |
| [Dispose](../../groupdocs.search/indexrepository/dispose)() | Rilascia tutte le risorse utilizzate da [`IndexRepository`](../indexrepository). |
| [Search](../../groupdocs.search/indexrepository/search#search)(SearchQuery) | Cerca in tutti gli indici del repository. |
| [Search](../../groupdocs.search/indexrepository/search#search_2)(string) | Cerca in tutti gli indici del repository. |
| [Search](../../groupdocs.search/indexrepository/search#search_1)(SearchQuery, SearchOptions) | Cerca in tutti gli indici del repository. |
| [Search](../../groupdocs.search/indexrepository/search#search_3)(string, SearchOptions) | Cerca in tutti gli indici del repository. |
| [Update](../../groupdocs.search/indexrepository/update#update)() | Aggiorna tutti gli indici nel repository. |
| [Update](../../groupdocs.search/indexrepository/update#update_1)(UpdateOptions) | Aggiorna tutti gli indici nel repository. |

### Osservazioni

**Learn more**

* [Search index repository](https://docs.groupdocs.com/display/searchnet/Search+index+repository)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder1 = @"c:\MyIndex\";
string indexFolder2 = @"c:\MyIndex\";
string query = "Einstein";

IndexRepository repository = new IndexRepository();
repository.AddToRepository(indexFolder1); // Loading an existing index
repository.AddToRepository(indexFolder2); // Loading another existing index

SearchResult result = repository.Search(query); // Searching in indexes of the repository
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
