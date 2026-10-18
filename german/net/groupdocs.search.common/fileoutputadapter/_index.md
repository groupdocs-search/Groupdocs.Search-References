---
title: "FileOutputAdapter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Ausgabeadapter dar, der Ausgaben in einer Datei sammelt."
type: docs
weight: 150
url: /de/net/groupdocs.search.common/fileoutputadapter/
---
## FileOutputAdapter class

Stellt einen Ausgabeadapter dar, der Ausgaben in einer Datei sammelt.

```csharp
public class FileOutputAdapter : OutputAdapter
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FileOutputAdapter](fileoutputadapter)(OutputFormat, string) | Initialisiert eine neue Instanz der [`FileOutputAdapter`](../fileoutputadapter)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FilePath](../../groupdocs.search.common/fileoutputadapter/filepath) { get; } | Ruft einen Ausgabedateipfad ab. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Liefert das Ausgabeformat. |

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

FileOutputAdapter adapter = new FileOutputAdapter(@"c:\DocumentText.htm"); // Creating a file output adapter
index.GetDocumentText(documents[0], adapter); // Generating a document text into the output file
```

### Siehe auch

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
