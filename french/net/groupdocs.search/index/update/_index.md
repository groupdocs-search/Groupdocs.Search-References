---
title: "Mettre à jour"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Réindexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute les nouveaux fichiers qui ont été ajoutés aux dossiers indexés."
type: docs
weight: 280
url: /fr/net/groupdocs.search/index/update/
---
## Update() {#update}

Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute les nouveaux fichiers qui ont été ajoutés aux dossiers indexés.

```csharp
public void Update()
```

### Exemples

L'exemple montre comment mettre à jour un index.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Supprimer des documents du dossier documents ou les modifier ou ajouter de nouveaux documents au dossier

index.Update(); // Updating the index
```

### Voir aussi

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Ré-indexe les documents qui ont été modifiés ou supprimés depuis la dernière mise à jour. Ajoute les nouveaux fichiers qui ont été ajoutés aux dossiers indexés.

```csharp
public void Update(UpdateOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| options | UpdateOptions | Les options de mise à jour. |

### Exemples

L'exemple montre comment mettre à jour un index avec des options de mise à jour particulières.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Supprimer des documents du dossier documents ou les modifier ou ajouter de nouveaux documents au dossier

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Update(options); // Updating the index
```

### Voir aussi

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
