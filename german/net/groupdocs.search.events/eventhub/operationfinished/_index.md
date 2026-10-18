---
title: "OperationFinished"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn ein Indexvorgang abgeschlossen ist."
type: docs
weight: 40
url: /de/net/groupdocs.search.events/eventhub/operationfinished/
---
## EventHub.OperationFinished event

Tritt auf, wenn ein Indexvorgang abgeschlossen ist.

```csharp
public event EventHandler<OperationFinishedEventArgs> OperationFinished;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.OperationFinished += (sender, args) =>
{
    Console.WriteLine("Operation finished: " + args.OperationType);
    Console.WriteLine("Message: " + args.Message);
    Console.WriteLine("Index folder: " + args.IndexFolder);
    Console.WriteLine("Time: " + args.Time);
};

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
```

### Siehe auch

* class [OperationFinishedEventArgs](../../operationfinishedeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
