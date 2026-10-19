---
title: "OperationFinished"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando un'operazione di indicizzazione è terminata."
type: docs
weight: 40
url: /it/net/groupdocs.search.events/eventhub/operationfinished/
---
## EventHub.OperationFinished event

Si verifica quando un'operazione di indicizzazione è terminata.

```csharp
public event EventHandler<OperationFinishedEventArgs> OperationFinished;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Sottoscrizione all'evento
index.Events.OperationFinished += (sender, args) =>
{
    Console.WriteLine("Operation finished: " + args.OperationType);
    Console.WriteLine("Message: " + args.Message);
    Console.WriteLine("Index folder: " + args.IndexFolder);
    Console.WriteLine("Time: " + args.Time);
};

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
```

### Vedi anche

* class [OperationFinishedEventArgs](../../operationfinishedeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
