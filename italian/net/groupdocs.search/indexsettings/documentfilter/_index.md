---
title: "DocumentFilter"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene o imposta un filtro documento. Il DocumentFiltergroupdocs.search/indexsettings/documentfilter funziona con la logica di inclusione. Usa la classe DocumentFiltergroupdocs.search.options/documentfilter per creare istanze di filtro documento. Il valore predefinito è null, il che significa che tutti i documenti aggiunti vengono indicizzati."
type: docs
weight: 30
url: /it/net/groupdocs.search/indexsettings/documentfilter/
---
## IndexSettings.DocumentFilter property

Ottiene o imposta un filtro documento. Il `DocumentFilter` funziona con la logica di inclusione. Usa la classe [`DocumentFilter`](../../../groupdocs.search.options/documentfilter) per creare istanze di filtro documento. Il valore predefinito è `null`, il che significa che tutti i documenti aggiunti vengono indicizzati.

```csharp
public DocumentFilter DocumentFilter { get; set; }
```

### Property Value

Il filtro documento.

### Esempi

L'esempio dimostra come impostare il filtro documento.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Creazione di un filtro che ignora i documenti con estensioni '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter); // Inverting file extension filter
settings.DocumentFilter = invertedFilter;

// Creazione di un indice nella cartella specificata
Index index = new Index(indexFolder, settings);

// Indicizzazione dei documenti
index.Add(documentsFolder);

// Ricerca
SearchResult result = index.Search("Einstein");
```

### Vedi anche

* class [DocumentFilter](../../../groupdocs.search.options/documentfilter)
* class [IndexSettings](../../indexsettings)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
