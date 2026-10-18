---
title: "IFieldExtractor"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fournit des méthodes pour extraire des champs d'un document."
type: docs
weight: 190
url: /fr/net/groupdocs.search.common/ifieldextractor/
---
## IFieldExtractor interface

Fournit des méthodes pour extraire des champs d'un document.

```csharp
public interface IFieldExtractor
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Extensions](../../groupdocs.search.common/ifieldextractor/extensions) { get; } | Obtient les extensions prises en charge. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetFields](../../groupdocs.search.common/ifieldextractor/getfields#getfields)(Stream) | Extrait tous les champs du document spécifié. |
| [GetFields](../../groupdocs.search.common/ifieldextractor/getfields#getfields_1)(string) | Extrait tous les champs du document spécifié. |

### Remarques

**Learn more**

* [Custom text extractors](https://docs.groupdocs.com/display/searchnet/Custom+text+extractors)

### Exemples

L'exemple montre comment implémenter l'interface [`IFieldExtractor`](../ifieldextractor).

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

L'exemple montre comment utiliser l'extracteur personnalisé pour l'indexation.

```csharp
string indexFolder = @"c:\MyIndex\"; // Specify path to the index folder
string documentsFolder = @"c:\MyDocuments\"; // Specify path to a folder containing documents to search

Index index = new Index(indexFolder); // Creating or loading an index

index.IndexSettings.CustomExtractors.Add(new LogExtractor()); // Adding custom text extractor to index settings

index.Add(documentsFolder); // Indexing documents from the specified folder
```

### Voir aussi

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
