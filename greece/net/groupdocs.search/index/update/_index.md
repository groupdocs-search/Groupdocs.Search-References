---
title: Update
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Δημιουργεί εκ νέου ευρετήριο εγγράφων που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φακέλους ευρετηρίου.
type: docs
weight: 240
url: /el/net/groupdocs.search/index/update/
---
## Update() {#update}

Δημιουργεί εκ νέου ευρετήριο εγγράφων που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φακέλους ευρετηρίου.

```csharp
public void Update()
```

### Παραδείγματα

Το παράδειγμα δείχνει πώς να ενημερώσετε ένα ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

// Διαγράψτε έγγραφα από το φάκελο εγγράφων ή τροποποιήστε τα ή προσθέστε νέα έγγραφα στο φάκελο

index.Update(); // Ενημέρωση του ευρετηρίου
```

### Δείτε επίσης

* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Update(UpdateOptions) {#update_1}

Δημιουργεί εκ νέου ευρετήριο εγγράφων που έχουν αλλάξει ή διαγραφεί από την τελευταία ενημέρωση. Προσθέτει νέα αρχεία που έχουν προστεθεί στους φακέλους ευρετηρίου.

```csharp
public void Update(UpdateOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | UpdateOptions | Οι επιλογές ενημέρωσης. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να ενημερώσετε ένα ευρετήριο με συγκεκριμένες επιλογές ενημέρωσης.

```csharp
string indexFolder = @"c:\MyIndex\";
string documentsFolder = @"c:\MyDocuments\";

Index index = new Index(indexFolder); // Δημιουργία ευρετηρίου στον καθορισμένο φάκελο
index.Add(documentsFolder); // Δημιουργία ευρετηρίου εγγράφων από τον καθορισμένο φάκελο

// Διαγράψτε έγγραφα από το φάκελο εγγράφων ή τροποποιήστε τα ή προσθέστε νέα έγγραφα στο φάκελο

UpdateOptions options = new UpdateOptions();
options.Threads = 2; // Ρύθμιση του αριθμού των νημάτων ευρετηρίασης
index.Update(options); // Ενημέρωση του ευρετηρίου
```

### Δείτε επίσης

* class [UpdateOptions](../../../groupdocs.search.options/updateoptions)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->