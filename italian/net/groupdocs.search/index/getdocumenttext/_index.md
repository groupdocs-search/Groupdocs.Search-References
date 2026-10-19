---
title: "GetDocumentText"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output."
type: docs
weight: 140
url: /it/net/groupdocs.search/index/getdocumenttext/
---
## GetDocumentText(DocumentInfo, OutputAdapter) {#getdocumenttext}

Genera il testo di un documento indicizzato e lo passa attraverso un adattatore di output.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentInfo | DocumentInfo | Le informazioni del documento indicizzato. |
| adattatore | OutputAdapter | L'adattatore di output. |

### Esempi

L'esempio dimostra come ottenere il testo di un documento indicizzato da un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
 
// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
 
// Ottenere l'elenco dei documenti indicizzati
DocumentInfo[] documents = index.GetIndexedDocuments();
 
// Ottenere il testo di un documento
if (documents.Length > 0)
{
    FileOutputAdapter outputAdapter = new FileOutputAdapter(@"C:\Text.html");
    index.GetDocumentText(documents[0], outputAdapter);
}
```

### Vedi anche

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## GetDocumentText(DocumentInfo, OutputAdapter, TextOptions) {#getdocumenttext_1}

Genera testo formattato in HTML per il documento indicizzato e lo trasferisce attraverso l'adattatore di output.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentInfo | DocumentInfo | Le informazioni del documento indicizzato. |
| adattatore | OutputAdapter | L'adattatore di output. |
| opzioni | TextOptions | Le opzioni di recupero del testo. |

### Vedi anche

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [TextOptions](../../../groupdocs.search.options/textoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
