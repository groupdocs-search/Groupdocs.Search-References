---
title: "GetSearchReports"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene i report sulle operazioni di ricerca."
type: docs
weight: 200
url: /it/net/groupdocs.search/index/getsearchreports/
---
## Index.GetSearchReports method

Ottiene i report sulle operazioni di ricerca.

```csharp
public SearchReport[] GetSearchReports()
```

### Valore di ritorno

I report di ricerca.

### Esempi

L'esempio dimostra come ottenere i report di ricerca.

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

### Vedi anche

* class [SearchReport](../../../groupdocs.search.common/searchreport)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
