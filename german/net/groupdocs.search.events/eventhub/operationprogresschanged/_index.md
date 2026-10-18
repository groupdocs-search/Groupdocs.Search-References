---
title: "OperationProgressChanged"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn sich der Fortschritt des Indexierungs- oder Aktualisierungsvorgangs ändert."
type: docs
weight: 50
url: /de/net/groupdocs.search.events/eventhub/operationprogresschanged/
---
## EventHub.OperationProgressChanged event

Tritt auf, wenn sich der Fortschritt des Indexierungs- oder Aktualisierungsvorgangs ändert.

```csharp
public event EventHandler<OperationProgressEventArgs> OperationProgressChanged;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.OperationProgressChanged += (sender, args) =>
{
    Console.WriteLine("Last processed: " + args.LastDocumentPath);
    Console.WriteLine("Result: " + args.LastDocumentStatus);
    Console.WriteLine("Processed documents: " + args.TotalDocuments);
    Console.WriteLine("Progress percentage: " + args.ProgressPercentage);
};

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
```

### Siehe auch

* class [OperationProgressEventArgs](../../operationprogresseventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
