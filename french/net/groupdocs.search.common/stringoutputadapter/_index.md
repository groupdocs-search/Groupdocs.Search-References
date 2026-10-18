---
title: "StringOutputAdapter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un adaptateur de sortie qui collecte la sortie sous forme de chaîne."
type: docs
weight: 320
url: /fr/net/groupdocs.search.common/stringoutputadapter/
---
## StringOutputAdapter class

Représente un adaptateur de sortie qui collecte la sortie sous forme de chaîne.

```csharp
public class StringOutputAdapter : OutputAdapter
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [StringOutputAdapter](stringoutputadapter)(OutputFormat) | Initialise une nouvelle instance de la classe [`StringOutputAdapter`](../stringoutputadapter). |

## Propriétés

| Nom | Description |
| --- | --- |
| [OutputFormat](../../groupdocs.search.common/resultbuilderfactory/outputformat) { get; } | Obtient le format de sortie. |

## Méthodes

| Nom | Description |
| --- | --- |
| [GetResult](../../groupdocs.search.common/stringoutputadapter/getresult)() | Obtient la chaîne résultante. |

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

StringOutputAdapter adapter = new StringOutputAdapter(OutputFormat.Html); // Creating a string output adapter
index.GetDocumentText(documents[0], adapter); // Generating a document text into the adapter
String result = adapter.GetResult(); // Getting a result
```

### Voir aussi

* class [OutputAdapter](../outputadapter)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
