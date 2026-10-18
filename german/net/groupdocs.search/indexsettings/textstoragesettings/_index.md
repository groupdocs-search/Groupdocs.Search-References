---
title: "TextStorageSettings"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Liest oder setzt die Texteinstellungen für die Speicherung. Der Standardwert ist null, was bedeutet, dass Dokumenttexte nicht gespeichert werden."
type: docs
weight: 100
url: /de/net/groupdocs.search/indexsettings/textstoragesettings/
---
## IndexSettings.TextStorageSettings property

Ruft die Einstellungen für die Textspeicherung ab oder legt sie fest. Der Standardwert ist `null`, was bedeutet, dass Dokumenttexte nicht gespeichert werden.

```csharp
public TextStorageSettings TextStorageSettings { get; set; }
```

### Property Value

Die Texteinstellungen für die Speicherung.

### Beispiele

Das Beispiel zeigt, wie die Texteinstellungen für die Speicherung festgelegt werden.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen einer Indexeinstellungsinstanz
IndexSettings settings = new IndexSettings();
settings.TextStorageSettings = new TextStorageSettings(Compression.High); // Setting high compression level for the index text storage

// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder, settings);

// Indiziere Dokumente
index.Add(documentsFolder);

// Suche
SearchResult result = index.Search("Einstein");
```

### Siehe auch

* class [TextStorageSettings](../../../groupdocs.search.options/textstoragesettings)
* class [IndexSettings](../../indexsettings)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
