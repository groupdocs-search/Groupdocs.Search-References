---
title: "IFieldExtractor"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Methoden zum Extrahieren von Feldern aus einem Dokument bereit."
type: docs
weight: 190
url: /de/net/groupdocs.search.common/ifieldextractor/
---
## IFieldExtractor interface

Stellt Methoden zum Extrahieren von Feldern aus einem Dokument bereit.

```csharp
public interface IFieldExtractor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Extensions](../../groupdocs.search.common/ifieldextractor/extensions) { get; } | Ermittelt die unterstützten Erweiterungen. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFields](../../groupdocs.search.common/ifieldextractor/getfields#getfields)(Stream) | Extrahiert alle Felder aus dem angegebenen Dokument. |
| [GetFields](../../groupdocs.search.common/ifieldextractor/getfields#getfields_1)(string) | Extrahiert alle Felder aus dem angegebenen Dokument. |

### Hinweise

**Learn more**

* [Custom text extractors](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Beispiele

Das Beispiel zeigt, wie man das Interface [`IFieldExtractor`](../ifieldextractor) implementiert.

```csharp
public class LogExtractor : IFieldExtractor
{
    private readonly string[] extensions = new string[] { ".log" };

    public string[] Extensions
    {
        get { return extensions; }
    }

    public DocumentField[] GetFields(string filePath)
    {
        FileInfo fileInfo = new FileInfo(filePath);
        DocumentField[] fields = new DocumentField[]
        {
            new DocumentField("FileName", fileInfo.FullName),
            new DocumentField("CreationDate", fileInfo.CreationTime.ToString(CultureInfo.InvariantCulture)),
            new DocumentField("Content", ExtractContent(filePath)),
        };
        return fields;
    }

    private string ExtractContent(string filePath)
    {
        StringBuilder result = new StringBuilder();
        using (StreamReader streamReader = File.OpenText(filePath))
        {
            string line = streamReader.ReadLine();
            string processedLine = line.Remove(0, 12);
            result.AppendLine(processedLine);
        }
        return result.ToString();
    }
}
```

Das Beispiel zeigt, wie man den custorm extractor für die Indizierung verwendet.

```csharp
string indexFolder = @"c:\MyIndex\"; // Specify path to the index folder
string documentsFolder = @"c:\MyDocuments\"; // Specify path to a folder containing documents to search

Index index = new Index(indexFolder); // Creating or loading an index

index.IndexSettings.CustomExtractors.Add(new LogExtractor()); // Adding custom text extractor to index settings

index.Add(documentsFolder); // Indexing documents from the specified folder
```

### Siehe auch

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
