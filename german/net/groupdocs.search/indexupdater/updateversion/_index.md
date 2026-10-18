---
title: "UpdateVersion"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Führt die Neuindizierung von Dokumenten in einem Index einer alten Version durch. Der aktualisierte Index wird im Verzeichnis newIndexPath abgelegt. Der Index im Verzeichnis indexPath wird nicht geändert."
type: docs
weight: 40
url: /de/net/groupdocs.search/indexupdater/updateversion/
---
## IndexUpdater.UpdateVersion method

Führt das Reindizieren von Dokumenten in einem Index einer alten Version durch. Der aktualisierte Index wird im Verzeichnis *newIndexPath* abgelegt. Der Index im Verzeichnis *indexPath* wird nicht geändert.

```csharp
public VersionUpdateResult UpdateVersion(string indexPath, string newIndexPath)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexPath | String | Der Pfad zum Indexverzeichnis. |
| newIndexPath | String | Das Verzeichnis für den aktualisierten Index. |

### Rückgabewert

Das Ergebnis der Indexversions-Aktualisierungsoperation.

### Siehe auch

* enum [VersionUpdateResult](../../../groupdocs.search.common/versionupdateresult)
* class [IndexUpdater](../../indexupdater)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
