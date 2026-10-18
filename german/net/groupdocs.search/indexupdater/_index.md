---
title: "IndexUpdater"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Stellt einen Index-Aktualisierer dar. Diese Klasse führt das Reindizieren von Dokumenten in einem Index einer alten Version durch."
type: docs
weight: 730
url: /de/net/groupdocs.search/indexupdater/
---
## IndexUpdater class

Stellt einen Index-Aktualisierer dar. Diese Klasse führt das Reindizieren von Dokumenten in einem Index einer alten Version durch.

```csharp
public class IndexUpdater
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [IndexUpdater](indexupdater)() | Initialisiert eine neue Instanz der [`IndexUpdater`](../indexupdater)-Klasse. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | Prüft, ob ein Index im angegebenen Verzeichnis auf die neueste Version aktualisiert werden kann. |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | Prüft, ob das angegebene Verzeichnis einen Index der neuesten Version enthält. |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | Führt das Reindizieren von Dokumenten in einem Index einer alten Version durch. Der aktualisierte Index wird im Verzeichnis *newIndexPath* abgelegt. Der Index im Verzeichnis *indexPath* wird nicht geändert. |

### Hinweise

**Learn more**

* [Update index](https://docs.groupdocs.com/display/searchnet/Update+index)

### Beispiele

Das Beispiel zeigt eine typische Verwendung der Klasse.

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### Siehe auch

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
