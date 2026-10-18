---
title: "Add"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Εκτελεί λειτουργία ευρετηρίου. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν."
type: docs
weight: 80
url: /el/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Εκτελεί λειτουργία ευρετηρίου. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string path)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς ένα αρχείο ή φάκελο που θα ευρετηριαστεί. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder
index.Add(folderPath); // Indexing documents in the specified folder
index.Add(filePath); // Indexing the specified document
```

### Δείτε επίσης

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Εκτελεί λειτουργία ευρετηρίου. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string path, IndexingOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς ένα αρχείο ή φάκελο που θα ευρετηριαστεί. |
| επιλογές | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο με συγκεκριμένες επιλογές ευρετηρίασης.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
index.Add(folderPath, options); // Indexing documents in the specified folder
index.Add(filePath, options); // Indexing the specified document
```

### Δείτε επίσης

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Εκτελεί λειτουργία ευρετηρίου. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string[] paths)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| paths | String[] | Οι διαδρομές προς αρχεία ή φακέλους που θα ευρετηριαστούν. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Indexing documents at the specified paths
```

### Δείτε επίσης

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Εκτελεί λειτουργία ευρετηρίου. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| paths | String[] | Οι διαδρομές προς αρχεία ή φακέλους που θα ευρετηριαστούν. |
| επιλογές | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο με συγκεκριμένες επιλογές ευρετηρίασης.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Creating index in the specified folder

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Setting the number of indexing threads
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Indexing documents at the specified paths
```

### Δείτε επίσης

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Εκτελεί λειτουργία ευρετηρίου. Προσθέτει έγγραφα από σύστημα αρχείων, ροή ή δομή.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| έγγραφα | Document[] | Τα έγγραφα από το σύστημα αρχείων, τη ροή ή τη δομή. |
| επιλογές | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Δείτε επίσης

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Εκτελεί λειτουργία ευρετηρίου. Προσθέτει τα εξαγόμενα δεδομένα στο ευρετήριο.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| δεδομένα | ExtractedData[] | Τα εξαγόμενα δεδομένα. |
| επιλογές | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Δείτε επίσης

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
