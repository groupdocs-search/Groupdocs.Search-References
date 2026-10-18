---
title: "GetIndexingReports"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient les rapports sur les opérations d'indexation."
type: docs
weight: 190
url: /fr/net/groupdocs.search/index/getindexingreports/
---
## Index.GetIndexingReports method

Obtient les rapports sur les opérations d'indexation.

```csharp
public IndexingReport[] GetIndexingReports()
```

### Valeur de retour

Les rapports d'indexation.

### Exemples

L'exemple montre comment obtenir les rapports d'indexation.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

IndexingReport[] reports = index.GetIndexingReports(); // Getting indexing reports
```

### Voir aussi

* class [IndexingReport](../../../groupdocs.search.common/indexingreport)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
