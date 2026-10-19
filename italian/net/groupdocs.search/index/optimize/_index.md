---
title: "Ottimizza"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Riduce il numero di segmenti dell'indice unendoli tra loro. Questa operazione migliora le prestazioni della ricerca."
type: docs
weight: 240
url: /it/net/groupdocs.search/index/optimize/
---
## Optimize() {#optimize}

Riduce il numero di segmenti dell'indice unendoli tra loro. Questa operazione migliora le prestazioni della ricerca.

```csharp
public void Optimize()
```

### Esempi

L'esempio dimostra come unire segmenti di un indice.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creating index in the specified folder

index.Add(documentsFolder1); // Indexing documents from the specified folder
index.Add(documentsFolder2); // Each call to Add creates at least one new segment in the index
index.Add(documentsFolder3);

// Unione dei segmenti dell'indice
index.Optimize();
```

### Vedi anche

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Optimize(MergeOptions) {#optimize_1}

Riduce il numero di segmenti dell'indice unendoli tra loro. Questa operazione migliora le prestazioni della ricerca.

```csharp
public void Optimize(MergeOptions options)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| opzioni | MergeOptions | Le opzioni di unione. |

### Esempi

L'esempio dimostra come unire segmenti di un indice con opzioni di unione specifiche.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creating index in the specified folder

index.Add(documentsFolder1); // Indexing documents from the specified folder
index.Add(documentsFolder2); // Each call to Add creates at least one new segment in the index
index.Add(documentsFolder3);

MergeOptions options = new MergeOptions();
options.IsAsync = true; // Asynchronous operation
options.Cancellation = new Cancellation(); // Creating cancellation object

// Unione dei segmenti dell'indice
index.Optimize(options); // This method will return before the operation is completed

options.Cancellation.CancelAfter(10000); // Setting maximum duration of the operation to 10 seconds
```

### Vedi anche

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
