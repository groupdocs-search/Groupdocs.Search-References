---
title: Update
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Indiziert Dokumente neu die seit der letzten Aktualisierung geändert oder gelöscht wurden. Fügt neue Dateien hinzu die zu den indizierten Ordnern hinzugefügt wurden.
type: docs
weight: 240
url: /de/net/groupdocs.search/index/update/
---
## Update() {#update}

Indiziert Dokumente neu, die seit der letzten Aktualisierung geändert oder gelöscht wurden. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden.

```csharp
public void Update()
```

### Beispiele

Das Beispiel zeigt, wie ein Index aktualisiert wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

// Dokumente aus dem Dokumentenordner löschen oder ändern oder neue Dokumente zum Ordner hinzufügen

index.Update(); // Index aktualisieren
```

### Siehe auch

* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Indiziert Dokumente neu, die seit der letzten Aktualisierung geändert oder gelöscht wurden. Fügt neue Dateien hinzu, die zu den indizierten Ordnern hinzugefügt wurden.

```csharp
public void Update(UpdateOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| options | UpdateOptions | Die Update-Optionen. |

### Beispiele

Das Beispiel zeigt, wie ein Index mit bestimmten Aktualisierungsoptionen aktualisiert wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

// Dokumente aus dem Dokumentenordner löschen oder ändern oder neue Dokumente zum Ordner hinzufügen

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Festlegen der Anzahl der Indizierungsthreads
index.Update(options); // Index aktualisieren
```

### Siehe auch

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->