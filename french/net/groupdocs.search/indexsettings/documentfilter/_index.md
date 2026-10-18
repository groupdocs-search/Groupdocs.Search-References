---
title: "DocumentFilter"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient ou définit un filtre de documents. Le DocumentFiltergroupdocs.search/indexsettings/documentfilter fonctionne selon la logique d'inclusion. Utilisez la classe DocumentFiltergroupdocs.search.options/documentfilter pour créer des instances de filtre de documents. La valeur par défaut est null, ce qui signifie que tous les documents ajoutés sont indexés."
type: docs
weight: 30
url: /fr/net/groupdocs.search/indexsettings/documentfilter/
---
## IndexSettings.DocumentFilter property

Obtient ou définit un filtre de documents. Le `DocumentFilter` fonctionne selon la logique d'inclusion. Utilisez la classe [`DocumentFilter`](../../../groupdocs.search.options/documentfilter) pour créer des instances de filtre de documents. La valeur par défaut est `null`, ce qui signifie que tous les documents ajoutés sont indexés.

```csharp
public DocumentFilter DocumentFilter { get; set; }
```

### Property Value

Le filtre de documents.

### Exemples

L'exemple montre comment définir le filtre de document.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

// Création d'un filtre qui ignore les documents avec les extensions '.doc', '.docx', '.rtf'
IndexSettings settings = new IndexSettings();
DocumentFilter fileExtensionFilter = DocumentFilter.CreateFileExtension(".doc", ".docx", ".rtf"); // Creating file extension filter
DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter); // Inverting file extension filter
settings.DocumentFilter = invertedFilter;

// Création d'un index dans le dossier spécifié
Index index = new Index(indexFolder, settings);

// Indexation des documents
index.Add(documentsFolder);

// Recherche
SearchResult result = index.Search("Einstein");
```

### Voir aussi

* class [DocumentFilter](../../../groupdocs.search.options/documentfilter)
* class [IndexSettings](../../indexsettings)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
