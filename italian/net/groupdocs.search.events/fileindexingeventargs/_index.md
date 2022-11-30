---
title: FileIndexingEventArgs
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta gli argomenti per levento di avvio dellindicizzazione di un documento.
type: docs
weight: 510
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
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ottiene l'ID indice. |
| [SkipIndexing](../../groupdocs.search.events/fileindexingeventargs/skipindexing) { get; set; } | Ottiene o imposta un valore che indica che l'indicizzazione del documento deve essere saltata. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ottiene lo stato dell'indice. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ottiene l'ora di un evento. |

### Osservazioni

**Scopri di più**

* [Cerca eventi indice](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Guarda anche

* class [BaseIndexEventArgs](../baseindexeventargs)
* spazio dei nomi [GroupDocs.Search.Events](../../groupdocs.search.events)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->