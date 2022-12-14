---
title: GetDocumentText
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Genera testo in formato HTML per il documento indicizzato e lo trasferisce tramite ladattatore di output.
type: docs
weight: 120
url: /it/net/groupdocs.search/index/getdocumenttext/
---
## GetDocumentText(DocumentInfo, OutputAdapter) {#getdocumenttext}

Genera testo in formato HTML per il documento indicizzato e lo trasferisce tramite l'adattatore di output.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documentInfo | DocumentInfo | Le informazioni sul documento indicizzato. |
| adapter | OutputAdapter | L'adattatore di uscita. |

### Esempi

L'esempio mostra come ottenere il testo di un documento indicizzato da un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
 
// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
 
// Ottenere l'elenco dei documenti indicizzati
DocumentInfo[] documents = index.GetIndexedDocuments();
 
// Recupero del testo di un documento
if (documents.Length > 0)
{
    FileOutputAdapter outputAdapter = new FileOutputAdapter(@"C:\Text.html");
    index.GetDocumentText(documents[0], outputAdapter);
}
```

### Guarda anche

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## GetDocumentText(DocumentInfo, OutputAdapter, TextOptions) {#getdocumenttext_1}

Genera testo in formato HTML per il documento indicizzato e lo trasferisce tramite l'adattatore di output.

```csharp
public void GetDocumentText(DocumentInfo documentInfo, OutputAdapter adapter, TextOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| documentInfo | DocumentInfo | Le informazioni sul documento indicizzato. |
| adapter | OutputAdapter | L'adattatore di uscita. |
| options | TextOptions | Le opzioni di recupero del testo. |

### Guarda anche

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [OutputAdapter](../../../groupdocs.search.common/outputadapter)
* class [TextOptions](../../../groupdocs.search.options/textoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
