---
title: "Aktualisieren"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden."
type: docs
weight: 280
url: /de/net/groupdocs.search/index/update/
---
## Update() {#update}

Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden.

```csharp
public void Update()
```

### Beispiele

Das Beispiel zeigt, wie man einen Index aktualisiert.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Löschen Sie Dokumente aus dem Dokumentenordner oder ändern Sie sie oder fügen Sie neue Dokumente zum Ordner hinzu

index.Update(); // Updating the index
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Indiziert Dokumente, die seit dem letzten Update geändert oder gelöscht wurden, neu. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden.

```csharp
public void Update(UpdateOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Optionen | UpdateOptions | Die Aktualisierungsoptionen. |

### Beispiele

Das Beispiel zeigt, wie man einen Index mit bestimmten Aktualisierungsoptionen aktualisiert.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

// Löschen Sie Dokumente aus dem Dokumentenordner oder ändern Sie sie oder fügen Sie neue Dokumente zum Ordner hinzu

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Update(options); // Updating the index
```

### Siehe auch

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
