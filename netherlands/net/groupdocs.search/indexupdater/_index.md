---
title: IndexUpdater
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Vertegenwoordigt een indexupdater. Deze klasse voert herindexering van documenten uit in een index van een oude versie.
type: docs
weight: 710
url: /nl/net/groupdocs.search/indexupdater/
---
## IndexUpdater class

Vertegenwoordigt een indexupdater. Deze klasse voert herindexering van documenten uit in een index van een oude versie.

```csharp
public class IndexUpdater
```

## Constructeurs

| Naam | Beschrijving |
| --- | --- |
| [IndexUpdater](indexupdater)() | Initialiseert een nieuw exemplaar van het[`IndexUpdater`](../indexupdater) klasse. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | Controleert of een index in de opgegeven map kan worden bijgewerkt naar de laatste versie. |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | Controleert of de opgegeven map een index van de laatste versie bevat. |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | Voert herindexering van documenten uit in een index van een oude versie. De bijgewerkte index wordt in de*newIndexPath* directory. De index in het*indexPath* map wordt niet gewijzigd. |

### Opmerkingen

**Kom meer te weten**

* [Index bijwerken](https://docs.groupdocs.com/display/searchnet/Update+index)

### Voorbeelden

Het voorbeeld demonstreert een typisch gebruik van de klasse.

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### Zie ook

* naamruimte [GroupDocs.Search](../../groupdocs.search)
* montage [GroupDocs.Search](../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->