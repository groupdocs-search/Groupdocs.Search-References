---
title: Update
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Herindexeert documenten die zijn gewijzigd of verwijderd sinds de laatste update. Voegt nieuwe bestanden toe die zijn toegevoegd aan de geïndexeerde mappen.
type: docs
weight: 240
url: /nl/net/groupdocs.search/index/update/
---
## Update() {#update}

Herindexeert documenten die zijn gewijzigd of verwijderd sinds de laatste update. Voegt nieuwe bestanden toe die zijn toegevoegd aan de geïndexeerde mappen.

```csharp
public void Update()
```

### Voorbeelden

Het voorbeeld laat zien hoe u een index bijwerkt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

// Verwijder documenten uit de documentenmap of wijzig ze of voeg nieuwe documenten toe aan de map

index.Update(); // De index bijwerken
```

### Zie ook

* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Herindexeert documenten die zijn gewijzigd of verwijderd sinds de laatste update. Voegt nieuwe bestanden toe die zijn toegevoegd aan de geïndexeerde mappen.

```csharp
public void Update(UpdateOptions options)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| options | UpdateOptions | De update-opties. |

### Voorbeelden

Het voorbeeld laat zien hoe u een index bijwerkt met bepaalde update-opties.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index maken in de opgegeven map
index.Add(documentsFolder); // Documenten uit de opgegeven map indexeren

// Verwijder documenten uit de documentenmap of wijzig ze of voeg nieuwe documenten toe aan de map

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Het aantal indexthreads instellen
index.Update(options); // De index bijwerken
```

### Zie ook

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* naamruimte [GroupDocs.Search](../../index)
* montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->