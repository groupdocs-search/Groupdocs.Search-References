---
title: "Mettre à jour"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Met à jour tous les index du référentiel."
type: docs
weight: 80
url: /fr/net/groupdocs.search/indexrepository/update/
---
## Update() {#update}

Met à jour tous les index du référentiel.

```csharp
public void Update()
```

### Exemples

L'exemple montre comment mettre à jour les index dans le référentiel.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();

Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

// Supprimer des documents du dossier documents ou les modifier ou ajouter de nouveaux documents au dossier

repository.Update();
```

### Voir aussi

* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Met à jour tous les index du référentiel.

```csharp
public void Update(UpdateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | UpdateOptions | Les options de mise à jour. |

### Exemples

L'exemple montre comment mettre à jour les index dans le référentiel.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();

Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

// Supprimer des documents du dossier documents ou les modifier ou ajouter de nouveaux documents au dossier

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Setting the number of indexing threads
repository.Update(options);
```

### Voir aussi

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
