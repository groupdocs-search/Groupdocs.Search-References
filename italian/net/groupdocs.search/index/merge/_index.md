---
title: "Merge"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Unisce l'indice specificato all'indice corrente. Nota che l'altro indice non verrà modificato."
type: docs
weight: 220
url: /it/net/groupdocs.search/index/merge/
---
## Merge(Index, MergeOptions) {#merge}

Unisce l'indice specificato all'indice corrente. Nota che l'altro indice non verrà modificato.

```csharp
public void Merge(Index index, MergeOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| index | Index | L'indice in cui eseguire il merge. |
| opzioni | MergeOptions | Le opzioni di unione. |

### Osservazioni

Se l'altro indice ha una versione precedente, deve essere aggiornato prima di eseguire il merge con [`IndexUpdater`](../../indexupdater).

### Esempi

L'esempio dimostra come unire un indice nell'indice corrente.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

Index index1 = new Index(indexFolder1); // Creating index1
index1.Add(documentsFolder1); // Indexing documents

Index index2 = new Index(indexFolder2); // Creating index2
index2.Add(documentsFolder2); // Indexing documents

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Creating cancellation object

// Unione di index2 in index1. Nota che i file di index2 non saranno modificati.
index1.Merge(index2, options);
```

### Vedi anche

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Merge(IndexRepository, MergeOptions) {#merge_1}

Unisce gli indici dal repository di indice specificato all'indice corrente. Nota che gli indici nel repository non verranno modificati.

```csharp
public void Merge(IndexRepository repository, MergeOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| repository | IndexRepository | Il repository di indice in cui eseguire il merge. |
| opzioni | MergeOptions | Le opzioni di unione. |

### Osservazioni

Se altri indici hanno una versione precedente, devono essere aggiornati prima di eseguire il merge con [`IndexUpdater`](../../indexupdater).

### Esempi

L'esempio dimostra come unire un repository di indice nell'indice corrente.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string indexFolder3 = @"c:\MyIndex3\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index1 = new Index(indexFolder1); // Creating index1
index1.Add(documentsFolder1); // Indexing documents

IndexRepository repository = new IndexRepository(); // Creating index repository

Index index2 = repository.Create(indexFolder2); // Creating index2
index2.Add(documentsFolder2); // Indexing documents

Index index3 = repository.Create(indexFolder3); // Creating index3
index3.Add(documentsFolder3); // Indexing documents

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Creating cancellation object

// Unione di tutti gli indici nel repository di indice in index1. Nota che index2 e index3 non saranno modificati.
index1.Merge(repository, options);
```

### Vedi anche

* class [IndexRepository](../../indexrepository)
* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
