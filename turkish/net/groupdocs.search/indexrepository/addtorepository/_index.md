---
title: AddToRepository
second_title: .NET API Başvurusu için GroupDocs.Search
description: Dizin deposuna bir dizin ekler.
type: docs
weight: 40
url: /tr/net/groupdocs.search/indexrepository/addtorepository/
---
## AddToRepository(Index) {#addtorepository}

Dizin deposuna bir dizin ekler.

```csharp
public void AddToRepository(Index index)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| index | Index | Eklenecek dizin. |

### Örnekler

Örnek, dizin deposuna nasıl dizin ekleneceğini gösterir.

```csharp
Index index = new Index();

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(index);
```

### Ayrıca bakınız

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* ad alanı [GroupDocs.Search](../../indexrepository)
* toplantı [GroupDocs.Search](../../../)

---

## AddToRepository(string) {#addtorepository_1}

Açar ve dizin deposuna bir dizin ekler.

```csharp
public void AddToRepository(string indexFolder)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| indexFolder | String | Dizin klasörü. |

### Örnekler

Örnek, dizin deposuna nasıl dizin ekleneceğini gösterir.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(indexFolder);
```

### Ayrıca bakınız

* class [IndexRepository](../../indexrepository)
* ad alanı [GroupDocs.Search](../../indexrepository)
* toplantı [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->