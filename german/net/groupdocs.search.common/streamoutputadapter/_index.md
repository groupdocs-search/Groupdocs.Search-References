---
title: "StreamOutputAdapter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Ausgabeadapter dar, der Ausgaben in einen Stream sammelt."
type: docs
weight: 310
url: /de/net/groupdocs.search.common/streamoutputadapter/
---
## StreamOutputAdapter class

Stellt einen Ausgabeadapter dar, der Ausgaben in einen Stream sammelt.

```csharp
public class StreamOutputAdapter : OutputAdapter
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [StreamOutputAdapter](streamoutputadapter)(OutputFormat, Stream) | Initialisiert eine neue Instanz der [`StreamOutputAdapter`](../streamoutputadapter)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Liefert das Ausgabeformat. |
| [Stream](../../groupdocs.search.common/streamoutputadapter/stream) { get; } | Liefert einen Ausgabestream. |

### Hinweise

**Learn more**

* [Output adapters](https://docs.groupdocs.com/display/searchnet/Output+adapters)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

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

### Siehe auch

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
