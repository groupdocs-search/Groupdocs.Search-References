---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta gli argomenti per l'evento di avvio dell'indicizzazione di un documento."
type: docs
weight: 540
url: /it/net/groupdocs.search.events/fileindexingeventargs/
---
## FileIndexingEventArgs class

Rappresenta gli argomenti per l'evento di avvio dell'indicizzazione di un documento.

```csharp
public class FileIndexingEventArgs : BaseIndexEventArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.events/fileindexingeventargs/additionalfields) { get; set; } | Ottiene o imposta i campi aggiuntivi per il documento. |
| [Attributes](../../groupdocs.search.events/fileindexingeventargs/attributes) { get; set; } | Ottiene o imposta gli attributi del documento. |
| [CustomExtractor](../../groupdocs.search.events/fileindexingeventargs/customextractor) { get; set; } | Ottiene o imposta l'estrattore di testo personalizzato. |
| [Document](../../groupdocs.search.events/fileindexingeventargs/document) { get; } | Ottiene il documento. |
| [DocumentFullPath](../../groupdocs.search.events/fileindexingeventargs/documentfullpath) { get; } | Ottiene il percorso completo del documento. |
| [DocumentKey](../../groupdocs.search.events/fileindexingeventargs/documentkey) { get; } | Ottiene la chiave del documento. |
| [Encoding](../../groupdocs.search.events/fileindexingeventargs/encoding) { get; set; } | Ottiene o imposta la codifica del documento. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ottiene la cartella dell'indice. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ottiene l'ID dell'indice. |
| [SkipIndexing](../../groupdocs.search.events/fileindexingeventargs/skipindexing) { get; set; } | Ottiene o imposta un valore che indica che l'indicizzazione del documento dovrebbe essere saltata. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ottiene lo stato dell'indice. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ottiene il tempo di un evento. |
| [WordSplitter](../../groupdocs.search.events/fileindexingeventargs/wordsplitter) { get; set; } | Ottiene o imposta il separatore di parole personalizzato usato per dividere il testo in parole. |

### Osservazioni

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Vedi anche

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
