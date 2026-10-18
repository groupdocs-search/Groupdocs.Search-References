---
title: "GetSearchReports"
second_title: "Référence API de GroupDocs.Search pour .NET"
description: "Obtient les rapports sur les opérations de recherche."
type: docs
weight: 200
url: /fr/net/groupdocs.search/index/getsearchreports/
---
## Index.GetSearchReports method

Obtient les rapports sur les opérations de recherche.

```csharp
public SearchReport[] GetSearchReports()
```

### Valeur de retour

Les rapports de recherche.

### Exemples

L'exemple montre comment obtenir les rapports de recherche.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";
string query1 = "Einstein";
string query2 = "Newton";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

SearchResult result1 = index.Search(query1); // Searching
SearchResult result2 = index.Search(query2);
SearchResult result3 = index.Search(query1 + " & " + query2);

SearchReport[] reports = index.GetSearchReports(); // Getting search reports
```

### Voir aussi

* class [SearchReport](../../../groupdocs.search.common/searchreport)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.search.dll -->
