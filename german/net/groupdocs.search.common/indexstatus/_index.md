---
title: "IndexStatus"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Gibt einen Indexstatus an."
type: docs
weight: 240
url: /de/net/groupdocs.search.common/indexstatus/
---
## IndexStatus enumeration

Gibt einen Indexstatus an.

```csharp
public enum IndexStatus
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Ready | `0` | Der Index ist frei und bereit für Änderungen. |
| Failed | `1` | Der Index muss aufgrund eines Fehlers neu geladen werden. |
| Indexing | `2` | Der Index führt einen Indexierungsvorgang aus. |
| Updating | `3` | Der Index führt einen Aktualisierungsvorgang aus. |
| Merging | `4` | Der Index führt einen Zusammenführungsvorgang aus. |
| Optimizing | `5` | Der Index führt einen Optimierungsvorgang aus. |
| Deleting | `6` | Der Index führt einen Löschvorgang aus. |
| Renaming | `7` | Der Index führt einen Umbenennungsvorgang aus. |
| ChangingAttributes | `8` | Der Index ändert Attribute. |
| CheckingSegments | `9` | Der Index prüft Segmente. |
| SavingTheIndex | `10` | Der Index wird in einen anderen Ordner gespeichert. |

### Siehe auch

* namespace [GroupDocs.Search.Common](../../groupdocs.search.common)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
