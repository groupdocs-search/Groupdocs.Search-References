---
title: "StreamOutputAdapter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un adaptateur de sortie qui collecte la sortie dans un flux."
type: docs
weight: 310
url: /fr/net/groupdocs.search.common/streamoutputadapter/
---
## StreamOutputAdapter class

Représente un adaptateur de sortie qui collecte la sortie dans un flux.

```csharp
public class StreamOutputAdapter : OutputAdapter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [StreamOutputAdapter](streamoutputadapter)(OutputFormat, Stream) | Initialise une nouvelle instance de la classe [`StreamOutputAdapter`](../streamoutputadapter). |

## Propriétés

| Nom | Description |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Obtient le format de sortie. |
| [Stream](../../groupdocs.search.common/streamoutputadapter/stream) { get; } | Obtient un flux de sortie. |

### Remarques

**Learn more**

* [Output adapters](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Exemples

L'exemple montre une utilisation typique de la classe.

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

### Voir aussi

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
