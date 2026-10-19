---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta gli argomenti per l'evento che si verifica quando un documento protetto da password viene indicizzato."
type: docs
weight: 610
url: /it/net/groupdocs.search.events/passwordrequiredeventargs/
---
## PasswordRequiredEventArgs class

Rappresenta gli argomenti per l'evento che si verifica quando un documento protetto da password viene indicizzato.

```csharp
public class PasswordRequiredEventArgs : BaseIndexEventArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentFullPath](../../groupdocs.search.events/passwordrequiredeventargs/documentfullpath) { get; } | Ottiene il percorso completo del documento. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ottiene la cartella dell'indice. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ottiene l'ID dell'indice. |
| [Password](../../groupdocs.search.events/passwordrequiredeventargs/password) { get; set; } | Restituisce o imposta la password per aprire il documento. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ottiene lo stato dell'indice. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ottiene il tempo di un evento. |

### Osservazioni

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Vedi anche

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
