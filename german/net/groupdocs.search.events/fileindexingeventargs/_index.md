---
title: "FileIndexingEventArgs"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Argumente für das Ereignis des Beginns der Dokumentindizierung dar."
type: docs
weight: 540
url: /de/net/groupdocs.search.events/fileindexingeventargs/
---
## FileIndexingEventArgs class

Stellt Argumente für das Ereignis des Beginns der Dokumentindizierung dar.

```csharp
public class FileIndexingEventArgs : BaseIndexEventArgs
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AdditionalFields](../../groupdocs.search.events/fileindexingeventargs/additionalfields) { get; set; } | Liest oder setzt die zusätzlichen Felder für das Dokument. |
| [Attributes](../../groupdocs.search.events/fileindexingeventargs/attributes) { get; set; } | Liest oder setzt die Attribute des Dokuments. |
| [CustomExtractor](../../groupdocs.search.events/fileindexingeventargs/customextractor) { get; set; } | Liest oder setzt den benutzerdefinierten Text-Extraktor. |
| [Document](../../groupdocs.search.events/fileindexingeventargs/document) { get; } | Liest das Dokument. |
| [DocumentFullPath](../../groupdocs.search.events/fileindexingeventargs/documentfullpath) { get; } | Liest den vollständigen Pfad des Dokuments. |
| [DocumentKey](../../groupdocs.search.events/fileindexingeventargs/documentkey) { get; } | Gibt den Dokumentenschlüssel zurück. |
| [Encoding](../../groupdocs.search.events/fileindexingeventargs/encoding) { get; set; } | Liest oder setzt die Kodierung des Dokuments. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ermittelt den Indexordner. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ermittelt die Index‑ID. |
| [SkipIndexing](../../groupdocs.search.events/fileindexingeventargs/skipindexing) { get; set; } | Liest oder setzt einen Wert, der angibt, dass die Indexierung des Dokuments übersprungen werden soll. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ruft den Status des Index ab. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ermittelt die Zeit eines Ereignisses. |
| [WordSplitter](../../groupdocs.search.events/fileindexingeventargs/wordsplitter) { get; set; } | Liest oder setzt den benutzerdefinierten Worttrenner, der zum Aufteilen von Text in Wörter verwendet wird. |

### Hinweise

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Siehe auch

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
