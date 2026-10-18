---
title: "UpdateVersion"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Effectue le réindexage des documents dans un index d'ancienne version. L'index mis à jour sera placé dans le répertoire newIndexPath. L'index du répertoire indexPath ne sera pas modifié."
type: docs
weight: 40
url: /fr/net/groupdocs.search/indexupdater/updateversion/
---
## IndexUpdater.UpdateVersion method

Effectue le réindexage des documents dans un index d'une ancienne version. L'index mis à jour sera placé dans le répertoire *newIndexPath*. L'index du répertoire *indexPath* ne sera pas modifié.

```csharp
public VersionUpdateResult UpdateVersion(string indexPath, string newIndexPath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexPath | String | Le chemin du répertoire d'index. |
| newIndexPath | String | Le répertoire pour l'index mis à jour. |

### Valeur de retour

Le résultat de l'opération de mise à jour de version d'index.

### Voir aussi

* enum [VersionUpdateResult](../../../groupdocs.search.common/versionupdateresult)
* class [IndexUpdater](../../indexupdater)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
