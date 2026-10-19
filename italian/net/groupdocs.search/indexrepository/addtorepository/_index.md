---
title: "AddToRepository"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Aggiunge un indice al repository degli indici."
type: docs
weight: 40
url: /it/net/groupdocs.search/indexrepository/addtorepository/
---
## AddToRepository(Index) {#addtorepository}

Aggiunge un indice al repository degli indici.

```csharp
public void AddToRepository(Index index)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| index | Index | L'indice da aggiungere. |

### Esempi

L'esempio dimostra come aggiungere un indice al index repository.

```csharp
Index index = new Index();

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(index);
```

### Vedi anche

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## AddToRepository(string) {#addtorepository_1}

Apre e aggiunge un indice al repository degli indici.

```csharp
public void AddToRepository(string indexFolder)
```

| Parameter | Type | Descrizione |
| --- | --- | --- |
| indexFolder | String | La cartella dell'indice. |

### Esempi

L'esempio dimostra come aggiungere un indice al index repository.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(indexFolder);
```

### Vedi anche

* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
