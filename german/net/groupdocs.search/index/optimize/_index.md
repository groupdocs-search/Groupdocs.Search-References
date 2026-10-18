---
title: "Optimieren"
second_title: "GroupDocs.Search für .NET API-Referenz"
description: "Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung."
type: docs
weight: 240
url: /de/net/groupdocs.search/index/optimize/
---
## Optimize() {#optimize}

Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung.

```csharp
public void Optimize()
```

### Beispiele

Das Beispiel demonstriert, wie man Segmente eines Index zusammenführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creating index in the specified folder

index.Add(documentsFolder1); // Indexing documents from the specified folder
index.Add(documentsFolder2); // Each call to Add creates at least one new segment in the index
index.Add(documentsFolder3);

// Zusammenführen von Segmenten des Index
index.Optimize();
```

### Siehe auch

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Optimize(MergeOptions) {#optimize_1}

Minimiert die Anzahl der Indexsegmente, indem sie miteinander zusammengeführt werden. Dieser Vorgang verbessert die Suchleistung.

```csharp
public void Optimize(MergeOptions options)
```

| Parameter | Type | Beschreibung |
| --- | --- | --- |
| Optionen | MergeOptions | Die Zusammenführungsoptionen. |

### Beispiele

Das Beispiel demonstriert, wie man Segmente eines Index mit bestimmten Merge-Optionen zusammenführt.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index = new Index(indexFolder); // Creating index in the specified folder

index.Add(documentsFolder1); // Indexing documents from the specified folder
index.Add(documentsFolder2); // Each call to Add creates at least one new segment in the index
index.Add(documentsFolder3);

MergeOptions options = new MergeOptions();
options.IsAsync = true; // Asynchronous operation
options.Cancellation = new Cancellation(); // Creating cancellation object

// Zusammenführen von Segmenten des Index
index.Optimize(options); // This method will return before the operation is completed

options.Cancellation.CancelAfter(10000); // Setting maximum duration of the operation to 10 seconds
```

### Siehe auch

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- NICHT BEARBEITEN: generiert von xmldocmd für GroupDocs.search.dll -->
