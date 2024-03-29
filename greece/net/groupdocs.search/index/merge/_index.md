---
title: Merge
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Συγχωνεύει το καθορισμένο ευρετήριο στο τρέχον ευρετήριο. Σημειώστε ότι το άλλο ευρετήριο δεν θα αλλάξει.
type: docs
weight: 190
url: /el/net/groupdocs.search/index/merge/
---
## Merge(Index, MergeOptions) {#merge}

Συγχωνεύει το καθορισμένο ευρετήριο στο τρέχον ευρετήριο. Σημειώστε ότι το άλλο ευρετήριο δεν θα αλλάξει.

```csharp
public void Merge(Index index, MergeOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | Index | Το ευρετήριο για συγχώνευση. |
| options | MergeOptions | Οι επιλογές συγχώνευσης. |

### Παρατηρήσεις

Εάν το άλλο ευρετήριο έχει προηγούμενη έκδοση, πρέπει να ενημερωθεί πριν από τη συγχώνευση[`IndexUpdater`](../../indexupdater) .

### Παραδείγματα

Το παράδειγμα δείχνει πώς να συγχωνεύσετε ένα ευρετήριο στο τρέχον ευρετήριο.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";

Index index1 = new Index(indexFolder1); // Δημιουργία ευρετηρίου1
index1.Add(documentsFolder1); // Ευρετηρίαση εγγράφων

Index index2 = new Index(indexFolder2); // Δημιουργία ευρετηρίου2
index2.Add(documentsFolder2); // Ευρετηρίαση εγγράφων

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Δημιουργία αντικειμένου ακύρωσης

// Συγχώνευση του δείκτη2 στο δείκτη1. Σημειώστε ότι τα αρχεία index2 δεν θα αλλάξουν.
index1.Merge(index2, options);
```

### Δείτε επίσης

* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Merge(IndexRepository, MergeOptions) {#merge_1}

Συγχωνεύει ευρετήρια από το καθορισμένο χώρο αποθήκευσης ευρετηρίου στο τρέχον ευρετήριο. Σημειώστε ότι τα ευρετήρια στο χώρο αποθήκευσης δεν θα αλλάξουν.

```csharp
public void Merge(IndexRepository repository, MergeOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| repository | IndexRepository | Το αποθετήριο ευρετηρίου για συγχώνευση. |
| options | MergeOptions | Οι επιλογές συγχώνευσης. |

### Παρατηρήσεις

Εάν άλλα ευρετήρια έχουν προηγούμενη έκδοση, πρέπει να ενημερωθούν πριν από τη συγχώνευση[`IndexUpdater`](../../indexupdater) .

### Παραδείγματα

Το παράδειγμα δείχνει πώς να συγχωνεύσετε ένα αποθετήριο ευρετηρίου στο τρέχον ευρετήριο.

```csharp
string indexFolder1 = @"c:\MyIndex1\";
string indexFolder2 = @"c:\MyIndex2\";
string indexFolder3 = @"c:\MyIndex3\";
string documentsFolder1 = @"c:\MyDocuments1\";
string documentsFolder2 = @"c:\MyDocuments2\";
string documentsFolder3 = @"c:\MyDocuments3\";

Index index1 = new Index(indexFolder1); // Δημιουργία ευρετηρίου1
index1.Add(documentsFolder1); // Ευρετηρίαση εγγράφων

IndexRepository repository = new IndexRepository(); // Δημιουργία αποθετηρίου ευρετηρίου

Index index2 = repository.Create(indexFolder2); // Δημιουργία ευρετηρίου2
index2.Add(documentsFolder2); // Ευρετηρίαση εγγράφων

Index index3 = repository.Create(indexFolder3); // Δημιουργία ευρετηρίου3
index3.Add(documentsFolder3); // Ευρετηρίαση εγγράφων

MergeOptions options = new MergeOptions();
options.Cancellation = new Cancellation(); // Δημιουργία αντικειμένου ακύρωσης

// Συγχώνευση όλων των ευρετηρίων στο αποθετήριο ευρετηρίου στο index1. Σημειώστε ότι το index2 και το index3 δεν θα αλλάξουν.
index1.Merge(repository, options);
```

### Δείτε επίσης

* class [IndexRepository](../../indexrepository)
* class [MergeOptions](../../../groupdocs.search.options/mergeoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
