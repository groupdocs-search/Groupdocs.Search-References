---
title: "FileLogger"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Logger dar, der Ereignisse und Fehler in eine lokale Datei protokolliert."
type: docs
weight: 140
url: /de/net/groupdocs.search.common/filelogger/
---
## FileLogger class

Stellt einen Logger dar, der Ereignisse und Fehler in eine lokale Datei protokolliert.

```csharp
public class FileLogger : ILogger
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [FileLogger](filelogger)(string, double) | Initialisiert eine neue Instanz der [`FileLogger`](../filelogger)-Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [FilePath](../../groupdocs.search.common/filelogger/filepath) { get; } | Liefert den Pfad der Protokolldatei. |
| [MaxSize](../../groupdocs.search.common/filelogger/maxsize) { get; } | Liefert die maximale Größe der Protokolldatei in Megabyte. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Error](../../groupdocs.search.common/filelogger/error)(string) | Protokolliert einen Fehler, der im Index aufgetreten ist. |
| [Trace](../../groupdocs.search.common/filelogger/trace)(string) | Protokolliert ein Ereignis, das im Index aufgetreten ist. |

### Hinweise

**Learn more**

* [Logging](https://docs.groupdocs.com/display/searchnet/Logging)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

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

### Siehe auch

* interface [ILogger](../ilogger)
* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
