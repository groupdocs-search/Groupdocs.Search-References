---
title: Index
second_title: GroupDocs.Αναζήτηση για αναφορά API .NET
description: Αρχικοποιεί μια νέα παρουσία τουIndexgroupdocs.search/index τάξη στη μνήμη.
type: docs
weight: 10
url: /el/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Index`](../../index) τάξη στη μνήμη.

```csharp
public Index()
```

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ευρετήριο στη μνήμη χωρίς αποθήκευση αρχείων στο δίσκο.

```csharp
Index index = new Index(); 
```

### Δείτε επίσης

* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Index`](../../index) κλάση στη μνήμη με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
public Index(IndexSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| settings | IndexSettings | Το αντικείμενο ρυθμίσεων ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ευρετήριο στη μνήμη χωρίς αποθήκευση αρχείων στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(settings);
```

### Δείτε επίσης

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία του[`Index`](../../index) class. Δημιουργεί ένα νέο ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο.

```csharp
public Index(string indexFolder)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε έναν δίσκο ή να ανοίξετε ένα υπάρχον ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Δείτε επίσης

* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία του[`Index`](../../index) class. Δημιουργεί ένα νέο ευρετήριο με συγκεκριμένες ρυθμίσεις ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου ευρετηρίου. |
| settings | IndexSettings | Το αντικείμενο ρυθμίσεων ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε έναν δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Δείτε επίσης

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία του[`Index`](../../index) class. Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν*overwriteIfExists* είναι`ψευδής`; δημιουργεί ένα νέο ευρετήριο στο δίσκο διαφορετικά.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου ευρετηρίου. |
| overwriteIfExists | Boolean | Η σημαία αντικατάστασης του φακέλου ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα νέο ευρετήριο σε έναν φάκελο που περιέχει ήδη άλλο ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Δείτε επίσης

* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία του[`Index`](../../index) class. Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν*overwriteIfExists* είναι`ψευδής` ; δημιουργεί ένα νέο ευρετήριο στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου διαφορετικά.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου ευρετηρίου. |
| settings | IndexSettings | Το αντικείμενο ρυθμίσεων ευρετηρίου. |
| overwriteIfExists | Boolean | Η σημαία αντικατάστασης του φακέλου ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε έναν δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Δείτε επίσης

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* χώρος ονομάτων [GroupDocs.Search](../../index)
* συνέλευση [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Search.dll -->
