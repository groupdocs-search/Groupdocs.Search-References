---
title: Add
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.
type: docs
weight: 70
url: /el/net/groupdocs.search/index/add/
---
## Add(string) {#add_2}

Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string path)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς ένα αρχείο ή φάκελο προς ευρετηρίαση. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(folderPath); // Δημιουργία ευρετηρίου εγγράφων στον καθορισμένο φάκελο
index.Add(filePath); // Ευρετηρίαση του καθορισμένου εγγράφου
```

### Δείτε επίσης

* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Add(string, IndexingOptions) {#add_3}

Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει ένα αρχείο ή φάκελο με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string path, IndexingOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή προς ένα αρχείο ή φάκελο προς ευρετηρίαση. |
| options | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέτετε έγγραφα σε ένα ευρετήριο με συγκεκριμένες επιλογές ευρετηρίασης.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Ρύθμιση του αριθμού των νημάτων ευρετηρίασης
index.Add(folderPath, options); // Δημιουργία ευρετηρίου εγγράφων στον καθορισμένο φάκελο
index.Add(filePath, options); // Ευρετηρίαση του καθορισμένου εγγράφου
```

### Δείτε επίσης

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Add(string[]) {#add_4}

Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string[] paths)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| paths | String[] | Οι διαδρομές σε αρχεία ή φακέλους προς ευρετηρίαση. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέσετε έγγραφα σε ένα ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο

string[] paths = new string[] { folderPath, filePath };
index.Add(paths); // Ευρετηρίαση εγγράφων στις καθορισμένες διαδρομές
```

### Δείτε επίσης

* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Add(string[], IndexingOptions) {#add_5}

Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει αρχεία ή φακέλους με απόλυτη ή σχετική διαδρομή. Τα έγγραφα από όλους τους υποφακέλους θα ευρετηριαστούν.

```csharp
public void Add(string[] paths, IndexingOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| paths | String[] | Οι διαδρομές σε αρχεία ή φακέλους προς ευρετηρίαση. |
| options | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να προσθέτετε έγγραφα σε ένα ευρετήριο με συγκεκριμένες επιλογές ευρετηρίασης.

```csharp
string indexFolder = @"c:\MyIndex\";
string folderPath = @"c:\MyDocuments\";
string filePath = @"c:\Documents\MyFile.txt";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο

IndexingOptions options = new IndexingOptions();
options.Threads = 2; // Ρύθμιση του αριθμού των νημάτων ευρετηρίασης
string[] paths = new string[] { folderPath, filePath };
index.Add(paths, options); // Ευρετηρίαση εγγράφων στις καθορισμένες διαδρομές
```

### Δείτε επίσης

* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Add(Document[], IndexingOptions) {#add}

Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει έγγραφα από σύστημα αρχείων, ροή ή δομή.

```csharp
public void Add(Document[] documents, IndexingOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| documents | Document[] | Τα έγγραφα από σύστημα αρχείων, ροή ή δομή. |
| options | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Δείτε επίσης

* class [Document](../../../groupdocs.search.common/document)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Add(ExtractedData[], IndexingOptions) {#add_1}

Εκτελεί λειτουργία ευρετηρίασης. Προσθέτει τα εξαγόμενα δεδομένα στο ευρετήριο.

```csharp
public void Add(ExtractedData[] data, IndexingOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| data | ExtractedData[] | Τα εξαγόμενα δεδομένα. |
| options | IndexingOptions | Οι επιλογές ευρετηρίασης. |

### Δείτε επίσης

* class [ExtractedData](../../../groupdocs.search.common/extracteddata)
* class [IndexingOptions](../../../groupdocs.search.options/indexingoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
