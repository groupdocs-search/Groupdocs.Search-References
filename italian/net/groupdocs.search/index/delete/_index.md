---
title: "Delete"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Elimina file o cartelle indicizzate dall'indice. Quindi aggiorna l'indice senza i percorsi eliminati. Nota che un documento individuale non può essere eliminato dall'indice se è stato aggiunto all'indice come parte di una cartella."
type: docs
weight: 110
url: /it/net/groupdocs.search/index/delete/
---
## Delete(string[], UpdateOptions) {#delete_1}

Elimina file o cartelle indicizzate dall'indice. Quindi aggiorna l'indice senza i percorsi eliminati. Nota che un documento individuale non può essere eliminato dall'indice se è stato aggiunto all'indice come parte di una cartella.

```csharp
public DeleteResult Delete(string[] paths, UpdateOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| percorsi | String[] | I percorsi dei file o delle cartelle da eliminare. |
| opzioni | UpdateOptions | Le opzioni di aggiornamento. |

### Valore di ritorno

Un oggetto che descrive il risultato dell'eliminazione di file o cartelle dall'indice.

### Esempi

L'esempio dimostra come eliminare i percorsi indicizzati da un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalle cartelle specificate
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Ottenere i percorsi indicizzati dall'indice
string[] indexedPaths1 = index.GetIndexedPaths();

// Scrivere i percorsi indicizzati sulla console
Console.WriteLine("Indexed paths:");
foreach (string path in indexedPaths1)
{
    Console.WriteLine("\t" + path);
}

// Eliminare il percorso dell'indice dall'indice
DeleteResult deleteResult = index.Delete(new string[] { documentsFolder1 }, new UpdateOptions());

// Ottenere i percorsi indicizzati dopo l'eliminazione
string[] indexedPaths2 = index.GetIndexedPaths();
Console.WriteLine("\nDeleted paths: " + deleteResult.SuccessCount);

Console.WriteLine("\nIndexed paths:");
foreach (string path in indexedPaths2)
{
    Console.WriteLine("\t" + path);
}
```

### Vedi anche

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Delete(UpdateOptions, string[]) {#delete}

Elimina i documenti indicizzati da stream o strutture. Quindi aggiorna l'indice senza i documenti eliminati.

```csharp
public DeleteResult Delete(UpdateOptions options, string[] documentKeys)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| opzioni | UpdateOptions | Le opzioni di aggiornamento. |
| documentKeys | String[] | Le chiavi dei documenti aggiunti da flussi o strutture. |

### Valore di ritorno

Un oggetto che descrive il risultato dell'eliminazione dei documenti dall'indice.

### Vedi anche

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
