---
title: "ErrorOccurred"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando si verifica un errore durante un'operazione di indicizzazione."
type: docs
weight: 10
url: /it/net/groupdocs.search.events/eventhub/erroroccurred/
---
## EventHub.ErrorOccurred event

Si verifica quando si verifica un errore durante un'operazione di indicizzazione.

```csharp
public event EventHandler<IndexErrorEventArgs> ErrorOccurred;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

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

* class [IndexErrorEventArgs](../../indexerroreventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
