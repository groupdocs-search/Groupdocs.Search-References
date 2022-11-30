---
title: Document
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta la classe base per i documenti aggiunti a un indice da file system flusso o struttura. Contiene metodi statici per la creazione di documenti da diversi tipi di origini.
type: docs
weight: 50
url: /it/net/groupdocs.search.common/document/
---
## Document class

Rappresenta la classe base per i documenti aggiunti a un indice da file system, flusso o struttura. Contiene metodi statici per la creazione di documenti da diversi tipi di origini.

```csharp
public abstract class Document
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [AdditionalFields](../../groupdocs.search.common/document/additionalfields) { get; set; } | Ottiene o imposta i campi aggiuntivi per il documento. |
| virtual [Attributes](../../groupdocs.search.common/document/attributes) { get; set; } | Ottiene o imposta gli attributi del documento. |
| abstract [DocumentKey](../../groupdocs.search.common/document/documentkey) { get; } | Ottiene la chiave del documento utilizzata per identificare il documento all'interno di un indice. |
| abstract [DocumentSourceKind](../../groupdocs.search.common/document/documentsourcekind) { get; } | Ottiene il tipo di origine del documento. |
| abstract [Extension](../../groupdocs.search.common/document/extension) { get; } | Ottiene l'estensione utilizzata per questo tipo di documento. |
| abstract [IsLazy](../../groupdocs.search.common/document/islazy) { get; } | Ottiene un valore che indica se il documento viene caricato come necessario o meno. |
| abstract [ModificationDate](../../groupdocs.search.common/document/modificationdate) { get; } | Ottiene la data dell'ultima modifica del documento. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateFromFile](../../groupdocs.search.common/document/createfromfile)(string) | Crea un documento da un file. |
| static [CreateFromStream](../../groupdocs.search.common/document/createfromstream)(string, DateTime, string, Stream) | Crea un documento da un flusso. |
| static [CreateFromStructure](../../groupdocs.search.common/document/createfromstructure)(string, DateTime, DocumentField[]) | Crea un documento da una struttura che è un array di campi di testo. |
| static [CreateLazy](../../groupdocs.search.common/document/createlazy)(DocumentSourceKind, string, IDocumentLoader) | Crea un documento a caricamento lento. |
| override [ToString](../../groupdocs.search.common/document/tostring)() | Restituisce aString che rappresenta la corrente[`Document`](../document) . |

### Osservazioni

**Scopri di più**

* [Indicizzazione da diverse fonti](https://docs.groupdocs.com/search/net/indexing-from-different-sources/)

### Guarda anche

* spazio dei nomi [GroupDocs.Search.Common](../../groupdocs.search.common)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->