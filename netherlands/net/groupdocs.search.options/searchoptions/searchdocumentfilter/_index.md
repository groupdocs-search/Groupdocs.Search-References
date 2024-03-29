---
title: SearchDocumentFilter
second_title: GroupDocs. Zoek naar .NET API-referentie
description: Haalt of stelt het zoekdocumentfilter in. SearchDocumentFiltergroupdocs.search.options/searchoptions/searchdocumentfilter werkt op de integratielogica. GebruikSearchDocumentFiltergroupdocs.search.options/searchdocumentfilter klasse voor het maken van een zoekdocument filterinstanties. De standaardwaarde isnul  wat betekent dat alle gevonden documenten worden geretourneerd.
type: docs
weight: 90
url: /nl/net/groupdocs.search.options/searchoptions/searchdocumentfilter/
---
## SearchOptions.SearchDocumentFilter property

Haalt of stelt het zoekdocumentfilter in. `SearchDocumentFilter` werkt op de integratielogica. Gebruik[`SearchDocumentFilter`](../../searchdocumentfilter) klasse voor het maken van een zoekdocument filterinstanties. De standaardwaarde is`nul` , wat betekent dat alle gevonden documenten worden geretourneerd.

```csharp
public ISearchDocumentFilter SearchDocumentFilter { get; set; }
```

### Eigendoms-waarde

Het zoekdocumentfilter.

### Voorbeelden

Het voorbeeld laat zien hoe u het documentfilter instelt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments1\";

// Een index maken in de opgegeven map
Index index = new Index(indexFolder);

// Documenten indexeren
index.Add(documentsFolder);

// Een zoekdocumentfilter maken dat documenten met de extensie '.doc', '.docx', '.rtf' overslaat
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Bestandsextensiefilter maken
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.CreateNot(fileExtensionFilter); // Bestandsextensiefilter omkeren
options.SearchDocumentFilter = invertedFilter;

// Zoeken in index
SearchResult result = index.Search("Einstein", options);
```

### Zie ook

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchOptions](../../searchoptions)
* naamruimte [GroupDocs.Search.Options](../../searchoptions)
* montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
