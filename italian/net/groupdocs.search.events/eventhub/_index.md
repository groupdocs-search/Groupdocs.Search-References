---
title: "EventHub"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce eventi dell'indice per l'iscrizione."
type: docs
weight: 530
url: /it/net/groupdocs.search.events/eventhub/
---
## EventHub class

Fornisce eventi dell'indice per l'iscrizione.

```csharp
public class EventHub
```

## Eventi

| Nome | Descrizione |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search.events/eventhub/erroroccurred) | Si verifica quando si verifica un errore durante un'operazione di indicizzazione. |
| event [FileIndexing](../../groupdocs.search.events/eventhub/fileindexing) | Si verifica quando un documento sta per essere indicizzato. |
| event [ImagePreparing](../../groupdocs.search.events/eventhub/imagepreparing) | Si verifica quando un'immagine sta per essere preparata per l'indicizzazione. |
| event [OperationFinished](../../groupdocs.search.events/eventhub/operationfinished) | Si verifica quando un'operazione di indicizzazione è terminata. |
| event [OperationProgressChanged](../../groupdocs.search.events/eventhub/operationprogresschanged) | Si verifica quando il progresso dell'operazione di indicizzazione o aggiornamento cambia. |
| event [OptimizationProgressChanged](../../groupdocs.search.events/eventhub/optimizationprogresschanged) | Si verifica quando il progresso dell'operazione di ottimizzazione cambia. |
| event [PasswordRequired](../../groupdocs.search.events/eventhub/passwordrequired) | Si verifica quando un documento richiede una password per l'apertura. |
| event [SearchPhaseCompleted](../../groupdocs.search.events/eventhub/searchphasecompleted) | Si verifica quando la fase di ricerca è completata. |
| event [StatusChanged](../../groupdocs.search.events/eventhub/statuschanged) | Si verifica quando lo stato dell'indice cambia. |

### Osservazioni

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Esempi

L'esempio dimostra un uso tipico dell'interfaccia.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// Creazione di un indice
Index index = new Index(indexFolder);

// Sottoscrizione all'evento
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);

// Ricerca nell'indice
SearchResult result = index.Search(query);
```

### Vedi anche

* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
