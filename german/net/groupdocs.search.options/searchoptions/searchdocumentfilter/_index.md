---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Liest oder setzt den Suchdokumentfilter. SearchDocumentFiltergroupdocs.search.options/searchoptions/searchdocumentfilter arbeitet nach der Einschlusslogik. Verwenden Sie die Klasse SearchDocumentFiltergroupdocs.search.options/searchdocumentfilter zur Erstellung von Instanzen des Suchdokumentfilters. Der Standardwert ist null, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden."
type: docs
weight: 100
url: /de/net/groupdocs.search.options/searchoptions/searchdocumentfilter/
---
## SearchOptions.SearchDocumentFilter property

Liest oder setzt den Suchdokumentfilter. `SearchDocumentFilter` arbeitet nach der Einschlusslogik. Verwenden Sie die [`SearchDocumentFilter`](../../searchdocumentfilter) Klasse zur Erstellung von Suchdokumentfilter-Instanzen. Der Standardwert ist `null`, was bedeutet, dass alle gefundenen Dokumente zurückgegeben werden.

```csharp
public ISearchDocumentFilter SearchDocumentFilter { get; set; }
```

### Property Value

Der Suchdokumentfilter.

### Beispiele

Das Beispiel zeigt, wie der Dokumentfilter festgelegt wird.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments1\";

// Erstelle einen Index im angegebenen Ordner
Index index = new Index(indexFolder);

// Indiziere Dokumente
index.Add(documentsFolder);

// Erstellen eines Suchdokumentfilters, der Dokumente mit den Erweiterungen '.doc', '.docx', '.rtf' überspringt
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.CreateNot(fileExtensionFilter); // Inverting file extension filter
options.SearchDocumentFilter = invertedFilter;

// Suche im Index
SearchResult result = index.Search("Einstein", options);
```

### Siehe auch

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
