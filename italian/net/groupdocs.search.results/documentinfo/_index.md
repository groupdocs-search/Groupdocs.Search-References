---
title: "DocumentInfo"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un descrittore per un documento indicizzato."
type: docs
weight: 1230
url: /it/net/groupdocs.search.results/documentinfo/
---
## DocumentInfo class

Rappresenta un descrittore per un documento indicizzato.

```csharp
public class DocumentInfo
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DocumentSourceKind](../../groupdocs.search.results/documentinfo/documentsourcekind) { get; } | Restituisce il tipo di origine del documento. |
| [FilePath](../../groupdocs.search.results/documentinfo/filepath) { get; } | Ottiene il percorso del file indicizzato da file o la chiave del documento indicizzato da stream o struttura. |
| [FileType](../../groupdocs.search.results/documentinfo/filetype) { get; } | Ottiene il tipo di file. |
| [FormatFamily](../../groupdocs.search.results/documentinfo/formatfamily) { get; } | Ottiene la famiglia del formato del documento. |
| [IndexedWithError](../../groupdocs.search.results/documentinfo/indexedwitherror) { get; } | Ottiene l'indicatore di errore di indicizzazione. |
| [InnerPath](../../groupdocs.search.results/documentinfo/innerpath) { get; } | Ottiene il percorso interno per l'elemento del documento contenitore. |
| [InnerPathParts](../../groupdocs.search.results/documentinfo/innerpathparts) { get; } | Ottiene le parti del percorso interno per l'elemento del documento contenitore. |
| [ModificationTime](../../groupdocs.search.results/documentinfo/modificationtime) { get; } | Ottiene l'ora di modifica. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [Deserialize](../../groupdocs.search.results/documentinfo/deserialize)(byte[]) | Deserializza un'istanza da un array di byte. |
| [Serialize](../../groupdocs.search.results/documentinfo/serialize)() | Serializza l'istanza corrente in un array di byte. |
| override [ToString](../../groupdocs.search.results/documentinfo/tostring)() | Restituisce una stringa che rappresenta l'attuale [`DocumentInfo`](../documentinfo). |

### Osservazioni

**Learn more**

* [Search results](https://docs.groupdocs.com/display/searchnet/Search+results)
* [Getting indexed documents](https://docs.groupdocs.com/display/searchnet/Getting+indexed+documents)

### Vedi anche

* namespace [GroupDocs.Search.Results](../../groupdocs.search.results)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
