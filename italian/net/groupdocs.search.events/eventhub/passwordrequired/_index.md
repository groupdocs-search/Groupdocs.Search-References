---
title: "PasswordRequired"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Si verifica quando un documento richiede una password per l'apertura."
type: docs
weight: 70
url: /it/net/groupdocs.search.events/eventhub/passwordrequired/
---
## EventHub.PasswordRequired event

Si verifica quando un documento richiede una password per l'apertura.

```csharp
public event EventHandler<PasswordRequiredEventArgs> PasswordRequired;
```

### Esempi

L'esempio dimostra come utilizzare l'evento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un indice
Index index = new Index(indexFolder);

// Sottoscrizione all'evento
index.Events.PasswordRequired += (sender, args) =>
{
    if (args.DocumentFullPath.EndsWith("ProtectedDocument.pdf", StringComparison.InvariantCultureIgnoreCase))
    {
        args.Password = "123456";
    }
};

// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
```

### Vedi anche

* class [PasswordRequiredEventArgs](../../passwordrequiredeventargs)
* class [EventHub](../../eventhub)
* namespace [GroupDocs.Search.Events](../../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
