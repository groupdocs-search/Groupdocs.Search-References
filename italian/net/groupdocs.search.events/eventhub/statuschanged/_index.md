---
title: "StatusChanged"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando lo stato dell'indice cambia."
type: docs
weight: 90
url: /it/net/groupdocs.search.events/eventhub/statuschanged/
---
## EventHub.StatusChanged event

Si verifica quando lo stato dell'indice cambia.

```csharp
public event EventHandler<BaseIndexEventArgs> StatusChanged;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Sottoscrizione all'evento
index.Events.StatusChanged += (sender, args) =>
{
    if (args.Status != IndexStatus.InProgress)
    {
        // Una notifica del completamento dell'operazione dovrebbe essere qui
    }
};

// Impostazione del flag per l'indicizzazione asincrona
IndexingOptions options = new IndexingOptions();
options.IsAsync = true;

// Indicizzazione asincrona dei documenti dalla cartella specificata
// Il metodo termina prima che l'operazione sia completata
index.Add(documentsFolder, options);
```

### Vedi anche

* class [BaseIndexEventArgs](../../baseindexeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
