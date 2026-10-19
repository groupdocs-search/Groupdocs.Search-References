---
title: "UpdateVersion"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Esegue il reindicizzamento dei documenti in un indice di una versione precedente. L'indice aggiornato verrà collocato nella directory newIndexPath. L'indice nella directory indexPath non verrà modificato."
type: docs
weight: 40
url: /it/net/groupdocs.search/indexupdater/updateversion/
---
## IndexUpdater.UpdateVersion method

Esegue il reindicizzamento dei documenti in un indice di una versione precedente. L'indice aggiornato sarà collocato nella directory *newIndexPath*. L'indice nella directory *indexPath* non verrà modificato.

```csharp
public VersionUpdateResult UpdateVersion(string indexPath, string newIndexPath)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexPath | String | Il percorso della directory dell'indice. |
| newIndexPath | String | La directory per l'indice aggiornato. |

### Valore di ritorno

Il risultato dell'operazione di aggiornamento della versione dell'indice.

### Vedi anche

* enum [VersionUpdateResult](../../../groupdocs.search.common/versionupdateresult)
* class [IndexUpdater](../../indexupdater)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
