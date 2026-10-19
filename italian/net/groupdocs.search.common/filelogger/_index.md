---
title: "FileLogger"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un logger che registra eventi ed errori in un file locale."
type: docs
weight: 140
url: /it/net/groupdocs.search.common/filelogger/
---
## FileLogger class

Rappresenta un logger che registra eventi ed errori in un file locale.

```csharp
public class FileLogger : ILogger
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [FileLogger](filelogger)(string, double) | Inizializza una nuova istanza della classe [`FileLogger`](../filelogger). |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FilePath](../../groupdocs.search.common/filelogger/filepath) { get; } | Restituisce il percorso del file di log. |
| [MaxSize](../../groupdocs.search.common/filelogger/maxsize) { get; } | Restituisce la dimensione massima del file di log in megabyte. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Error](../../groupdocs.search.common/filelogger/error)(string) | Registra un errore verificatosi nell'indice. |
| [Trace](../../groupdocs.search.common/filelogger/trace)(string) | Registra un evento verificatosi nell'indice. |

### Osservazioni

**Learn more**

* [Logging](https://docs.groupdocs.com/display/searchnet/Logging)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

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

### Vedi anche

* interface [ILogger](../ilogger)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
