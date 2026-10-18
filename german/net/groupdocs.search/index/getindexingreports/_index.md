---
title: "GetIndexingReports"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Gibt die Berichte zu Indexierungsvorgängen zurück."
type: docs
weight: 190
url: /de/net/groupdocs.search/index/getindexingreports/
---
## Index.GetIndexingReports method

Gibt die Berichte zu Indexierungsvorgängen zurück.

```csharp
public IndexingReport[] GetIndexingReports()
```

### Rückgabewert

Die Indexierungsberichte.

### Beispiele

Das Beispiel zeigt, wie man Indexierungsberichte abruft.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

IndexingReport[] reports = index.GetIndexingReports(); // Getting indexing reports
```

### Siehe auch

* class [IndexingReport](../../../groupdocs.search.common/indexingreport)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
