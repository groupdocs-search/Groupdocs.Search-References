---
title: "FileOutputAdapter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un adaptateur de sortie qui collecte la sortie dans un fichier."
type: docs
weight: 150
url: /fr/net/groupdocs.search.common/fileoutputadapter/
---
## FileOutputAdapter class

Représente un adaptateur de sortie qui collecte la sortie dans un fichier.

```csharp
public class FileOutputAdapter : OutputAdapter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FileOutputAdapter](fileoutputadapter)(OutputFormat, string) | Initialise une nouvelle instance de la classe [`FileOutputAdapter`](../fileoutputadapter). |

## Propriétés

| Nom | Description |
| --- | --- |
| [FilePath](../../groupdocs.search.common/fileoutputadapter/filepath) { get; } | Obtient un chemin de fichier de sortie. |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Obtient le format de sortie. |

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

FileOutputAdapter adapter = new FileOutputAdapter(@"c:\DocumentText.htm"); // Creating a file output adapter
index.GetDocumentText(documents[0], adapter); // Generating a document text into the output file
```

### Voir aussi

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
