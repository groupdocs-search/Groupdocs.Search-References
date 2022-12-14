---
title: Delete
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Elimina i file o le cartelle indicizzati dallindice. Quindi aggiorna lindice senza percorsi eliminati. Nota che un singolo documento non può essere eliminato dallindice se è stato aggiunto allindice come parte di una cartella.
type: docs
weight: 90
url: /it/net/groupdocs.search/index/delete/
---
## Delete(string[], UpdateOptions) {#delete_1}

Elimina i file o le cartelle indicizzati dall'indice. Quindi aggiorna l'indice senza percorsi eliminati. Nota che un singolo documento non può essere eliminato dall'indice se è stato aggiunto all'indice come parte di una cartella.

```csharp
public DeleteResult Delete(string[] paths, UpdateOptions options)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| paths | String[] | I percorsi dei file o delle cartelle da eliminare. |
| options | UpdateOptions | Le opzioni di aggiornamento. |

### Valore di ritorno

Un oggetto che descrive il risultato dell'eliminazione di file o cartelle dall'indice.

### Esempi

L'esempio mostra come eliminare i percorsi indicizzati da un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments\";
string documentsFolder2 = @"c:\MyDocuments2\";

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);

// Indicizzazione dei documenti dalle cartelle specificate
index.Add(documentsFolder1);
index.Add(documentsFolder2);

// Ottenere percorsi indicizzati dall'indice
string[] indexedPaths1 = index.GetIndexedPaths();

// Scrittura di percorsi indicizzati nella console
Console.WriteLine("Indexed paths:");
foreach (string path in indexedPaths1)
{
    Console.WriteLine("\t" + path);
}

// Eliminazione del percorso dell'indice dall'indice
DeleteResult deleteResult = index.Delete(new string[] { documentsFolder1 }, new UpdateOptions());

// Ottenere percorsi indicizzati dopo l'eliminazione
string[] indexedPaths2 = index.GetIndexedPaths();
Console.WriteLine("\nDeleted paths: " + deleteResult.SuccessCount);

Console.WriteLine("\nIndexed paths:");
foreach (string path in indexedPaths2)
{
    Console.WriteLine("\t" + path);
}
```

### Guarda anche

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

---

## Delete(UpdateOptions, string[]) {#delete}

Elimina i documenti indicizzati da flussi o strutture. Quindi aggiorna l'indice senza documenti eliminati.

```csharp
public DeleteResult Delete(UpdateOptions options, string[] documentKeys)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| options | UpdateOptions | Le opzioni di aggiornamento. |
| documentKeys | String[] | Le chiavi dei documenti aggiunti da flussi o strutture. |

### Valore di ritorno

Un oggetto che descrive il risultato dell'eliminazione di documenti dall'indice.

### Guarda anche

* class [DeleteResult](../../../groupdocs.search.results/deleteresult)
* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* spazio dei nomi [GroupDocs.Search](../../index)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
