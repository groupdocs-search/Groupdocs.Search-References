---
title: "AddToRepository"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Ajoute un index au référentiel d'index."
type: docs
weight: 40
url: /fr/net/groupdocs.search/indexrepository/addtorepository/
---
## AddToRepository(Index) {#addtorepository}

Ajoute un index au référentiel d'index.

```csharp
public void AddToRepository(Index index)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| index | Index | L'index à ajouter. |

### Exemples

L'exemple montre comment ajouter un index au référentiel d'index.

```csharp
Index index = new Index();

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(index);
```

### Voir aussi

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## AddToRepository(string) {#addtorepository_1}

Ouvre et ajoute un index au référentiel d'index.

```csharp
public void AddToRepository(string indexFolder)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| indexFolder | String | Le dossier d'index. |

### Exemples

L'exemple montre comment ajouter un index au référentiel d'index.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(indexFolder);
```

### Voir aussi

* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
