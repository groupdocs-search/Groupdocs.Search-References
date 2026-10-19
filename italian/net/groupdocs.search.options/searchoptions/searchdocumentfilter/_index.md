---
title: "SearchDocumentFilter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene o imposta il filtro documento di ricerca. SearchDocumentFiltergroupdocs.search.options/searchoptions/searchdocumentfilter funziona con la logica di inclusione. Utilizzare la classe SearchDocumentFiltergroupdocs.search.options/searchdocumentfilter per creare istanze del filtro documento di ricerca. Il valore predefinito è null, il che significa che verranno restituiti tutti i documenti trovati."
type: docs
weight: 100
url: /it/net/groupdocs.search.options/searchoptions/searchdocumentfilter/
---
## SearchOptions.SearchDocumentFilter property

Ottiene o imposta il filtro del documento di ricerca. `SearchDocumentFilter` funziona con la logica di inclusione. Utilizzare la classe [`SearchDocumentFilter`](../../searchdocumentfilter) per creare istanze del filtro del documento di ricerca. Il valore predefinito è `null`, il che significa che verranno restituiti tutti i documenti trovati.

```csharp
public ISearchDocumentFilter SearchDocumentFilter { get; set; }
```

### Property Value

Il filtro del documento di ricerca.

### Esempi

L'esempio dimostra come impostare il filtro documento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments1\";

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder);

// Indicizzazione dei documenti
index.Add(documentsFolder);

// Creazione di un filtro documento di ricerca che ignora i documenti con estensioni '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.CreateNot(fileExtensionFilter); // Inverting file extension filter
options.SearchDocumentFilter = invertedFilter;

// Cerca nell'indice
SearchResult result = index.Search("Einstein", options);
```

### Vedi anche

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
