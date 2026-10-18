---
title: "Optimiser"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche."
type: docs
weight: 240
url: /fr/net/groupdocs.search/index/optimize/
---
## Optimize() {#optimize}

Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche.

```csharp
public void Optimize()
```

### Exemples

L'exemple montre comment fusionner les segments d'un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creating index in the specified folder

index.Add(documentsFolder1); // Indexing documents from the specified folder
index.Add(documentsFolder2); // Each call to Add creates at least one new segment in the index
index.Add(documentsFolder3);

// Fusion des segments de l'index
index.Optimize();
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Optimize(MergeOptions) {#optimize_1}

Réduit le nombre de segments d'index en les fusionnant les uns avec les autres. Cette opération améliore les performances de recherche.

```csharp
public void Optimize(MergeOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | MergeOptions | Les options de fusion. |

### Exemples

L'exemple montre comment fusionner les segments d'un index avec des options de fusion particulières.

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

// Fusion des segments de l'index
index.Optimize(options); // This method will return before the operation is completed

options.Cancellation.CancelAfter(10000); // Setting maximum duration of the operation to 10 seconds
```

### Voir aussi

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
