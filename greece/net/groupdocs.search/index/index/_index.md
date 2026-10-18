---
title: "Index"
second_title: "GroupDocs.Search για .NET Αναφορά API"
description: "Αρχικοποιεί μια νέα παρουσία της κλάσης Indexgroupdocs.search/index στη μνήμη."
type: docs
weight: 10
url: /el/net/groupdocs.search/index/index/
---
## Index() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../../index) στη μνήμη.

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
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(IndexSettings) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../../index) στη μνήμη με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
public Index(IndexSettings settings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| settings | IndexSettings | Το αντικείμενο ρυθμίσεων του ευρετηρίου. |

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
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string) {#constructor_2}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../../index). Δημιουργεί ένα νέο ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο.

```csharp
public Index(string indexFolder)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου του ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε δίσκο ή να ανοίξετε ένα υπάρχον ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder); 
```

### Δείτε επίσης

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings) {#constructor_4}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../../index). Δημιουργεί ένα νέο ευρετήριο με συγκεκριμένες ρυθμίσεις ή ανοίγει ένα υπάρχον ευρετήριο στο δίσκο.

```csharp
public Index(string indexFolder, IndexSettings settings)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου του ευρετηρίου. |
| settings | IndexSettings | Το αντικείμενο ρυθμίσεων του ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings);
```

### Δείτε επίσης

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, bool) {#constructor_3}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../../index). Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν το *overwriteIfExists* είναι `false`; δημιουργεί ένα νέο ευρετήριο στο δίσκο διαφορετικά.

```csharp
public Index(string indexFolder, bool overwriteIfExists)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου του ευρετηρίου. |
| overwriteIfExists | Boolean | Η σημαία για την αντικατάσταση του φακέλου του ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα νέο ευρετήριο σε φάκελο που ήδη περιέχει άλλο ευρετήριο.

```csharp
string indexFolder = @"c:\MyIndex\";
Index index = new Index(indexFolder, true);
```

### Δείτε επίσης

* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

---

## Index(string, IndexSettings, bool) {#constructor_5}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Index`](../../index). Φορτώνει ένα υπάρχον ευρετήριο από το δίσκο εάν το *overwriteIfExists* είναι `false`; δημιουργεί ένα νέο ευρετήριο στο δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου διαφορετικά.

```csharp
public Index(string indexFolder, IndexSettings settings, bool overwriteIfExists)
```

| Parameter | Type | Περιγραφή |
| --- | --- | --- |
| indexFolder | String | Η διαδρομή του φακέλου του ευρετηρίου. |
| settings | IndexSettings | Το αντικείμενο ρυθμίσεων του ευρετηρίου. |
| overwriteIfExists | Boolean | Η σημαία για την αντικατάσταση του φακέλου του ευρετηρίου. |

### Παραδείγματα

Το παράδειγμα δείχνει πώς να δημιουργήσετε ένα ευρετήριο σε δίσκο με συγκεκριμένες ρυθμίσεις ευρετηρίου.

```csharp
string indexFolder = @"c:\MyIndex\";
IndexSettings settings = new IndexSettings();
settings.IndexType = IndexType.CompactIndex;
Index index = new Index(indexFolder, settings, true);
```

### Δείτε επίσης

* class [IndexSettings](../../indexsettings)
* class [Index](../../index)
* namespace [GroupDocs.Search](../../../groupdocs.search)
* assembly [GroupDocs.Search](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.search.dll -->
