---
title: "GetIndexingReports"
second_title: "GroupDocs.Search per .NET Riferimento API"
description: "Ottiene i report sulle operazioni di indicizzazione."
type: docs
weight: 190
url: /it/net/groupdocs.search/index/getindexingreports/
---
## Index.GetIndexingReports method

Ottiene i report sulle operazioni di indicizzazione.

```csharp
public IndexingReport[] GetIndexingReports()
```

### Valore di ritorno

I report di indicizzazione.

### Esempi

L'esempio dimostra come ottenere i report di indicizzazione.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(documentsFolder); // Indexing documents from the specified folder

IndexingReport[] reports = index.GetIndexingReports(); // Getting indexing reports
```

### Vedi anche

* class [IndexingReport](../../../groupdocs.search.common/indexingreport)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NON MODIFICARE: generato da xmldocmd per GroupDocs.search.dll -->
