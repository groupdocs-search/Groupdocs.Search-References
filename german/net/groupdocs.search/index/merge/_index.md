---
title: "Merge"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Führt den angegebenen Index in den aktuellen Index zusammen. Hinweis: Der andere Index wird nicht geändert."
type: docs
weight: 220
url: /de/net/groupdocs.search/index/merge/
---
## Merge(Index, MergeOptions) {#merge}

Führt den angegebenen Index in den aktuellen Index zusammen. Hinweis: Der andere Index wird nicht geändert.

```csharp
public void Merge(Index index, MergeOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| index | Index | Der Index, in den zusammengeführt werden soll. |
| Optionen | MergeOptions | Die Zusammenführungsoptionen. |

### Hinweise

Wenn der andere Index eine vorherige Version hat, muss er vor dem Zusammenführen mit [`IndexUpdater`](../../indexupdater) aktualisiert werden.

### Beispiele

Das Beispiel zeigt, wie man einen Index in den aktuellen Index zusammenführt.

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

// Zusammenführen von index2 in index1. Hinweis: Die Dateien von index2 werden nicht geändert.
index1.Merge(index2, options);
```

### Siehe auch

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Merge(IndexRepository, MergeOptions) {#merge_1}

Führt Indizes aus dem angegebenen Index-Repository in den aktuellen Index zusammen. Hinweis: Die Indizes im Repository werden nicht geändert.

```csharp
public void Merge(IndexRepository repository, MergeOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Repository | IndexRepository | Das Index-Repository, in das zusammengeführt werden soll. |
| Optionen | MergeOptions | Die Zusammenführungsoptionen. |

### Hinweise

Wenn andere Indizes eine vorherige Version haben, müssen sie aktualisiert werden, bevor sie mit [`IndexUpdater`](../../indexupdater) zusammengeführt werden.

### Beispiele

Das Beispiel zeigt, wie ein Index-Repository in den aktuellen Index zusammengeführt wird.

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

// Alle Indizes im Index-Repository werden in index1 zusammengeführt. Hinweis: index2 und index3 werden nicht geändert.
index1.Merge(repository, options);
```

### Siehe auch

* class [IndexRepository](../../indexrepository)
* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
