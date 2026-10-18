---
title: "GetSearchReports"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Gibt die Berichte zu Suchvorgängen zurück."
type: docs
weight: 200
url: /de/net/groupdocs.search/index/getsearchreports/
---
## Index.GetSearchReports method

Gibt die Berichte zu Suchvorgängen zurück.

```csharp
public SearchReport[] GetSearchReports()
```

### Rückgabewert

Die Suchberichte.

### Beispiele

Das Beispiel zeigt, wie Suchberichte abgerufen werden.

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

### Siehe auch

* class [SearchReport](../../../groupdocs.search.common/searchreport)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
