---
title: "IndexUpdater"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Représente une mise à jour d'index. Cette classe effectue le réindexage des documents dans un index d'une version antérieure."
type: docs
weight: 730
url: /fr/net/groupdocs.search/indexupdater/
---
## IndexUpdater class

Représente une mise à jour d'index. Cette classe effectue le réindexage des documents dans un index d'une version antérieure.

```csharp
public class IndexUpdater
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [IndexUpdater](indexupdater)() | Initialise une nouvelle instance de la classe [`IndexUpdater`](../indexupdater). |

## Méthodes

| Nom | Description |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | Vérifie si un index dans le répertoire spécifié peut être mis à jour vers la dernière version. |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | Vérifie si le répertoire spécifié contient un index de la dernière version. |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | Effectue le réindexage des documents dans un index d'une ancienne version. L'index mis à jour sera placé dans le répertoire *newIndexPath*. L'index du répertoire *indexPath* ne sera pas modifié. |

### Remarques

**Learn more**

* [Update index](https://docs.groupdocs.com/display/searchnet/Update+index)

### Exemples

L'exemple montre une utilisation typique de la classe.

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### Voir aussi

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
