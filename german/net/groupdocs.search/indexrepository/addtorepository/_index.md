---
title: "AddToRepository"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Fügt dem Index-Repository einen Index hinzu."
type: docs
weight: 40
url: /de/net/groupdocs.search/indexrepository/addtorepository/
---
## AddToRepository(Index) {#addtorepository}

Fügt dem Index-Repository einen Index hinzu.

```csharp
public void AddToRepository(Index index)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| index | Index | Der hinzuzufügende Index. |

### Beispiele

Das Beispiel zeigt, wie ein Index zum Index-Repository hinzugefügt wird.

```csharp
Index index = new Index();

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(index);
```

### Siehe auch

* class [Index](../../index)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## AddToRepository(string) {#addtorepository_1}

Öffnet und fügt dem Index-Repository einen Index hinzu.

```csharp
public void AddToRepository(string indexFolder)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| indexFolder | String | Der Indexordner. |

### Beispiele

Das Beispiel zeigt, wie ein Index zum Index-Repository hinzugefügt wird.

```csharp
string indexFolder = @"c:\MyIndex\";

IndexRepository indexRepository = new IndexRepository();

indexRepository.AddToRepository(indexFolder);
```

### Siehe auch

* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
