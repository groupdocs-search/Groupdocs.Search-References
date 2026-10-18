---
title: "OperationProgressEventArgs"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt die Argumente für das Fortschrittsänderungsereignis der Indexierungsoperation bereit."
type: docs
weight: 580
url: /de/net/groupdocs.search.events/operationprogresseventargs/
---
## OperationProgressEventArgs class

Stellt die Argumente für das Fortschrittsänderungsereignis der Indexierungsoperation bereit.

```csharp
public class OperationProgressEventArgs : BaseIndexEventArgs
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ermittelt den Indexordner. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ermittelt die Index‑ID. |
| [LastDocumentKey](../../groupdocs.search.events/operationprogresseventargs/lastdocumentkey) { get; } | Ruft den Schlüssel des zuletzt verarbeiteten Dokuments ab. |
| [LastDocumentPath](../../groupdocs.search.events/operationprogresseventargs/lastdocumentpath) { get; } | Ruft den Pfad des zuletzt verarbeiteten Dokuments ab. |
| [LastDocumentStatus](../../groupdocs.search.events/operationprogresseventargs/lastdocumentstatus) { get; } | Ruft den Status des zuletzt verarbeiteten Dokuments ab. |
| [ProcessedDocuments](../../groupdocs.search.events/operationprogresseventargs/processeddocuments) { get; } | Ruft die Anzahl erfolgreich verarbeiteter Dokumente ab. |
| [ProgressPercentage](../../groupdocs.search.events/operationprogresseventargs/progresspercentage) { get; } | Ermittelt den Prozentsatz des Fortschritts. |
| [SkippedDocuments](../../groupdocs.search.events/operationprogresseventargs/skippeddocuments) { get; } | Ruft die Anzahl übersprungener Dokumente ab. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ruft den Status des Index ab. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ermittelt die Zeit eines Ereignisses. |
| [TotalDocuments](../../groupdocs.search.events/operationprogresseventargs/totaldocuments) { get; } | Ermittelt die Gesamtzahl der zu verarbeitenden Dokumente. |

### Hinweise

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Siehe auch

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
