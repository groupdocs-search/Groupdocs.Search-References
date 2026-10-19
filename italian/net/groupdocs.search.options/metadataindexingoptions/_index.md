---
title: "MetadataIndexingOptions"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce opzioni per l'indicizzazione dei campi dei metadati."
type: docs
weight: 1020
url: /it/net/groupdocs.search.options/metadataindexingoptions/
---
## MetadataIndexingOptions class

Fornisce opzioni per l'indicizzazione dei campi dei metadati.

```csharp
public class MetadataIndexingOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DefaultFieldName](../../groupdocs.search.options/metadataindexingoptions/defaultfieldname) { get; set; } | Ottiene o imposta il nome campo predefinito usato per indicizzare i nomi campo vuoti. Il valore predefinito è `"unknown"`. |
| [IndexingEmptyNames](../../groupdocs.search.options/metadataindexingoptions/indexingemptynames) { get; set; } | Ottiene o imposta un valore che indica se indicizzare i nomi campo vuoti o meno. Il valore predefinito è `true`. |
| [IndexingEmptyValues](../../groupdocs.search.options/metadataindexingoptions/indexingemptyvalues) { get; set; } | Ottiene o imposta un valore che indica se indicizzare i valori campo vuoti o meno. Il valore predefinito è `true`. |
| [MaxBytesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxbytestoindexfield) { get; set; } | Ottiene o imposta il numero massimo di valori in un array di tipo byte per indicizzare il campo. Il valore predefinito è `int.MaxValue`. |
| [MaxDoublesToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxdoublestoindexfield) { get; set; } | Ottiene o imposta il numero massimo di valori in un array di tipo double per indicizzare il campo. Il valore predefinito è `int.MaxValue`. |
| [MaxIntsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxintstoindexfield) { get; set; } | Ottiene o imposta il numero massimo di valori in un array di tipo int per indicizzare il campo. Il valore predefinito è `int.MaxValue`. |
| [MaxLongsToIndexField](../../groupdocs.search.options/metadataindexingoptions/maxlongstoindexfield) { get; set; } | Ottiene o imposta il numero massimo di valori in un array di tipo long per indicizzare il campo. Il valore predefinito è `int.MaxValue`. |
| [SeparatorBetweenValues](../../groupdocs.search.options/metadataindexingoptions/separatorbetweenvalues) { get; set; } | Ottiene o imposta il separatore tra i valori in un campo di tipo array. Il valore predefinito è lo spazio. |
| [SeparatorInCompoundName](../../groupdocs.search.options/metadataindexingoptions/separatorincompoundname) { get; set; } | Ottiene o imposta il separatore nel nome composto di un campo. Il valore predefinito è `\".\"`. |

### Osservazioni

**Learn more**

* [Indexing options](https://docs.groupdocs.com/display/searchnet/Indexing+options)
* MetadataIndexingOptions are used when retrieving document text from an index: [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)
* MetadataIndexingOptions are used when highlighting search results: [Highlighting search results](https://docs.groupdocs.com/display/searchnet/Highlighting+search+results)

### Vedi anche

* namespace [GroupDocs.Search.Options](../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
