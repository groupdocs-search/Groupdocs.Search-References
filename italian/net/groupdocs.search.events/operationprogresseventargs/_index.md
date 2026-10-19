---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta gli argomenti per l'evento di cambiamento di avanzamento dell'operazione di indicizzazione."
type: docs
weight: 580
url: /it/net/groupdocs.search.events/operationprogresseventargs/
---
## OperationProgressEventArgs class

Rappresenta gli argomenti per l'evento di cambiamento di avanzamento dell'operazione di indicizzazione.

```csharp
public class OperationProgressEventArgs : BaseIndexEventArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ottiene la cartella dell'indice. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ottiene l'ID dell'indice. |
| [LastDocumentKey](../../groupdocs.search.events/operationprogresseventargs/lastdocumentkey) { get; } | Restituisce la chiave dell'ultimo documento elaborato. |
| [LastDocumentPath](../../groupdocs.search.events/operationprogresseventargs/lastdocumentpath) { get; } | Restituisce il percorso dell'ultimo documento elaborato. |
| [LastDocumentStatus](../../groupdocs.search.events/operationprogresseventargs/lastdocumentstatus) { get; } | Restituisce lo stato dell'ultimo documento elaborato. |
| [ProcessedDocuments](../../groupdocs.search.events/operationprogresseventargs/processeddocuments) { get; } | Restituisce il numero di documenti elaborati con successo. |
| [ProgressPercentage](../../groupdocs.search.events/operationprogresseventargs/progresspercentage) { get; } | Ottiene la percentuale di avanzamento. |
| [SkippedDocuments](../../groupdocs.search.events/operationprogresseventargs/skippeddocuments) { get; } | Restituisce il numero di documenti saltati. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ottiene lo stato dell'indice. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ottiene il tempo di un evento. |
| [TotalDocuments](../../groupdocs.search.events/operationprogresseventargs/totaldocuments) { get; } | Restituisce il numero totale di documenti da elaborare. |

### Osservazioni

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Vedi anche

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
