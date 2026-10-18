---
title: "Aktualisieren"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Aktualisiert alle Indizes im Repository."
type: docs
weight: 80
url: /de/net/groupdocs.search/indexrepository/update/
---
## Update() {#update}

Aktualisiert alle Indizes im Repository.

```csharp
public void Update()
```

### Beispiele

Das Beispiel demonstriert, wie man Indizes im Repository aktualisiert.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();

Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

// Löschen Sie Dokumente aus dem Dokumentenordner oder ändern Sie sie oder fügen Sie neue Dokumente zum Ordner hinzu

repository.Update();
```

### Siehe auch

* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Aktualisiert alle Indizes im Repository.

```csharp
public void Update(UpdateOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Optionen | UpdateOptions | Die Aktualisierungsoptionen. |

### Beispiele

Das Beispiel demonstriert, wie man Indizes im Repository aktualisiert.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

IndexRepository repository = new IndexRepository();

Index index = repository.Create(indexFolder); // Creating index
index.Add(documentsFolder); // Indexing documents

// Löschen Sie Dokumente aus dem Dokumentenordner oder ändern Sie sie oder fügen Sie neue Dokumente zum Ordner hinzu

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Setting the number of indexing threads
repository.Update(options);
```

### Siehe auch

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [IndexRepository](../../indexrepository)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
