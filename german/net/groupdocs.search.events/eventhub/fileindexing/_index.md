---
title: "FileIndexing"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn ein Dokument indiziert werden soll."
type: docs
weight: 20
url: /de/net/groupdocs.search.events/eventhub/fileindexing/
---
## EventHub.FileIndexing event

Tritt auf, wenn ein Dokument indiziert werden soll.

```csharp
public event EventHandler<FileIndexingEventArgs> FileIndexing;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.FileIndexing += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("Protected.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.AdditionalFields = new DocumentField[]
        {
            new DocumentField("Tags", "Protected")
        };
    }
    if (!args.DocumentFullPath.ToLowerInvariant().Contains("important"))
    {
        args.SkipIndexing = true;
    }
};

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);
```

### Siehe auch

* class [FileIndexingEventArgs](../../fileindexingeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
