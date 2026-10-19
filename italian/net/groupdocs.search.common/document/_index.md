---
title: "Documento"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta la classe base per i documenti aggiunti a un indice da flusso o struttura del file system. Contiene metodi statici per creare documenti da diversi tipi di sorgenti."
type: docs
weight: 50
url: /it/net/groupdocs.search.common/document/
---
## Document class

Rappresenta la classe base per i documenti aggiunti a un indice dal file system, dallo stream o dalla struttura. Contiene metodi statici per creare documenti da diversi tipi di sorgenti.

```csharp
public abstract class Document
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [AdditionalFields](../../groupdocs.search.common/document/additionalfields) { get; set; } | Ottiene o imposta i campi aggiuntivi per il documento. |
| virtual [Attributes](../../groupdocs.search.common/document/attributes) { get; set; } | Ottiene o imposta gli attributi del documento. |
| abstract [DocumentKey](../../groupdocs.search.common/document/documentkey) { get; } | Restituisce la chiave del documento utilizzata per identificare il documento all'interno di un indice. |
| abstract [DocumentSourceKind](../../groupdocs.search.common/document/documentsourcekind) { get; } | Restituisce il tipo di origine del documento. |
| abstract [Extension](../../groupdocs.search.common/document/extension) { get; } | Restituisce l'estensione utilizzata per questo tipo di documento. |
| abstract [IsLazy](../../groupdocs.search.common/document/islazy) { get; } | Restituisce un valore che indica se il documento è caricato su richiesta o meno. |
| abstract [ModificationDate](../../groupdocs.search.common/document/modificationdate) { get; } | Restituisce la data dell'ultima modifica del documento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateFromFile](../../groupdocs.search.common/document/createfromfile)(string) | Crea un documento da un file. |
| static [CreateFromStream](../../groupdocs.search.common/document/createfromstream)(string, DateTime, string, Stream) | Crea un documento da un flusso. |
| static [CreateFromStructure](../../groupdocs.search.common/document/createfromstructure)(string, DateTime, DocumentField[]) | Crea un documento da una struttura che è un array di campi di testo. |
| static [CreateLazy](../../groupdocs.search.common/document/createlazy)(DocumentSourceKind, string, IDocumentLoader) | Crea un documento caricato pigramente. |
| override [ToString](../../groupdocs.search.common/document/tostring)() | Restituisce una String che rappresenta il corrente [`Document`](../document). |

### Osservazioni

**Learn more**

* [Indexing from different sources](https://docs.groupdocs.com/search/net/indexing-from-different-sources/)

### Vedi anche

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
