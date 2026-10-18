---
title: "FileLogger"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente un journal qui enregistre les événements et les erreurs dans un fichier local."
type: docs
weight: 140
url: /fr/net/groupdocs.search.common/filelogger/
---
## FileLogger class

Représente un journal qui enregistre les événements et les erreurs dans un fichier local.

```csharp
public class FileLogger : ILogger
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [FileLogger](filelogger)(string, double) | Initialise une nouvelle instance de la classe [`FileLogger`](../filelogger). |

## Propriétés

| Nom | Description |
| --- | --- |
| [FilePath](../../groupdocs.search.common/filelogger/filepath) { get; } | Obtient le chemin du fichier journal. |
| [MaxSize](../../groupdocs.search.common/filelogger/maxsize) { get; } | Obtient la taille maximale du fichier journal en mégaoctets. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Error](../../groupdocs.search.common/filelogger/error)(string) | Enregistre une erreur survenue dans l'index. |
| [Trace](../../groupdocs.search.common/filelogger/trace)(string) | Enregistre un événement survenu dans l'index. |

### Remarques

**Learn more**

* [Logging](https://docs.groupdocs.com/display/searchnet/Logging)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";
string logPath = @"c:\Log.txt";

IndexSettings settings = new IndexSettings();
settings.Logger = new FileLogger(logPath, 4.0); // Specifying the path to the log file and a maximum length of 4 MB

Index index = new Index(indexFolder, settings); // Creating an index in the specified folder

index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result = index.Search(query); // Search in index
```

### Voir aussi

* interface [ILogger](../ilogger)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
