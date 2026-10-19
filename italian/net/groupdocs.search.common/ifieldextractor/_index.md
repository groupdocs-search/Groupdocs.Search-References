---
title: "IFieldExtractor"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Fornisce metodi per estrarre campi da un documento."
type: docs
weight: 190
url: /it/net/groupdocs.search.common/ifieldextractor/
---
## IFieldExtractor interface

Fornisce metodi per estrarre campi da un documento.

```csharp
public interface IFieldExtractor
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Extensions](../../groupdocs.search.common/ifieldextractor/extensions) { get; } | Ottiene le estensioni supportate. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFields](../../groupdocs.search.common/ifieldextractor/getfields#getfields)(Stream) | Estrae tutti i campi dal documento specificato. |
| [GetFields](../../groupdocs.search.common/ifieldextractor/getfields#getfields_1)(string) | Estrae tutti i campi dal documento specificato. |

### Osservazioni

**Learn more**

* [Custom text extractors](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Esempi

L'esempio dimostra come implementare l'interfaccia [`IFieldExtractor`](../ifieldextractor).

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

L'esempio dimostra come utilizzare l'estrattore personalizzato per l'indicizzazione.

```csharp
string indexFolder = @"c:\MyIndex\"; // Specify path to the index folder
string documentsFolder = @"c:\MyDocuments\"; // Specify path to a folder containing documents to search

Index index = new Index(indexFolder); // Creating or loading an index

index.IndexSettings.CustomExtractors.Add(new LogExtractor()); // Adding custom text extractor to index settings

index.Add(documentsFolder); // Indexing documents from the specified folder
```

### Vedi anche

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
