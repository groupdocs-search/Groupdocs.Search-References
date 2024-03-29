---
title: FileLogger
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Rappresenta un logger che registra eventi ed errori in un file locale.
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
| [FileLogger](filelogger)(string, double) | Inizializza una nuova istanza di[`FileLogger`](../filelogger) classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FilePath](../../groupdocs.search.common/filelogger/filepath) { get; } | Ottiene il percorso del file di registro. |
| [MaxSize](../../groupdocs.search.common/filelogger/maxsize) { get; } | Ottiene la dimensione massima del file di registro in megabyte. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Error](../../groupdocs.search.common/filelogger/error)(string) | Registra un errore che si è verificato nell'indice. |
| [Trace](../../groupdocs.search.common/filelogger/trace)(string) | Registra un evento verificatosi nell'indice. |

### Osservazioni

**Saperne di più**

* [Registrazione](https://docs.groupdocs.com/display/searchnet/Logging)

### Esempi

L'esempio mostra un utilizzo tipico della classe.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";
string logPath = @"c:\Log.txt";

IndexSettings settings = new IndexSettings();
settings.Logger = new FileLogger(logPath, 4.0); // Specificando il percorso del file di registro e una lunghezza massima di 4 MB

Index index = new Index(indexFolder, settings); // Creazione di un indice nella cartella specificata

index.Add(documentsFolder); // Indicizzazione dei documenti dalla cartella specificata

SearchResult result = index.Search(query); // Cerca nell'indice
```

### Guarda anche

* interface [ILogger](../ilogger)
* spazio dei nomi [GroupDocs.Search.Common](../../groupdocs.search.common)
* assemblea [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
