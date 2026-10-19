---
title: "GetIndexedDocumentItems"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Restituisce un array di elementi nidificati del documento specificato per documenti contenitore come ZIP, OST, PST."
type: docs
weight: 160
url: /it/net/groupdocs.search/index/getindexeddocumentitems/
---
## Index.GetIndexedDocumentItems method

Ottiene un array di elementi annidati del documento specificato (per documenti contenitori come ZIP, OST, PST).

```csharp
public DocumentInfo[] GetIndexedDocumentItems(DocumentInfo documentInfo)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| documentInfo | DocumentInfo | Le informazioni del documento. |

### Valore di ritorno

Un array di elementi del documento.

### Esempi

L'esempio dimostra come ottenere un elenco di elementi di un documento indicizzato da un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
 
// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);
 
// Indicizzazione dei documenti dalla cartella specificata
index.Add(documentsFolder);
 
// Ottenere l'elenco dei documenti indicizzati
DocumentInfo[] documents = index.GetIndexedDocuments();
for (int i = 0; i < documents.Length; i++)
{
    DocumentInfo document = documents[i];
    Console.WriteLine(document.FilePath);
    DocumentInfo[] items = index.GetIndexedDocumentItems(document); // Getting list of document items
    for (int j = 0; j < items.Length; j++)
    {
        DocumentInfo item = items[j];
        Console.WriteLine("\t" + item.InnerPath);
    }
}
```

### Vedi anche

* class [DocumentInfo](../../../groupdocs.search.results/documentinfo)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
