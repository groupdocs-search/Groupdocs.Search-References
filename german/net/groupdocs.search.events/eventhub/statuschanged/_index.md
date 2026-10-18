---
title: "StatusChanged"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Tritt auf, wenn sich der Indexstatus ändert."
type: docs
weight: 90
url: /de/net/groupdocs.search.events/eventhub/statuschanged/
---
## EventHub.StatusChanged event

Tritt auf, wenn sich der Indexstatus ändert.

```csharp
public event EventHandler<BaseIndexEventArgs> StatusChanged;
```

### Beispiele

Das Beispiel zeigt, wie das Ereignis verwendet wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.StatusChanged += (sender, args) =>
{
    if (args.Status != IndexStatus.InProgress)
    {
        // Eine Benachrichtigung über den Abschluss der Operation sollte hier sein
    }
};

// Setzen des Flags für die asynchrone Indizierung
IndexingOptions options = new IndexingOptions();
options.IsAsync = true;

// Asynchrone Indizierung von Dokumenten aus dem angegebenen Ordner
// Die Methode beendet sich, bevor die Operation abgeschlossen ist
index.Add(documentsFolder, options);
```

### Siehe auch

* class [BaseIndexEventArgs](../../baseindexeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
