---
title: "Add"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Esegue l'operazione di indicizzazione. È supportata l'indicizzazione solo da flusso e struttura."
type: docs
weight: 20
url: /it/net/groupdocs.search.scaling/indexer/add/
---
## Add(IList&lt;Document&gt;, IList&lt;string&gt;, IndexingOptions) {#add}

Esegue l'operazione di indicizzazione. È supportata l'indicizzazione solo da flusso e struttura.

```csharp
public void Add(IList<Document> documents, IList<string> passwords, IndexingOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documenti | IList`1 | I documenti dallo stream o dalla struttura. |
| password | IList`1 | Le password del documento. |
| opzioni | IndexingOptions | Le opzioni di aggiunta. |

### Vedi anche

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

---

## Add(IList&lt;ExtractedData&gt;, IndexingOptions) {#add_1}

Esegue l'operazione di indicizzazione. Aggiunge i dati estratti alla rete di ricerca.

```csharp
public void Add(IList<ExtractedData> data, IndexingOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| dati | IList`1 | I dati estratti. |
| opzioni | IndexingOptions | Le opzioni di indicizzazione. |

### Vedi anche

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Indexer](../../indexer)
* namespace [GroupDocs.Search.Scaling](../../../groupdocs.search.scaling)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
