---
title: "IndexUpdater"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Rappresenta un aggiornatore di indice. Questa classe esegue la reindicizzazione dei documenti in un indice di una versione precedente."
type: docs
weight: 730
url: /it/net/groupdocs.search/indexupdater/
---
## IndexUpdater class

Rappresenta un aggiornatore di indice. Questa classe esegue la reindicizzazione dei documenti in un indice di una versione precedente.

```csharp
public class IndexUpdater
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [IndexUpdater](indexupdater)() | Inizializza una nuova istanza della classe [`IndexUpdater`](../indexupdater). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CanUpdateVersion](../../groupdocs.search/indexupdater/canupdateversion)(string) | Verifica se un indice nella directory specificata può essere aggiornato all'ultima versione. |
| [IsLatestVersion](../../groupdocs.search/indexupdater/islatestversion)(string) | Verifica se la directory specificata contiene un indice dell'ultima versione. |
| [UpdateVersion](../../groupdocs.search/indexupdater/updateversion)(string, string) | Esegue il reindicizzamento dei documenti in un indice di una versione precedente. L'indice aggiornato sarà collocato nella directory *newIndexPath*. L'indice nella directory *indexPath* non verrà modificato. |

### Osservazioni

**Learn more**

* [Update index](https://docs.groupdocs.com/display/searchnet/Update+index)

### Esempi

L'esempio dimostra un utilizzo tipico della classe.

```csharp
string sourceIndexFolder = @"c:\MyOldIndex\";
string targetIndexFolder = @"c:\MyNewIndex\";

IndexUpdater updater = new IndexUpdater();

if (updater.CanUpdateVersion(sourceIndexFolder))
{
    VersionUpdateResult result = updater.UpdateVersion(sourceIndexFolder, targetIndexFolder);
}
```

### Vedi anche

* namespace [GroupDocs.Search](../../groupdocs.search)
* assembly [GroupDocs.Search](../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
