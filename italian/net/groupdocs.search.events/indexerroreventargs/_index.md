---
title: "IndexErrorEventArgs"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta gli argomenti per l'evento di errore dell'indice."
type: docs
weight: 560
url: /it/net/groupdocs.search.events/indexerroreventargs/
---
## IndexErrorEventArgs class

Rappresenta gli argomenti per l'evento di errore dell'indice.

```csharp
public class IndexErrorEventArgs : BaseIndexEventArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ottiene la cartella dell'indice. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ottiene l'ID dell'indice. |
| [IsCritical](../../groupdocs.search.events/indexerroreventargs/iscritical) { get; } | Ottiene un flag che indica che l'errore verificato è critico e l'indice dovrebbe essere riavviato. |
| [Message](../../groupdocs.search.events/indexerroreventargs/message) { get; } | Ottiene il messaggio di errore. |
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
