---
title: "ErrorOccurred"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn ein Fehler während einer Indexoperation auftritt."
type: docs
weight: 10
url: /de/net/groupdocs.search.events/eventhub/erroroccurred/
---
## EventHub.ErrorOccurred event

Tritt auf, wenn ein Fehler während einer Indexoperation auftritt.

```csharp
public event EventHandler<IndexErrorEventArgs> ErrorOccurred;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);

// Durchsuchen des Index
SearchResult result = index.Search(query);
```

### Siehe auch

* class [IndexErrorEventArgs](../../indexerroreventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
