---
title: "DocumentFilter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Liest oder setzt einen Dokumentfilter. Der DocumentFiltergroupdocs.search/indexsettings/documentfilter arbeitet nach der Einschlusslogik. Verwenden Sie die DocumentFiltergroupdocs.search.options/documentfilter-Klasse zur Erstellung von Dokumentfilter-Instanzen. Der Standardwert ist null, was bedeutet, dass alle hinzugefügten Dokumente indexiert werden."
type: docs
weight: 30
url: /de/net/groupdocs.search/indexsettings/documentfilter/
---
## IndexSettings.DocumentFilter property

Liest oder setzt einen Dokumentfilter. Der `DocumentFilter` arbeitet nach der Einschlusslogik. Verwenden Sie die [`DocumentFilter`](../../../groupdocs.search.options/documentfilter)-Klasse zur Erstellung von Dokumentfilter-Instanzen. Der Standardwert ist `null`, was bedeutet, dass alle hinzugefügten Dokumente indexiert werden.

```csharp
public DocumentFilter DocumentFilter { get; set; }
```

### Property Value

Der Dokumentfilter.

### Beispiele

Das Beispiel zeigt, wie der Dokumentfilter festgelegt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Erstellen eines Filters, der Dokumente mit den Erweiterungen '.doc', '.docx', '.rtf' überspringt
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter); // Inverting file extension filter
settings.DocumentFilter = invertedFilter;

// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder, settings);

// Indiziere Dokumente
index.Add(documentsFolder);

// Suche
SearchResult result = index.Search("Einstein");
```

### Siehe auch

* class [DocumentFilter](../../../groupdocs.search.options/documentfilter)
* class [IndexSettings](../../indexsettings)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
