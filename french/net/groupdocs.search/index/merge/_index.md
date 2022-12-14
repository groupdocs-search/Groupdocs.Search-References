---
title: Merge
second_title: Référence de l'API GroupDocs.Search pour .NET
description: Fusionne lindex spécifié dans lindex actuel. Notez que lautre index ne sera pas modifié.
type: docs
weight: 190
url: /fr/net/groupdocs.search/index/merge/
---
## Merge(Index, MergeOptions) {#merge}

Fusionne l'index spécifié dans l'index actuel. Notez que l'autre index ne sera pas modifié.

```csharp
public void Merge(Index index, MergeOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| index | Index | L'index dans lequel fusionner. |
| options | MergeOptions | Les options de fusion. |

### Remarques

Si l'autre index a une version précédente, il doit être mis à jour avant de fusionner avec[`IndexUpdater`](../../indexupdater) .

### Exemples

L'exemple montre comment fusionner un index dans l'index actuel.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

Index index1 = new Index(indexFolder1); // Création de l'index1
index1.Add(documentsFolder1); // Indexation des documents

Index index2 = new Index(indexFolder2); // Création de l'index2
index2.Add(documentsFolder2); // Indexation des documents

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Création d'un objet d'annulation

// Fusion de l'index2 dans l'index1. Notez que les fichiers index2 ne seront pas modifiés.
index1.Merge(index2, options);
```

### Voir également

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

---

## Merge(IndexRepository, MergeOptions) {#merge_1}

Fusionne les index du référentiel d'index spécifié dans l'index actuel. Notez que les index du référentiel ne seront pas modifiés.

```csharp
public void Merge(IndexRepository repository, MergeOptions options)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| repository | IndexRepository | Le référentiel d'index dans lequel fusionner. |
| options | MergeOptions | Les options de fusion. |

### Remarques

Si d'autres index ont une version précédente, ils doivent être mis à jour avant de fusionner avec[`IndexUpdater`](../../indexupdater) .

### Exemples

L'exemple montre comment fusionner un référentiel d'index dans l'index actuel.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string indexFolder3 = @"c:\MyIndex3\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index1 = new Index(indexFolder1); // Création de l'index1
index1.Add(documentsFolder1); // Indexation des documents

IndexRepository repository = new IndexRepository(); // Création du référentiel d'index

Index index2 = repository.Create(indexFolder2); // Création de l'index2
index2.Add(documentsFolder2); // Indexation des documents

Index index3 = repository.Create(indexFolder3); // Création de l'index3
index3.Add(documentsFolder3); // Indexation des documents

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Création d'un objet d'annulation

// Fusion de tous les index du référentiel d'index dans index1. Notez que index2 et index3 ne seront pas modifiés.
index1.Merge(repository, options);
```

### Voir également

* class [IndexRepository](../../indexrepository)
* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* espace de noms [GroupDocs.Search](../../index)
* Assemblée [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
