---
title: AddToRepository
second_title: GroupDocs.Search efter .NET API Reference
description: Lägger till ett index i indexförrådet.
type: docs
weight: 40
url: /sv/net/groupdocs.search/indexrepository/addtorepository/
---
## AddToRepository(Index) {#addtorepository}

Lägger till ett index i indexförrådet.

```csharp
public void AddToRepository(Index index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Index | Indexet att lägga till. |

### Exempel

Exemplet visar hur man lägger till ett index i indexförrådet.

```csharp
Index index = new Index();

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(index);
```

### Se även

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namnutrymme [GroupDocs.Search](../../indexrepository)
* hopsättning [GroupDocs.Search](../../../)

---

## AddToRepository(string) {#addtorepository_1}

Öppnar och lägger till ett index i indexförrådet.

```csharp
public void AddToRepository(string indexFolder)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| indexFolder | String | Indexmappen. |

### Exempel

Exemplet visar hur man lägger till ett index i indexförrådet.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(indexFolder);
```

### Se även

* class [IndexRepository](../../indexrepository)
* namnutrymme [GroupDocs.Search](../../indexrepository)
* hopsättning [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
