---
title: "DocumentFilter"
second_title: "GroupDocs.Search για Java API Reference"
description: "Αντιπροσωπεύει τη βασική κλάση για φίλτρα εγγράφων."
type: docs
weight: 14
url: /el/java/com.groupdocs.search/documentfilter/
---
**Inheritance:**
java.lang.Object
```
public abstract class DocumentFilter
```

Αντιπροσωπεύει την βασική κλάση για φίλτρα εγγράφων. Περιέχει μεθόδους για τη δημιουργία παρουσιών φίλτρων εγγράφων.


**Learn more**

* [Document filtering during indexing](../https://docs.groupdocs.com/display/searchjava/Document+filtering+during+indexing)

## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentFilter()](#DocumentFilter--) |  |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
|  | [toString()](#toString--) | Επιστρέφει την αναπαράσταση ως συμβολοσειρά ενός φίλτρου εγγράφου. |
|
|  | [createCreationTimeLowerBound(Date lowerBound)](#createCreationTimeLowerBound-java.util.Date-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία δημιουργίας νωρίτερη από το κατώτερο όριο. |
|
|  | [createCreationTimeUpperBound(Date upperBound)](#createCreationTimeUpperBound-java.util.Date-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία δημιουργίας μεταγενέστερη από το ανώτερο όριο. |
|
|  | [createCreationTimeRange(Date lowerBound, Date upperBound)](#createCreationTimeRange-java.util.Date-java.util.Date-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία δημιουργίας εκτός του καθορισμένου εύρους. |
|
|  | [createModificationTimeLowerBound(Date lowerBound)](#createModificationTimeLowerBound-java.util.Date-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία τροποποίησης νωρίτερη από το κατώτερο όριο. |
|
|  | [createModificationTimeUpperBound(Date upperBound)](#createModificationTimeUpperBound-java.util.Date-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία τροποποίησης μεταγενέστερη από το ανώτερο όριο. |
|
|  | [createModificationTimeRange(Date lowerBound, Date upperBound)](#createModificationTimeRange-java.util.Date-java.util.Date-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία τροποποίησης εκτός του καθορισμένου εύρους. |
|
|  | [createFilePathRegularExpression(String pattern)](#createFilePathRegularExpression-java.lang.String-) | Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. |
|
|  | [createFilePathRegularExpression(String pattern, int options)](#createFilePathRegularExpression-java.lang.String-int-) | Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. |
|
|  | [createFileLengthLowerBound(long lowerBound)](#createFileLengthLowerBound-long-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με μήκος μικρότερο από το κατώτερο όριο. |
|
|  | [createFileLengthUpperBound(long upperBound)](#createFileLengthUpperBound-long-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με μήκος μεγαλύτερο από το ανώτερο όριο. |
|
|  | [createFileLengthRange(long lowerBound, long upperBound)](#createFileLengthRange-long-long-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων εκτός του καθορισμένου εύρους μήκους εγγράφου. |
|
|  | [createFileExtension(String[] extensions)](#createFileExtension-java.lang.String...-) | Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων που δεν έχουν επιτρεπόμενη επέκταση. |
|
|  | [createNot(DocumentFilter innerFilter)](#createNot-com.groupdocs.search.DocumentFilter-) | Δημιουργεί ένα φίλτρο που έχει αντίστροφη λογική σε σχέση με το καθορισμένο εσωτερικό φίλτρο. |
|
|  | [createAnd(DocumentFilter[] filters)](#createAnd-com.groupdocs.search.DocumentFilter...-) | Δημιουργεί μια λογική σύζευξη των καθορισμένων φίλτρων. |
|
|  | [createOr(DocumentFilter[] filters)](#createOr-com.groupdocs.search.DocumentFilter...-) | Δημιουργεί μια λογική διάζευξη των καθορισμένων φίλτρων. |
|
### DocumentFilter() {#DocumentFilter--}
```
public DocumentFilter()
```


### toString() {#toString--}
```
public abstract String toString()
```


Επιστρέφει την αναπαράσταση ως συμβολοσειρά ενός φίλτρου εγγράφου.


**Returns:**
java.lang.String - Αναπαράσταση ως συμβολοσειρά ενός φίλτρου εγγράφου.

### createCreationTimeLowerBound(Date lowerBound) {#createCreationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeLowerBound(Date lowerBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία δημιουργίας νωρίτερη από το κατώτερο όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Το κατώτερο όριο του χρόνου δημιουργίας του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeUpperBound(Date upperBound) {#createCreationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createCreationTimeUpperBound(Date upperBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία δημιουργίας μεταγενέστερη από το ανώτερο όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | upperBound | java.util.Date | Το άνω όριο του χρόνου δημιουργίας του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createCreationTimeRange(Date lowerBound, Date upperBound) {#createCreationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createCreationTimeRange(Date lowerBound, Date upperBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία δημιουργίας εκτός του καθορισμένου εύρους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Το κατώτερο όριο του χρόνου δημιουργίας του εγγράφου. |
|
|  | upperBound | java.util.Date | Το άνω όριο του χρόνου δημιουργίας του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document creation time.

### createModificationTimeLowerBound(Date lowerBound) {#createModificationTimeLowerBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeLowerBound(Date lowerBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία τροποποίησης νωρίτερη από το κατώτερο όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Το κάτω όριο του χρόνου τροποποίησης του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeUpperBound(Date upperBound) {#createModificationTimeUpperBound-java.util.Date-}
```
public static DocumentFilter createModificationTimeUpperBound(Date upperBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία τροποποίησης μεταγενέστερη από το ανώτερο όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | upperBound | java.util.Date | Το άνω όριο του χρόνου τροποποίησης του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createModificationTimeRange(Date lowerBound, Date upperBound) {#createModificationTimeRange-java.util.Date-java.util.Date-}
```
public static DocumentFilter createModificationTimeRange(Date lowerBound, Date upperBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με ημερομηνία τροποποίησης εκτός του καθορισμένου εύρους.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lowerBound | java.util.Date | Το κάτω όριο του χρόνου τροποποίησης του εγγράφου. |
|
|  | upperBound | java.util.Date | Το άνω όριο του χρόνου τροποποίησης του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document modification time.

### createFilePathRegularExpression(String pattern) {#createFilePathRegularExpression-java.lang.String-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern)
```


Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. Η κανονική έκφραση εφαρμόζεται στην πλήρη διαδρομή ενός εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | java.lang.String | Το μοτίβο της κανονικής έκφρασης. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFilePathRegularExpression(String pattern, int options) {#createFilePathRegularExpression-java.lang.String-int-}
```
public static DocumentFilter createFilePathRegularExpression(String pattern, int options)
```


Δημιουργεί ένα φίλτρο για την παράλειψη εγγράφων που δεν ταιριάζουν με μια κανονική έκφραση. Η κανονική έκφραση εφαρμόζεται στην πλήρη διαδρομή ενός εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | pattern | java.lang.String | Το μοτίβο της κανονικής έκφρασης. |
|
|  | options | int | Οι επιλογές της κανονικής έκφρασης. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by file name.

### createFileLengthLowerBound(long lowerBound) {#createFileLengthLowerBound-long-}
```
public static DocumentFilter createFileLengthLowerBound(long lowerBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με μήκος μικρότερο από το κατώτερο όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lowerBound | long | Το κάτω όριο του μήκους του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthUpperBound(long upperBound) {#createFileLengthUpperBound-long-}
```
public static DocumentFilter createFileLengthUpperBound(long upperBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων με μήκος μεγαλύτερο από το ανώτερο όριο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | upperBound | long | Το άνω όριο του μήκους του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileLengthRange(long lowerBound, long upperBound) {#createFileLengthRange-long-long-}
```
public static DocumentFilter createFileLengthRange(long lowerBound, long upperBound)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων εκτός του καθορισμένου εύρους μήκους εγγράφου.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | lowerBound | long | Το κάτω όριο του μήκους του εγγράφου. |
|
|  | upperBound | long | Το άνω όριο του μήκους του εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document length.

### createFileExtension(String[] extensions) {#createFileExtension-java.lang.String...-}
```
public static DocumentFilter createFileExtension(String[] extensions)
```


Δημιουργεί ένα φίλτρο για παράλειψη εγγράφων που δεν έχουν επιτρεπόμενη επέκταση.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | extensions | java.lang.String[] | Η λίστα των επιτρεπόμενων επεκτάσεων. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter by document extension.

### createNot(DocumentFilter innerFilter) {#createNot-com.groupdocs.search.DocumentFilter-}
```
public static DocumentFilter createNot(DocumentFilter innerFilter)
```


Δημιουργεί ένα φίλτρο που έχει αντίστροφη λογική σε σχέση με το καθορισμένο εσωτερικό φίλτρο.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | innerFilter | [DocumentFilter](../../com.groupdocs.search/documentfilter) | Το εσωτερικό φίλτρο εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - An inverted document filter.

### createAnd(DocumentFilter[] filters) {#createAnd-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createAnd(DocumentFilter[] filters)
```


Δημιουργεί μια λογική σύζευξη των καθορισμένων φίλτρων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Τα φίλτρα εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of conjunction of the specified filters.

### createOr(DocumentFilter[] filters) {#createOr-com.groupdocs.search.DocumentFilter...-}
```
public static DocumentFilter createOr(DocumentFilter[] filters)
```


Δημιουργεί μια λογική διάζευξη των καθορισμένων φίλτρων.


**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | filters | [DocumentFilter\[\]](../../com.groupdocs.search/documentfilter) | Τα φίλτρα εγγράφου. |
|

**Returns:**
[DocumentFilter](../../com.groupdocs.search/documentfilter) - A document filter that represents result of disjunction of the specified filters.

