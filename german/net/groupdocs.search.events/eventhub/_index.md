---
title: "EventHub"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Bietet Indexereignisse zum Abonnieren an."
type: docs
weight: 530
url: /de/net/groupdocs.search.events/eventhub/
---
## EventHub class

Bietet Indexereignisse zum Abonnieren an.

```csharp
public class EventHub
```

## Ereignisse

| Name | Beschreibung |
| --- | --- |
| event [ErrorOccurred](../../groupdocs.search.events/eventhub/erroroccurred) | Tritt auf, wenn ein Fehler während einer Indexoperation auftritt. |
| event [FileIndexing](../../groupdocs.search.events/eventhub/fileindexing) | Tritt auf, wenn ein Dokument indiziert werden soll. |
| event [ImagePreparing](../../groupdocs.search.events/eventhub/imagepreparing) | Tritt auf, wenn ein Bild für die Indizierung vorbereitet wird. |
| event [OperationFinished](../../groupdocs.search.events/eventhub/operationfinished) | Tritt auf, wenn ein Indexvorgang abgeschlossen ist. |
| event [OperationProgressChanged](../../groupdocs.search.events/eventhub/operationprogresschanged) | Tritt auf, wenn sich der Fortschritt des Indexierungs- oder Aktualisierungsvorgangs ändert. |
| event [OptimizationProgressChanged](../../groupdocs.search.events/eventhub/optimizationprogresschanged) | Tritt auf, wenn sich der Fortschritt des Optimierungsvorgangs ändert. |
| event [PasswordRequired](../../groupdocs.search.events/eventhub/passwordrequired) | Tritt auf, wenn ein Dokument ein Passwort zum Öffnen benötigt. |
| event [SearchPhaseCompleted](../../groupdocs.search.events/eventhub/searchphasecompleted) | Tritt auf, wenn die Suchphase abgeschlossen ist. |
| event [StatusChanged](../../groupdocs.search.events/eventhub/statuschanged) | Tritt auf, wenn sich der Indexstatus ändert. |

### Hinweise

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Beispiele

Das Beispiel demonstriert eine typische Verwendung der Schnittstelle.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query = "Einstein";

// Erstellen eines Index
Index index = new Index(indexFolder);

// Abonnieren des Ereignisses
index.Events.ErrorOccurred += (sender, args) =>
{
    Console.WriteLine(args.Message);
};

// Indizierung von Dokumenten aus dem angegebenen Ordner
index.Add(documentsFolder);

// Durchsuchen des Index
SearchResult result = index.Search(query);
```

### Siehe auch

* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
