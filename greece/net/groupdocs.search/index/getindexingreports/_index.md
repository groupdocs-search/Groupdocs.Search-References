---
title: GetIndexingReports
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Λαμβάνει τις αναφορές για τις λειτουργίες ευρετηρίασης.
type: docs
weight: 160
url: /el/net/groupdocs.search/index/getindexingreports/
---
## Index.GetIndexingReports method

Λαμβάνει τις αναφορές για τις λειτουργίες ευρετηρίασης.

```csharp
public IndexingReport[] GetIndexingReports()
```

### Επιστρεφόμενη Αξία

Οι αναφορές ευρετηρίασης.

### Παραδείγματα

Το παράδειγμα δείχνει πώς να λαμβάνετε αναφορές ευρετηρίασης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

IndexingReport[] reports = index.GetIndexingReports(); // Λήψη αναφορών ευρετηρίου
```

### Δείτε επίσης

* class [IndexingReport](../../../groupdocs.search.common/indexingreport)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->