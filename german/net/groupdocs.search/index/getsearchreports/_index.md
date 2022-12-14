---
title: GetSearchReports
second_title: GroupDocs.Suche nach .NET-API-Referenz
description: Ruft die Berichte zu Suchvorgängen ab.
type: docs
weight: 170
url: /de/net/groupdocs.search/index/getsearchreports/
---
## Index.GetSearchReports method

Ruft die Berichte zu Suchvorgängen ab.

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

Index index = new Index(indexFolder); // Index im angegebenen Ordner erstellen
index.Add(documentsFolder); // Indizierung von Dokumenten aus dem angegebenen Ordner

SearchResult result1 = index.Search(query1); // Suchen
SearchResult result2 = index.Search(query2);
SearchResult result3 = index.Search(query1 + " & " + query2);

SearchReport[] reports = index.GetSearchReports(); // Suchberichte abrufen
```

### Siehe auch

* class [SearchReport](../../../groupdocs.search.common/searchreport)
* class [Index](../../index)
* namensraum [GroupDocs.Search](../../index)
* Montage [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
