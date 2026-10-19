---
title: "OperationProgressChanged"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando il progresso dell'operazione di indicizzazione o aggiornamento cambia."
type: docs
weight: 50
url: /it/net/groupdocs.search.events/eventhub/operationprogresschanged/
---
## EventHub.OperationProgressChanged event

Si verifica quando il progresso dell'operazione di indicizzazione o aggiornamento cambia.

```csharp
public event EventHandler<OperationProgressEventArgs> OperationProgressChanged;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Sottoscrizione all'evento
index.Events.OperationProgressChanged += (sender, args) =>
{
    Console.WriteLine("Last processed: " + args.LastDocumentPath);
    Console.WriteLine("Result: " + args.LastDocumentStatus);
    Console.WriteLine("Processed documents: " + args.TotalDocuments);
    Console.WriteLine("Progress percentage: " + args.ProgressPercentage);
};

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
```

### Vedi anche

* class [OperationProgressEventArgs](../../operationprogresseventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
