---
title: "FileIndexing"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando un documento sta per essere indicizzato."
type: docs
weight: 20
url: /it/net/groupdocs.search.events/eventhub/fileindexing/
---
## EventHub.FileIndexing event

Si verifica quando un documento sta per essere indicizzato.

```csharp
public event EventHandler<FileIndexingEventArgs> FileIndexing;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Sottoscrizione all'evento
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

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
```

### Vedi anche

* class [FileIndexingEventArgs](../../fileindexingeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
