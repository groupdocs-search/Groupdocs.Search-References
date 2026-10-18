---
title: "Merge"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Fusionne l'index spécifié dans l'index actuel. Notez que l'autre index ne sera pas modifié."
type: docs
weight: 220
url: /fr/net/groupdocs.search/index/merge/
---
## Merge(Index, MergeOptions) {#merge}

Fusionne l'index spécifié dans l'index actuel. Notez que l'autre index ne sera pas modifié.

```csharp
public void Merge(Index index, MergeOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| index | Index | L'index dans lequel fusionner. |
| options | MergeOptions | Les options de fusion. |

### Remarques

Si l'autre index possède une version précédente, il doit être mis à jour avant la fusion avec [`IndexUpdater`](../../indexupdater).

### Exemples

L'exemple montre comment fusionner un index dans l'index actuel.

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

// Fusion de index2 dans index1. Notez que les fichiers de index2 ne seront pas modifiés.
index1.Merge(index2, options);
```

### Voir aussi

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Merge(IndexRepository, MergeOptions) {#merge_1}

Fusionne les index du référentiel d'index spécifié dans l'index actuel. Notez que les index du référentiel ne seront pas modifiés.

```csharp
public void Merge(IndexRepository repository, MergeOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| repository | IndexRepository | Le référentiel d'index dans lequel fusionner. |
| options | MergeOptions | Les options de fusion. |

### Remarques

Si d'autres index ont une version précédente, ils doivent être mis à jour avant la fusion avec [`IndexUpdater`](../../indexupdater).

### Exemples

L'exemple montre comment fusionner un référentiel d'index dans l'index actuel.

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

// Fusion de tous les index du référentiel d'index dans index1. Notez que les index2 et index3 ne seront pas modifiés.
index1.Merge(repository, options);
```

### Voir aussi

* class [IndexRepository](../../indexrepository)
* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
