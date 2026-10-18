---
title: "PasswordRequiredEventArgs"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt Argumente für das Ereignis dar, das auftritt, wenn ein durch ein Passwort geschütztes Dokument indiziert wird."
type: docs
weight: 610
url: /de/net/groupdocs.search.events/passwordrequiredeventargs/
---
## PasswordRequiredEventArgs class

Stellt Argumente für das Ereignis dar, das auftritt, wenn ein durch ein Passwort geschütztes Dokument indiziert wird.

```csharp
public class PasswordRequiredEventArgs : BaseIndexEventArgs
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DocumentFullPath](../../groupdocs.search.events/passwordrequiredeventargs/documentfullpath) { get; } | Liest den vollständigen Pfad des Dokuments. |
| [IndexFolder](../../groupdocs.search.events/baseindexeventargs/indexfolder) { get; } | Ermittelt den Indexordner. |
| [IndexId](../../groupdocs.search.events/baseindexeventargs/indexid) { get; } | Ermittelt die Index‑ID. |
| [Password](../../groupdocs.search.events/passwordrequiredeventargs/password) { get; set; } | Ruft das Passwort zum Öffnen des Dokuments ab oder legt es fest. |
| [Status](../../groupdocs.search.events/baseindexeventargs/status) { get; } | Ruft den Status des Index ab. |
| [Time](../../groupdocs.search.events/baseindexeventargs/time) { get; } | Ermittelt die Zeit eines Ereignisses. |

### Hinweise

**Learn more**

* [Search index events](https://docs.groupdocs.com/display/searchnet/Search+index+events)

### Siehe auch

* class [BaseIndexEventArgs](../baseindexeventargs)
* namespace [GroupDocs.Search.Events](../../groupdocs.search.events)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
