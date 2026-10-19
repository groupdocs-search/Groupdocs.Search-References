---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output in uno stream."
type: docs
weight: 310
url: /it/net/groupdocs.search.common/streamoutputadapter/
---
## StreamOutputAdapter class

Rappresenta un adattatore di output che raccoglie l'output in uno stream.

```csharp
public class StreamOutputAdapter : OutputAdapter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [StreamOutputAdapter](streamoutputadapter)(OutputFormat, Stream) | Inizializza una nuova istanza della classe [`StreamOutputAdapter`](../streamoutputadapter). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Restituisce il formato di output. |
| [Stream](../../groupdocs.search.common/streamoutputadapter/stream) { get; } | Restituisce un flusso di output. |

### Osservazioni

**Learn more**

* [Output adapters](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating an index in the specified folder

index.Add(documentsFolder); // Indexing documents from the specified folder

DocumentInfo[] documents = index.GetIndexedDocuments(); // Getting information on indexed documents

using (Stream stream = new MemoryStream()) // Creating a stream
{
    StreamOutputAdapter adapter = new StreamOutputAdapter(stream); // Creating a stream output adapter
    index.GetDocumentText(documents[0], adapter); // Generating a document text into the stream
}
```

### Vedi anche

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
