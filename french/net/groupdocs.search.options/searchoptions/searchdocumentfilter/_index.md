---
title: "SearchDocumentFilter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient ou définit le filtre de document de recherche. SearchDocumentFiltergroupdocs.search.options/searchoptions/searchdocumentfilter fonctionne selon la logique d'inclusion. Utilisez la classe SearchDocumentFiltergroupdocs.search.options/searchdocumentfilter pour créer des instances de filtre de document de recherche. La valeur par défaut est null, ce qui signifie que tous les documents trouvés seront retournés."
type: docs
weight: 100
url: /fr/net/groupdocs.search.options/searchoptions/searchdocumentfilter/
---
## SearchOptions.SearchDocumentFilter property

Obtient ou définit le filtre de document de recherche. `SearchDocumentFilter` fonctionne selon la logique d'inclusion. Utilisez la classe [`SearchDocumentFilter`](../../searchdocumentfilter) pour créer des instances de filtre de document de recherche. La valeur par défaut est `null`, ce qui signifie que tous les documents trouvés seront retournés.

```csharp
public ISearchDocumentFilter SearchDocumentFilter { get; set; }
```

### Property Value

Le filtre de document de recherche.

### Exemples

L'exemple montre comment définir le filtre de document.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments1\";

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder);

// Indexation des documents
index.Add(documentsFolder);

// Création d'un filtre de document de recherche qui ignore les documents avec les extensions '.doc', '.docx', '.rtf'
SearchOptions options = new SearchOptions();
ISearchDocumentFilter fileExtensionFilter = SearchDocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
ISearchDocumentFilter invertedFilter = SearchDocumentFilter.CreateNot(fileExtensionFilter); // Inverting file extension filter
options.SearchDocumentFilter = invertedFilter;

// Recherche dans l'index
SearchResult result = index.Search("Einstein", options);
```

### Voir aussi

* interface [ISearchDocumentFilter](../../isearchdocumentfilter)
* class [SearchOptions](../../searchoptions)
* namespace [GroupDocs.Search.Options](../../../groupdocs.search.options)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
