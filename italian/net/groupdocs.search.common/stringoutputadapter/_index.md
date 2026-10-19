---
title: "StringOutputAdapter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output come stringa."
type: docs
weight: 320
url: /it/net/groupdocs.search.common/stringoutputadapter/
---
## StringOutputAdapter class

Rappresenta un adattatore di output che raccoglie l'output come stringa.

```csharp
public class StringOutputAdapter : OutputAdapter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [StringOutputAdapter](stringoutputadapter)(OutputFormat) | Inizializza una nuova istanza della classe [`StringOutputAdapter`](../stringoutputadapter). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Restituisce il formato di output. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetResult](../../groupdocs.search.common/stringoutputadapter/getresult)() | Ottiene la stringa risultante. |

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

StringOutputAdapter adapter = new StringOutputAdapter(OutputFormat.Html); // Creating a string output adapter
index.GetDocumentText(documents[0], adapter); // Generating a document text into the adapter
String result = adapter.GetResult(); // Getting a result
```

### Vedi anche

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
