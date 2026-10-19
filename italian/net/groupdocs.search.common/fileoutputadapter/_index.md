---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un adattatore di output che raccoglie l'output in un file."
type: docs
weight: 150
url: /it/net/groupdocs.search.common/fileoutputadapter/
---
## FileOutputAdapter class

Rappresenta un adattatore di output che raccoglie l'output in un file.

```csharp
public class FileOutputAdapter : OutputAdapter
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FileOutputAdapter](fileoutputadapter)(OutputFormat, string) | Inizializza una nuova istanza della classe [`FileOutputAdapter`](../fileoutputadapter). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FilePath](../../groupdocs.search.common/fileoutputadapter/filepath) { get; } | Ottiene un percorso file di output. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Restituisce il formato di output. |

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

FileOutputAdapter adapter = new FileOutputAdapter(@"c:\DocumentText.htm"); // Creating a file output adapter
index.GetDocumentText(documents[0], adapter); // Generating a document text into the output file
```

### Vedi anche

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
