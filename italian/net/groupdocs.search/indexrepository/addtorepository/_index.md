---
title: AddToRepository
second_title: GroupDocs.Cerca il riferimento dell'API .NET
description: Aggiunge un indice al repository dellindice.
type: docs
weight: 40
url: /it/net/groupdocs.search/indexrepository/addtorepository/
---
## AddToRepository(Index) {#addtorepository}

Aggiunge un indice al repository dell'indice.

```csharp
public void AddToRepository(Index index)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | Index | Indice da aggiungere. |

### Esempi

L'esempio mostra come aggiungere un indice al repository dell'indice.

```csharp
Index index = new Index();

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(index);
```

### Guarda anche

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* spazio dei nomi [GroupDocs.Search](../../indexrepository)
* assemblea [GroupDocs.Search](../../../)

---

## AddToRepository(string) {#addtorepository_1}

Apre e aggiunge un indice al repository dell'indice.

```csharp
public void AddToRepository(string indexFolder)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indexFolder | String | La cartella indice. |

### Esempi

L'esempio mostra come aggiungere un indice al repository dell'indice.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(indexFolder);
```

### Guarda anche

* class [IndexRepository](../../indexrepository)
* spazio dei nomi [GroupDocs.Search](../../indexrepository)
* assemblea [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->